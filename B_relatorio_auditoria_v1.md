# Auditoria da v1 — Operação AS-IS do Atendimento ao Seguro-Desemprego pela URA da Caixa

- **Auditor (assistente 2):** Claude (Anthropic), via Claude.ai
- **Documento auditado:** `B_relatorio_assistente_v1.md`, produzido pelo ChatGPT (OpenAI) com Pesquisa aprofundada
- **Data:** 24/11/2026
- **Escopo:** erros factuais, etapas de bastidor omitidas, evidências físicas e normativos ausentes, fail points não identificados, inferências mal-suportadas e fontes fracas. Questões cosméticas não foram contadas.

## Método e verificações feitas

Leitura integral da v1, confrontada com o prompt que a originou, e verificação na web (24/11/2026) de quatro pontos:

1. **Horários do 0800 726 0207:** a página de atendimento da Caixa confirma atendimento humano de segunda a sexta, das 8h às 21h, e aos sábados, das 10h às 16h. **Correto na v1.**
2. **Resolução CODEFAT nº 1.043/2026:** existe (26/08/2026, DOU extra de 31/08/2026), mas trata da ampliação para até seis parcelas do **trabalhador resgatado**. Ver F06.
3. **Íntegra do Contrato MTE nº 07/2026:** o portal do MTE publica o arquivo completo do contrato (`.../licitacoes-e-contratos/pca/072026completo.pdf`). Ver F01.
4. **Outros canais da Caixa:** a mesma página de atendimento lista SAC CAIXA (0800 726 0101), Ouvidoria CAIXA (0800 725 7474, dias úteis, 9h–18h) e atendimento em Libras por parceiro. Ver F09 e F10.

**Veredito geral:** a v1 é sólida na divisão institucional (MTE decide, Dataprev processa, Caixa paga) e honesta sobre as lacunas da URA. As falhas mais graves são: afirmar que a íntegra do contrato vigente não foi localizada quando ela é pública; usar o rótulo [F] para cenários hipotéticos; e omitir evidências físicas, canais de escalonamento e etapas de bastidor que mudam o blueprint. Foram identificadas **16 falhas (F01 a F16)**.

---

## 1. Erros factuais e fontes fracas

**F01 — Íntegra do contrato vigente tratada como não localizada.**
Trecho: *"não foi localizada, na documentação pública recuperada, a íntegra contratual ou cláusula de 2026 que demonstre se a URA é item tarifável específico"*. O MTE publica o PDF completo do Contrato nº 07/2026. A pergunta central sobre a remuneração da URA no Seguro-Desemprego pode ser respondida por leitura direta. A v1 usou o contrato do Abono como "evidência comparativa" quando a fonte primária estava disponível.

**F02 — Nenhuma referência tem link.**
Seção "Referências verificáveis": as fontes S01 a S16 têm título e data, mas **nenhum link direto**, contrariando o item 6.8 do prompt. Também faltam artigo, cláusula ou página na maioria (S01, S02, S05, S10, S12). Sem links, as afirmações [F] não são verificáveis por terceiros.

**F03 — Sistema de rótulos confuso e incoerente.**
Trecho: *"nas referências, acrescenta-se o sufixo -F para fonte oficial/primária, -I para informe/indústria e -L para relato, controle, legislativo ou usuário"*. O sufixo "-L" reúne relatos de usuário, órgãos de controle e textos legislativos. Resultado: o TCU (S09) aparece como "-L", a mesma letra que significa "lacuna" no corpo do texto. A sobreposição dificulta saber se uma afirmação é lacuna ou fonte de controle.

**F04 — Rótulo [F] aplicado a cenários hipotéticos.**
Na matriz, etapa "Perceber a necessidade": *"[F] Percebe parcela não liberada, status pendente, bloqueio ou dúvida"*. Isso é um cenário de jornada, não um fato documentado. O mesmo ocorre em *"[F] Busca CAIXA, MTE, Gov.br ou telefone"* e *"[F] confronta resposta com problema concreto"*. O prompt exigia não tratar a jornada hipotética como fato.

**F05 — Fail point FP-01 classificado como documentado sem evidência.**
Trecho: *"FP-01 … [F] coexistem 0800 CAIXA e 158/MTE com escopos sobrepostos na percepção do cidadão"*. A coexistência dos canais é fato; a confusão "na percepção do cidadão" é inferência. A própria seção de questões admite: *"FP-01: a dificuldade de localizar o canal correto é estrutural ou apenas potencial?"*. Deveria estar entre os hipotéticos ou rotulado [I].

**F06 — Normativo citado sem dizer o que muda.**
Trecho: *"Resolução CODEFAT nº 1.043/2026 | altera Res. 957 | … | demonstra atualização normativa recente"*. A resolução amplia para até seis parcelas o benefício do trabalhador resgatado. É irrelevante para a jornada do trabalhador formal na URA, ou, se relevante, a v1 não explica por quê. Citar norma sem conteúdo é ruído na seção de normativos.

**F07 — FP-08 não é fail point da jornada.**
Trecho: *"FP-08 | Consistência sistêmica | Auditoria do TCU encontrou falhas de controle e inconsistências em processamento"*. A própria v1 reconhece *"não prova falha na URA"*. Falhas de controle de pagamentos indevidos não são, por si, um ponto em que o cidadão desiste ou recebe resposta errada no atendimento. Sem nexo com uma etapa, o item deveria ser hipotético ou sair da lista.

