# Diagrama AS-IS: pagamento do Seguro-Desemprego não localizado

Complementa `C_blueprint_asis.md`, onde estão as descrições, categorias e fontes dos fail points.

**Como ler:** seta cheia é o fluxo da jornada ou uma interação; seta tracejada é ligação não comprovada, hipótese ou associação de fail point. Vermelho marca fail points; amarelo, saídas laterais.

```mermaid
flowchart TD
    CID(["Cidadão"])

    subgraph JORNADA["Etapas da jornada"]
        direction TB
        E1["1. Perceber"]
        E2["2. Buscar canal"]
        E3["3. Ligar e navegar"]
        E4["4. Identificar e consultar"]
        E5["5. Receber resposta"]
        E6{"6. Avaliar resolução<br/>obteve F2?"}
        E7["7. Encerrar, repetir ou migrar"]
        OK(["Resolvido: sabe onde ou quando<br/>o dinheiro estará disponível"])
        DES(["Desistiu"])
    end

    subgraph FRONT["Frontstage: o que o cidadão percebe"]
        PAG["Páginas CAIXA e MTE"]
        CTPS["CTPS Digital"]
        TEM["CAIXA Tem"]
        URA["URA 0800 726 0207"]
        ATD["Atendente CAIXA"]
    end

    subgraph BACK["Backstage: atende esta ligação"]
        ROT["Roteamento e fila - L"]
        CONS["Identificação e consulta - L"]
        PROT["Registro de protocolo - L"]
        OPER["Operador da central - L"]
    end

    subgraph SUP["Processos de Suporte"]
        CAIXA["CAIXA"]
        BASES[("Sistema Seguro-Desemprego e bases")]
        LOTES["Processamento de lotes<br/>e arquivos de pagamento"]
        TEL["Infraestrutura telefônica"]
        DTP["Dataprev"]
        DEST["Instituição financeira de destino"]
    end

    subgraph MIGRA["Canais de migração"]
        AG["Agência CAIXA"]
        LOT["Lotérica - L"]
        SAC["SAC CAIXA 0800 726 0101"]
        OUV["Ouvidoria CAIXA 0800 725 7474"]
        RA["Reclame Aqui"]
    end

    subgraph LATMTE["Saída lateral: competência"]
        MTE["MTE"]
        C158["Central 158"]
        GOV["Gov.br"]
    end

    subgraph LATAC["Saída lateral: acessibilidade"]
        LIB["Atendimento em Libras"]
        L2492["Linha 0800 726 2492"]
    end

    %% Fluxo da jornada
    CID --> E1
    E1 --> E2 --> E3 --> E4 --> E5 --> E6
    E6 -->|"sim"| OK
    E6 -->|"não"| E7
    E7 -->|"liga de novo"| E3
    E7 -->|"abandona"| DES
    E3 -->|"chamada encerrada"| E7

    %% Interações
    E1 --> CTPS
    E1 --> TEM
    E2 --> PAG
    E3 --> URA
    E4 --> URA
    E5 --> URA
    E5 --> ATD

    %% Linha de visibilidade e backstage
    URA --> ROT
    ROT --> ATD
    URA -.-> CONS
    ATD -.-> CONS
    ATD -.-> PROT
    OPER -.->|"quem opera não é conhecido"| URA

    %% Suporte
    CONS -.->|"ligação não comprovada"| BASES
    TEL --> URA
    CAIXA -->|"responde pelo canal"| URA
    CAIXA --> LOTES
    LOTES -->|"movimento liquidado"| DTP
    DTP --> BASES
    LOTES -->|"TED"| DEST
    LOTES -->|"crédito em poupança CAIXA"| TEM
    MTE -->|"gere e contrata"| CAIXA

    %% Migração
    E7 --> AG
    E7 -.-> LOT
    E7 --> SAC
    SAC -.-> OUV
    E7 --> RA
    E7 --> CTPS

    %% Saídas laterais
    E3 -.->|"bloqueio ou recurso"| MTE
    E5 -.->|"habilitação, bloqueio ou recurso"| MTE
    E7 -.->|"decisão fora da CAIXA"| MTE
    MTE --> C158
    MTE --> GOV
    MTE --> CTPS
    E3 -.->|"pessoa surda"| LIB
    E3 -.->|"deficiência auditiva ou de fala"| L2492
    LIB -.->|"aciona o SAC"| SAC

    %% Fail points
    F03["FP-03: consta paga, não está onde se esperava<br/>FP-05: paga não garante disponibilidade"]
    H09["HP-09: dúvida entre 0800 e 158"]
    F01["FP-01: espera longa e chamada encerrada<br/>RA-01: voz não atende pessoa surda<br/>HA-01: equivalência das alternativas<br/>HP-08: humano fora do horário<br/>HP-01: menu sem bloqueio ou recurso"]
    H03["HP-03: atendente não vê a causa<br/>HP-06: sistema indisponível<br/>HP-07: base defasada"]
    F02["FP-02: orientação ao app sem F2<br/>HP-05: status sem origem"]
    FC["FP-C: encerra sem a informação de F2"]
    H02["HP-02: repetir CPF ou NIS<br/>HP-04: sem protocolo ou contexto"]
    F04["FP-04: pagador não decide o benefício"]
    F06["FP-06: arquivo rejeitado<br/>sem relato neste cenário"]

    F03 -.- E1
    H09 -.- E2
    F01 -.- E3
    H03 -.- E4
    F02 -.- E5
    FC -.- E6
    H02 -.- E7
    F04 -.- MTE
    F06 -.- LOTES

    classDef falha fill:#fde2e2,stroke:#b42318,color:#1a1a1a
    classDef lateral fill:#fff3cd,stroke:#8a6d00,color:#1a1a1a
    class F03,H09,F01,H03,F02,FC,H02,F04,F06 falha
    class MTE,C158,GOV,LIB,L2492 lateral
```

## Ressalvas

- **L** indica lacuna: elemento não comprovado em fonte pública.
- Os relatos mostram que o problema ocorre, não que é o mais frequente.
- A ligação entre a consulta da chamada e as bases não está comprovada.
- Nenhuma transferência técnica entre CAIXA e MTE está comprovada: as setas de saída lateral indicam mudança de canal.
- A CTPS Digital aparece como tela consultada antes da ligação e como canal de migração.
