# Service Blueprint AS-IS: atendimento ao Seguro-Desemprego pela URA da CAIXA

**Base:** `B_relatorio_assistente_v3.md` (data de corte 24/11/2026) e decisões das rodadas 1 a 8 da entrevista, citadas como (R1) a (R8).

**Método:** Service Blueprint de Shostack, que originou os fail points e a linha de visibilidade. As cinco camadas e três linhas usadas aqui incorporam refinamentos posteriores (Kingman-Brundage; Bitner e colegas).

## Escopo

| Item | Definição |
|---|---|
| Cenário principal | Pagamento não localizado (R1) |
| Saída lateral | Demanda de habilitação, bloqueio ou recurso, que sai da competência da CAIXA e vai para o MTE (R1) |
| Protagonista | Trabalhador formal dispensado que espera uma parcela prevista. É construção analítica, não usuário típico comprovado (R3) |
| Variantes | Recebimento por TED em outra instituição ou em poupança CAIXA (R3) |
| Fora do escopo | Modalidades especiais, como o trabalhador resgatado (R3) |
| Início | O cidadão percebe, ainda antes de ligar, que o dinheiro não está onde esperava (R2) |
| Fim | Qualquer desfecho observável: resolvido, migrou de canal, ligou de novo ou desistiu (R2) |
| Critério de sucesso (F2) | O cidadão localiza o dinheiro ou sabe quando e onde ele estará disponível (R2) |
| Limite da evidência | Os relatos mostram que o problema ocorre, não que é o mais frequente (R1) |

**Marcadores:** `[F]` fato documentado; `[I]` inferência; `[L]` lacuna, não comprovado.

## Blueprint

| Camada / linha | 1. Perceber | 2. Buscar canal | 3. Ligar e navegar | 4. Identificar e consultar | 5. Receber resposta | 6. Avaliar resolução | 7. Encerrar, repetir ou migrar |
|---|---|---|---|---|---|---|---|
| **Evidências Físicas** | [F] CTPS Digital, CAIXA Tem, extrato, data e status, requerimento (R8) | [F] Páginas e apps que divulgam 0800 e 158 (R8) | [F] Número 0800 726 0207<br>[L] Voz, menus, som ou silêncio da espera (R8) | [L] Dados pedidos pela URA (R8) | [F] Informação falada<br>[L] Roteiro (R8) | [I] O que ouviu comparado ao extrato ou à conta (R8) | [I] Registro da chamada no aparelho<br>[L] Protocolo e comprovante<br>[F] Resposta no Reclame Aqui, quando há<br>[F] Cartão do Cidadão e senha, para recebimento¹<br>[L] Lotérica¹ (R8) |
| **Ações do Cidadão** | Percebe que o dinheiro não está onde esperava (R2) | Escolhe um canal (R2) | Liga, ouve, digita e espera (R5) | Identifica-se [L] (R5) | Ouve a URA ou o atendente (R5) | Verifica se obteve F2 (R2) | Encerra, liga de novo, migra ou desiste (R2) |
| ***Linha de Interação*** | — | — | — | — | — | — | — |
| **Frontstage** | [F] Status e data exibidos nos canais digitais (R8) | [F] Canais divulgados pela CAIXA e pelo MTE (R8) | [F] URA 0800 726 0207<br>Menus, mensagens, espera e queda da chamada (R5) | [L] Pergunta de identificação (R5) | [F] URA ou Atendente CAIXA<br>Dado verbalizado como fala (R5) | — | [F] Agência CAIXA, SAC CAIXA 0800 726 0101, Ouvidoria CAIXA 0800 725 7474, canais digitais (R2)<br>Saída lateral: MTE (R1) |
| ***Linha de Visibilidade*** (separa o que o cidadão percebe do que não percebe, R5) | — | — | — | — | — | — | — |
| **Backstage** (feito para atender esta ligação, R6) | — | — | [L] Roteamento e fila (R6) | [L] Identificação do chamador<br>[L] Consulta pela URA ou pelo atendente (R6) | [L] Origem do dado (R5)<br>[I] Telas e classificação da demanda (R6) | — | [L] Registro de protocolo (R6) |
| ***Linha de Interação Interna*** (separa o que serve à chamada do que roda sem ela, R6) | — | — | — | ⇣ ligação entre consulta e bases **não comprovada** [L] (R6) | — | — | — |
| **Processos de Suporte** (rodam mesmo sem a ligação, R6) | [F] Processamento de lotes e arquivos de pagamento<br>[F] TED ou crédito em poupança (R6)<br>[F] CAIXA, Dataprev e Instituição financeira de destino (v3) | [F] Normas e Contrato 07/2026 (R6, R8) | [F] Infraestrutura telefônica<br>[L] Dimensionamento de atendentes (R6) | [F] Sistema Seguro-Desemprego e bases (R6) | [L] Operador da central | — | [F] Normas de competência e recurso (R6) |
| **Fail points** | **FP-03** [F], **FP-05** [F, risco] (R7) | **HP-09** [L] (R7) | **FP-01** [F], **RA-01** [restrição], **HA-01** [L], **HP-08** [I], **HP-01** [L] (R4, R7) | **HP-03** [I], **HP-06** [I], **HP-07** [I] (R7) | **FP-02** [F], **HP-05** [L] (R7) | **FP-C** [F], ponto central (R7) | **HP-02** [L], **HP-04** [I], **FP-04** [restrição] (R7) |

¹ Ver a nota sobre evidências de recebimento, abaixo.

## Fail points

Entra o que pode impedir F2 (R7).