**F08 — Diagrama de fluxo perdido.**
A seção "Fluxo da jornada" traz só rótulos soltos ("Sim", "Não", "Escolhe CAIXA?") e a indicação "Exibir código". O código do diagrama não foi incluído no relatório, e as ramificações que ele representaria não podem ser examinadas.

## 2. Evidências físicas omitidas

**F09 — Cartão do Cidadão e senha ausentes.**
A página oficial de atendimento da Caixa informa que o Seguro-Desemprego pode ser sacado no autoatendimento *com o cartão do cidadão*. O Cartão do Cidadão e sua senha são evidências físicas centrais da jornada de recebimento, e potencialmente da identificação no telefone, mas não aparecem em nenhuma célula da matriz. Também faltam: número do requerimento, comunicado de dispensa, notificações da CTPS Digital e a Poupança Social Digital (CAIXA Tem) como destino do crédito.

**F10 — Canais de acessibilidade ignorados.**
O prompt pedia regras de acessibilidade. A Caixa mantém atendimento em Libras por empresa parceira e linha para pessoas com deficiência auditiva. Para um blueprint centrado no cidadão, a ausência de qualquer menção a como uma pessoa surda percorre a jornada telefônica é uma lacuna real.

## 3. Etapas de bastidor omitidas

**F11 — Fluxo de arquivos MTE → Caixa não descrito.**
A v1 cita os arts. 64 a 66 da Res. 957 (pagamento), mas não descreve o bastidor que faz a informação de "parcela liberada" chegar à Caixa: geração e envio dos arquivos de pagamento pelo MTE/Dataprev, processamento pela Caixa, retorno de pagamentos realizados e não realizados. É esse fluxo que determina se a URA "sabe" algo. Sem ele, a camada Backstage das etapas 3 a 5 fica vazia ou genérica.

**F12 — Escalonamento interno da Caixa ausente.**
SAC CAIXA (0800 726 0101) e Ouvidoria CAIXA (0800 725 7474) são as instâncias para onde vai a reclamação não resolvida. A v1 menciona Ouvidoria só em pergunta final (*"há uso recorrente de … Ouvidoria CAIXA ou Fala.BR"*) e não a coloca na jornada nem nos pontos de transferência. Isso empobrece a etapa 7 (migrar, repetir ou encerrar).

## 4. Fail points não identificados

**F13 — Nível da conta gov.br como barreira.**
A carta de serviço do Seguro-Desemprego remete ao nível da conta gov.br para acesso digital. Quando a Caixa orienta o cidadão a usar a CTPS Digital (FP-07), ele pode esbarrar na exigência de conta prata ou ouro. É um fail point da transição telefone → canal digital, não registrado.

**F14 — Assimetria de horários entre canais.**
O 0800 tem atendimento humano até 21h (16h aos sábados) e nenhum aos domingos; a Central 158 é informada pela própria v1 como de segunda a sábado, 7h–22h. Fora desses horários, o cidadão só tem a URA eletrônica, cujas funções são desconhecidas. A v1 registra os horários, mas não os transforma em fail point (demanda que exige humano fora do horário).

**F15 — Diferença entre "parcela paga" e "valor disponível" sem bastidor.**
FP-05 está correto como experiência relatada, mas a v1 não investiga a causa no bastidor (crédito por TED em dia útil, destino em conta poupança diversa da esperada). A resposta posterior da Caixa no próprio relato indica que a informação existia, mas não chegou ao cidadão pelo telefone. Isso sugere um fail point de **comunicação**, não de sistema, distinção importante para a camada em que o problema se situa.

## 5. Inferência mal-suportada

**F16 — "Confiança alta" para inferência sem base operacional.**
Trecho: *"[I, alta] operador classifica demanda conforme competência"* (Backstage da etapa "Avaliar resolução"). Não há nenhuma fonte sobre o trabalho do atendente: a própria v1 lista como lacuna as *"telas usadas por atendentes"* e as *"regras de roteamento"*. Uma inferência sobre o comportamento interno do operador, sem documento, não pode ter confiança alta.

---

## Quadro-resumo

| ID | Tipo | Gravidade para o blueprint |
|---|---|---|
| F01 | Erro factual (contrato não lido) | Alta |
| F02 | Fontes sem link | Alta |
| F03 | Rótulos incoerentes | Média |
| F04 | [F] em cenário hipotético | Média |
| F05 | Fail point sem evidência | Média |
| F06 | Normativo sem conteúdo | Baixa |
| F07 | Fail point sem nexo com etapa | Média |
| F08 | Diagrama perdido | Baixa |
| F09 | Evidências físicas omitidas | Alta |
| F10 | Acessibilidade omitida | Média |
| F11 | Bastidor do fluxo de arquivos omitido | Alta |
| F12 | Escalonamento SAC/Ouvidoria omitido | Média |
| F13 | Fail point: nível da conta gov.br | Média |
| F14 | Fail point: horários | Média |
| F15 | Fail point de comunicação | Média |
| F16 | Confiança inflada | Média |

## Recomendação para a v2

Tratar **cada** falha F01–F16 com (a) correção, (b) defesa com evidência ou (c) marcação como pendente, começando por uma **tabela de tratamento no início do relatório**. Prioridade: F01 (ler o Contrato 07/2026), F02 (links diretos), F09 e F11 (evidências físicas e bastidor do pagamento). A v2 deve manter o tamanho próximo ao da v1 (cerca de 4.000 palavras), substituindo trechos em vez de só acrescentar.