| ID | Etapa | Categoria | Descrição | Base |
|---|---|---|---|---|
| FP-03 | 1. Perceber | Ocorrência documentada | Parcela consta como paga, mas não está onde o cidadão esperava. A falha começa antes da ligação (R7) | S11 |
| FP-05 | 1. Perceber | Risco documentado | "Emitida" ou "paga" não prova disponibilidade imediata na conta consultada (R7) | S03, S05, S09–S11 |
| HP-09 | 2. Buscar canal | Hipótese [L] | Dúvida entre o 0800 da CAIXA e o 158 do MTE. Não há evidência de confusão generalizada (R7) | Nova, sem origem no v3 |
| FP-01 | 3. Ligar e navegar | Ocorrência documentada | Espera de 40 minutos e chamada encerrada, sem causa atribuída (R5, R7). Relato distinto registra mais de 20 minutos de espera | S09, S10 |
| RA-01 | 3. Ligar e navegar | Restrição estrutural | Canal só de voz não atende diretamente uma pessoa surda. Decorre da natureza do canal (R4) | Não depende de relato |
| HA-01 | 3. Ligar e navegar | Hipótese [L] | Não está provado nem refutado que o Atendimento em Libras e a linha 0800 726 2492 entreguem as funções da URA para este pagamento (R4) | S12 e fonte nova² |
| HP-08 | 3. Ligar e navegar | Hipótese [I, média] | Necessidade de atendimento humano fora do horário da CAIXA (R7) | S02, S06 |
| HP-01 | 3. Ligar e navegar → saída lateral | Hipótese [L] | Menu não cobrir bloqueio ou recurso (R7) | v3 |
| HP-03 | 4. Identificar e consultar | Hipótese [I, baixa] | Atendente ver o pagamento, mas não a causa detalhada (R7) | v3 |
| HP-06 | 4. Identificar e consultar | Hipótese [I, baixa] | Indisponibilidade de sistema degradar a URA (R7) | v3 |
| HP-07 | 4. Identificar e consultar | Hipótese [I, baixa] | Base da central defasada (R7) | v3 |
| FP-02 | 5. Receber resposta | Ocorrência documentada | Orientação para consultar o app. Só é falha se o cidadão sair sem F2 (R7) | S10 |
| HP-05 | 5. Receber resposta | Hipótese [L] | URA informar status sem explicar a origem (R7) | v3 |
| **FP-C** | 6. Avaliar resolução | Ocorrência documentada | **O cidadão encerra o contato sem a informação de F2** (R2, R7) | S09, S10, S11³ |
| HP-02 | 7. Encerrar, repetir ou migrar | Hipótese [L] | Repetir CPF ou NIS ao mudar de canal (R7) | v3 |
| HP-04 | 7. Encerrar, repetir ou migrar | Hipótese [I, média] | Redirecionamento sem protocolo ou contexto (R7) | v3 |
| FP-04 | Saída lateral | Restrição estrutural | Habilitação e recurso não são decididos pelo agente pagador (R1, R7) | S03–S05 |
| FP-06 | Suporte | Restrição documental | Arquivo de pagamento inconsistente pode ser rejeitado. **Nenhum relato o liga a este cenário** (R7) | S03 |

Os identificadores RA-01, HA-01, HP-09 e FP-C foram criados neste blueprint.

## Saídas laterais

| Saída | De onde | Para onde | Ressalva |
|---|---|---|---|
| Competência (R1) | Etapas 3, 5 ou 7 | MTE: Central 158, CTPS Digital, Gov.br | [L] Transferência técnica e protocolo compartilhado não comprovados |
| Acessibilidade (R4) | Etapa 3 | Atendimento em Libras; linha 0800 726 2492 | [L] Equivalência com a URA não comprovada |

## Notas de leitura

- **Quem atende não é quem decide:** o v3 trata a afirmação como inferência `[I, confiança alta]`. Aparece pelos nomes dos atores e pela saída lateral, não pela Linha de Visibilidade (R5).
- **Espera:** a percepção fica acima da linha; a fila fica no Backstage; o dimensionamento que define a fila fica em Suporte (R5, R6). O v3 não descreve música de espera.
- **Backstage cheio de [L]:** é um achado do diagnóstico. A parte mais próxima do cidadão é a menos documentada (R6).
- **Comprovante:** a falta de comprovante da informação recebida é lacuna `[L]`, não falha (R8).
- **Evidências de recebimento:** Cartão do Cidadão e senha servem ao recebimento e não estão comprovados como identificação na URA (R8). Essa ressalva e a senha vêm da **v2** (fonte S12 da v2, CAIXA, "Cartão do Cidadão"), não do v3. O v3 cita o cartão como meio de recebimento. A lotérica para saque não tem fonte no v3.
- **F09:** o apontamento sobre essas evidências é da auditoria v1 (R8).

² Fonte nova, fora do v3: [Acessibilidade CAIXA](https://www.caixa.gov.br/acessibilidade/Paginas/default.aspx) e [Atendimento em Libras](https://www.caixa.gov.br/libras). Consultadas apenas por resumo de busca em 26/11/2026; as páginas não foram abertas. O resumo indica que a videochamada em Libras aciona o SAC, não o Atendimento CAIXA Cidadão.

³ Os relatos indicam contato sem F2 e há resposta pública posterior nos três. Isso não prova que foi a primeira vez que o cidadão recebeu a informação, nem que o dinheiro foi localizado.

**Fontes S01–S14:** ver as referências em `B_relatorio_assistente_v3.md`. Não foram reverificadas para este blueprint.
