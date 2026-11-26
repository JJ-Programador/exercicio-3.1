# Diagnóstico AS-IS v2 — Atendimento ao Seguro-Desemprego pela URA/Atendimento CAIXA Cidadão

| Falha | Tratamento | Tratamento na v2 | Seção alterada |
|---|---|---|---|
| **F01** | **a** | Lida a íntegra do Contrato MTE nº 07/2026: a remuneração contratual é **R$ 2,25 por parcela paga**, não por atendimento/URA; “URA” não aparece no PDF como item remunerado. | Bastidores; Normativos |
| **F02** | **a** | Referências passam a indicar link direto e dispositivo, cláusula, página ou seção relevante. | Referências |
| **F03** | **a** | `[F]/[I]/[L]` passam a indicar **somente estatuto epistemológico**. A natureza da fonte é registrada separadamente nas referências. | Síntese; Referências |
| **F04** | **a** | Motivações e trajetórias possíveis do cidadão que não têm ocorrência documentada são classificadas `[I]`, não `[F]`. | Matriz |
| **F05** | **a** | A coexistência de 0800 CAIXA e 158/MTE é fato; eventual **confusão do cidadão** passa a ser fail point hipotético `[I]`. | Fail points |
| **F06** | **a** | A Resolução 1.043/2026 é delimitada à ampliação de parcelas do **trabalhador resgatado** e não usada para caracterizar a jornada geral do trabalhador formal. | Normativos |
| **F07** | **a** | O achado do TCU sai dos fail points da URA; permanece apenas como evidência contextual do processamento/status de pagamento. | Bastidores; Fail points |
| **F08** | **a** | Incluído fluxo textual completo, com ramificações e incertezas explícitas. | Matriz |
| **F09** | **a** | Incluídos Requerimento, CPF, Cartão do Cidadão/Social, senha, documentação de dispensa, CTPS Digital e CAIXA Tem; **nenhum deles é presumido como autenticação telefônica**. | Matriz; Bastidores |
| **F10** | **a** | Incluídos atendimento para pessoa surda/com deficiência auditiva e Libras/ICOM; integração específica com a URA do Seguro-Desemprego permanece `[L]`. | Matriz; Transferências |
| **F11** | **a** | Reconstruído o fluxo de lotes/arquivos MTE→CAIXA e retornos CAIXA→Dataprev/MTE; relação direta desses arquivos com consultas da URA permanece não comprovada. | Bastidores |
| **F12** | **a** | SAC e Ouvidoria CAIXA entram como canais de reclamação/escalonamento; não são tratados como transferência integrada sem prova. | Transferências |
| **F13** | **b** | A alegação da auditoria de exigência “prata ou ouro” é **refutada**: a carta atual admite conta **Bronze, Prata ou Ouro**. | Fail points; Normativos |
| **F14** | **a** | Assimetria de horários é registrada como condição documentada; o efeito de produzir falha para um cidadão específico é classificado como hipótese. | Fail points |
| **F15** | **a** | Recuperada a fonte original do relato; distinguem-se “parcela emitida/paga”, liquidação de TED em dia útil e conta de destino. O caso sustenta falha individual de **comunicação**, não falha sistêmica da URA. | Fail points; Bastidores |
| **F16** | **a** | Retirada a confiança alta na atuação do operador. Regras, telas e critérios de classificação de demanda permanecem `[L]`; qualquer roteamento interno inferido é de baixa confiança. | Matriz; Bastidores |

A tabela acima responde individualmente às 16 falhas da auditoria obrigatória. fileciteturn1file0 A **v1 original não estava disponível como arquivo acessível nesta execução**; por isso, esta v2 foi reconstruída a partir dos trechos reproduzidos na auditoria e de verificação independente das fontes, sem inventar conteúdo ausente.

## Síntese executiva

**Convenção.** `[F]` = fato confirmado diretamente pela evidência; `[I]` = inferência, sempre com confiança indicada quando relevante; `[L]` = lacuna documental. Isso é independente da **natureza da fonte** — oficial primária, oficial institucional, controle/auditoria ou relato de usuário.

Na data de corte, **24/11/2026**, a CAIXA apresenta o **0800 726 0207 — Atendimento CAIXA Cidadão** como canal para PIS, benefícios sociais, FGTS e Cartão Social; sua FAQ específica inclui esse número entre os meios para acompanhar parcela do Seguro-Desemprego. O atendimento eletrônico é informado como 24×7 e o humano como segunda a sexta, 8h–21h, e sábado, 10h–16h. citeturn150084search0turn150084search3

A divisão institucional permanece o principal achado do AS-IS. `[F]` O MTE responde pela concessão e pelo sistema que emite parcelas; a Dataprev declara operar o sistema que verifica se o cidadão atende aos requisitos; e a CAIXA é normativamente o agente pagador. A própria CAIXA encaminha dúvidas de **concessão e valor** aos canais do MTE. Portanto, a hipótese “quem atende não é necessariamente quem decide” é confirmada **para parte das demandas**, mas não significa que o 0800 seja incapaz de informar pagamentos: a CAIXA o divulga justamente como canal de consulta de parcela. citeturn946820view10turn452304view6turn150084search0

A leitura integral do Contrato MTE nº 07/2026 corrige um erro material da v1. `[F]` O contrato remunera a CAIXA por **parcelas do Seguro-Desemprego**, à razão de R$ 2,25 cada; não há item tarifário de URA e a busca integral não encontrou a expressão “URA”. O Termo de Referência admite “atendimento ao público” como serviço acessório eventualmente subcontratável, explicitando que ele **não integra o objeto principal**. Isso não prova inexistência de custos ou operação de URA; prova apenas que este contrato não estabelece remuneração específica por atendimento telefônico. citeturn452304view0turn403732view0turn403732view1turn403732view2

As lacunas críticas continuam sendo a árvore de menus do Seguro-Desemprego, prompts gravados, dados solicitados para identificação telefônica, telas do operador, regras de roteamento, bases consultadas durante a chamada, continuidade de protocolo entre CAIXA e MTE e indicadores de espera/resolução específicos do benefício. `[L]` Nenhum documento público recuperado permite ligar diretamente a URA aos arquivos de pagamento descritos no contrato.

## Matriz da jornada AS-IS

| Camada | E1 — Perceber necessidade | E2 — Localizar canal | E3 — Ligar/navegar | E4 — Formular consulta |
|---|---|---|---|---|
| **Evidências Físicas** | `[F]` Requerimento do SD/CPF; CTPS Digital pode exibir acompanhamento; CAIXA Tem pode mostrar benefício/crédito quando aplicável. `[I]` O trabalhador pode confrontar esses registros com uma dúvida. citeturn946820view7turn150084search6 | `[F]` FAQ CAIXA, 0800 726 0207; 158/MTE; gov.br e CTPS Digital. citeturn150084search0turn946820view6 | `[F]` número discado e atendimento eletrônico; `[L]` sequência de menus e mensagens específicas do SD. citeturn150084search3 | `[L]` não foi localizada relação pública dos dados exigidos pela URA para identificar o beneficiário. |
| **Ações do Cidadão** | `[I, média]` percebe divergência, atraso, dúvida de valor/status/bloqueio ou quer confirmar parcela. | `[I, média]` escolhe entre CAIXA, MTE ou canal digital; não há prova de confusão generalizada. | `[F]` liga para o 0800; `[I]` tenta selecionar opção compatível. | `[I, baixa]` formula a demanda e eventualmente fornece identificadores; conteúdo exato solicitado é `[L]`. |
| **— Linha de Interação —** | | | | |
| **Frontstage** | — | `[F]` páginas oficiais expõem diferentes canais e competências. | `[F]` há atendimento eletrônico 24×7 e humano em horário delimitado; `[L]` rota interna do Seguro-Desemprego. citeturn150084search3 | `[L]` não foram recuperados scripts públicos de autenticação ou diálogo. |
| **— Linha de Visibilidade —** | | | | |
| **Backstage** | `[F]` o benefício já possui dados processados pelo sistema sob responsabilidade da Dataprev/MTE. citeturn946820view10 | `[L]` lógica que associa uma consulta web/telefone a filas ou equipes específicas. | `[L]` árvore, motor da URA e integração com bases do SD. | `[L]` telas do atendente, permissões, regras de classificação e consulta. |
| **— Linha de Interação Interna —** | | | | |
| **Processos de Suporte** | `[F]` MTE/Dataprev analisam requisitos; CAIXA opera pagamento quando parcelas são emitidas. citeturn452304view1turn452304view6 | `[F]` infraestrutura multicanal CAIXA/MTE. | `[F]` infraestrutura de teleatendimento CAIXA; fornecedor/operação específica do SD não identificados. | `[F]` dados de benefício/pagamento existem nos sistemas institucionais; `[L]` quais deles são efetivamente consultados por telefone. |

| Camada | E5 — Receber resposta | E6 — Avaliar resolução | E7 — Migrar, repetir ou encerrar |
|---|---|---|---|
| **Evidências Físicas** | `[F]` informação de parcela pode também aparecer em CTPS Digital, gov.br, CAIXA Tem/Portal Cidadão; pagamento pode chegar à conta indicada, conta CAIXA ou Poupança Social Digital. citeturn946820view7turn150084search0 | `[F]` conta/extrato, Cartão Social/Cidadão e senha são evidências da **etapa de recebimento**, não de autenticação telefônica. citeturn150084search1turn150084search2 | `[F]` 158, CTPS/gov.br, SAC, Ouvidoria e Libras são canais disponíveis segundo sua finalidade. citeturn946820view6turn150084search3turn150084search4 |
| **Ações do Cidadão** | `[I]` ouve/recebe informação automática ou humana; capacidade exata de cada opção da URA é `[L]`. | `[I]` compara a resposta com status digital, data esperada ou crédito efetivo. | `[I]` encerra se satisfeito; se não, pode repetir contato ou procurar outro canal. |
| **— Linha de Interação —** | | | |
| **Frontstage** | `[F]` 0800 é canal divulgado para consulta; `[L]` quais respostas são automáticas versus atendente. citeturn150084search0 | `[F]` para dúvidas de concessão/valor, a própria CAIXA orienta os canais MTE. citeturn150084search0 | `[F]` SAC recebe reclamações; Ouvidoria, reclamações não solucionadas. `[L]` transferência operacional direta a partir do 0800. citeturn150084search3 |
| **— Linha de Visibilidade —** | | | |
| **Backstage** | `[L]` consulta executada pela URA/operador. `[I, baixa]` algum roteamento é necessário para atendimento humano, mas sua regra não é pública. | `[F]` CAIXA processa créditos e devoluções; MTE mantém competência sobre concessão. | `[L]` eventual reaproveitamento de identificação, histórico ou protocolo entre canais. |
| **— Linha de Interação Interna —** | | | |
| **Processos de Suporte** | `[F]` lotes de parcelas são transmitidos à CAIXA; arquivos de movimento/retorno retroalimentam MTE/Dataprev. citeturn452304view1turn452304view3 | `[F]` crédito pode seguir para banco indicado, conta CAIXA, Poupança Social Digital ou canais presenciais conforme prioridade e resultado do processamento. citeturn452304view2 | `[F]` MTE mantém 158 e canais digitais; CAIXA mantém canais de reclamação e acessibilidade. |

**Fluxo textual completo.** `[I/F]` O trabalhador percebe uma necessidade → localiza um canal → se escolher o 0800 726 0207, entra no Atendimento CAIXA Cidadão → pode utilizar atendimento eletrônico a qualquer hora; se precisar de humano, este está publicamente disponível apenas nos horários informados pela CAIXA → a árvore específica do SD e o método de identificação não são públicos `[L]` → se a informação obtida for suficiente, a jornada encerra → se a questão for de concessão ou valor, a orientação oficial da CAIXA é procurar MTE/CTPS Digital/gov.br → se a dúvida for sobre crédito, a parcela pode estar sendo processada na cadeia de pagamento da CAIXA, inclusive para outro banco → se persistir reclamação referente à CAIXA, SAC e depois Ouvidoria existem como vias institucionais, mas não foi comprovada transferência direta da chamada → o cidadão também pode migrar espontaneamente para 158, CTPS Digital, gov.br, CAIXA Tem ou atendimento presencial. citeturn150084search0turn150084search3turn946820view6

A Linha de Visibilidade fica, preliminarmente, entre aquilo que o cidadão ouve/vê e as consultas/processamentos internos. A principal controvérsia é que o contrato comprova processamento de arquivos de pagamento, mas **não** comprova que esses mesmos artefatos ou sistemas estejam acessíveis à URA em tempo real.

## Bastidores, atores e sistemas

| Ator/sistema | Atividade comprovada | Relação com o atendimento | Evidência/classificação |
|---|---|---|---|
| **MTE** | Habilitação/concessão e emissão das parcelas; envio de lotes ao agente pagador. | Pode explicar por que determinadas questões não são decididas pela CAIXA. | `[F]` Res. 957 e Contrato 07/2026. citeturn452304view1turn452304view6 |
| **Dataprev** | Sistema que analisa requisitos e verifica dados online; recebe arquivos de movimento de pagamentos conforme contrato. | Suporte ao processamento; uso direto pela URA não demonstrado. | `[F]` função sistêmica; `[L]` integração URA. citeturn946820view10turn452304view3 |
| **CAIXA** | Agente pagador; valida dados, processa créditos, devoluções e canais residuais. | Detém informações da etapa de pagamento e oferece o 0800 de consulta. | `[F]`. citeturn452304view2turn150084search0 |
| **0800 726 0207** | Canal CAIXA Cidadão, eletrônico e humano. | Frontstage telefônico investigado. | `[F]` existência/horário; `[L]` menus, autenticação, telas e bases. citeturn150084search3 |
| **CTPS Digital/gov.br** | Requerimento/acompanhamento; exibição de valor, parcelas e datas. | Alternativa/redirecionamento para assuntos sob MTE. | `[F]`. citeturn946820view7 |
| **CAIXA Tem/Poupança Social Digital** | Consulta/movimentação de benefício quando creditado em conta digital CAIXA. | Evidência posterior à chamada e possível destino do crédito. | `[F]`; notificação proativa de decisões do MTE pelo CAIXA Tem: `[L]`. citeturn150084search1turn150084search6 |

O bastidor de pagamento é mais detalhado do que a v1 registrava. `[F]` Após habilitação, parcelas são emitidas pelo sistema do contratante e enviadas à CAIXA por transmissão de dados; arquivos semanais também transportam dados cadastrais para eventual abertura de Poupança Social Digital. A CAIXA pode validar CPF/nome/data de nascimento e devolver inconsistências. citeturn452304view1

`[F]` No pagamento, a prioridade contratual passa por conta indicada, contas CAIXA selecionadas automaticamente, Poupança Social Digital e, residualmente, canais físicos. Se o crédito em outra instituição for rejeitado, a parcela pode seguir para conta CAIXA do beneficiário; se o início da validade cair em dia não útil, a liquidação para outra instituição ocorre no próximo dia útil. O contrato considera a parcela efetivamente paga quando creditada em conta/digital ou **enviada para crédito em outra instituição**, diferença relevante entre “paga” no processamento e dinheiro já percebido pelo cidadão. citeturn452304view2

`[F]` A CAIXA envia diariamente à Dataprev/estrutura do MTE arquivos de movimento liquidado, e o contratante devolve relatórios de processamento e registros rejeitados. A Resolução 957 também determina que pagos e não pagos sejam informados ao sistema informatizado para gestão dos lotes. `[L]` Não se encontrou prova pública de que a URA leia diretamente esses arquivos, consulte esse banco de dados em tempo real ou apresente ao operador exatamente o mesmo status. citeturn452304view3turn452304view6

O Acórdão TCU 1.621/2026 é mantido somente como **contexto de processamento**, não como fail point da URA: o material da auditoria trata de inconsistências possíveis entre marcação de pagamento e resultado efetivo do processamento, mas não demonstra nexo causal com uma chamada no 0800. citeturn946820view11

## Pontos de transferência entre canais

| Etapa | Origem → destino | Tipo | Continuidade | Evidência |
|---|---|---|---|---|
| E5–E7 | CAIXA → CTPS Digital/gov.br/MTE para concessão ou valor | **Orientação/redirecionamento** | `[L]` protocolo ou identificação compartilhados não comprovados | `[F]` CAIXA orienta esses canais. citeturn150084search0 |
| E7 | cidadão → 158/MTE | Migração espontânea ou orientação, conforme origem | Não há evidência de transferência de chamada CAIXA→158 | `[F]` 158 atende Seguro-Desemprego. citeturn946820view6 |
| E7 | 0800/CAIXA → SAC 0800 726 0101 | Escalonamento institucional possível, **não transferência comprovada** | `[L]` | `[F]` SAC recebe reclamações e informações; 24×7. citeturn150084search3 |
| E7 | SAC → Ouvidoria 0800 725 7474 | Escalonamento de reclamação não solucionada | A função sucessiva é documentada; mecanismo de protocolo não examinado | `[F]` dias úteis, 9h–18h. citeturn150084search3 |
| E2–E7 | pessoa surda → ICOM/Libras ou 0800 726 2492 | Canal acessível alternativo | Integração específica com Seguro-Desemprego/0800 726 0207: `[L]` | `[F]` Libras interpreta SAC e atendimento presencial; linha auditiva 24×7. citeturn150084search4 |

A acessibilidade, portanto, existe institucionalmente, mas não se deve extrapolar: a página de Libras explicita interpretação do **SAC**, agências, lotéricas e correspondentes; não documenta uma árvore em Libras espelhada da URA 0800 726 0207. citeturn150084search4

## Fail points

**Documentados**

| ID | Etapa | Falha/descontinuidade | Evidência e alcance | Impacto/contorno |
|---|---|---|---|---|
| **FP-D01** | E6–E7 | Informação telefônica não esclareceu, em um caso individual, por que parcela “emitida” ainda não estava disponível. | `[F]` Relato de 16/02/2026: cidadão diz ter esperado >20 min e recebido apenas orientação de consultar app; a resposta posterior da CAIXA explicou que o valor fora enviado à conta de outra instituição e, por TED, seria liquidado no primeiro dia útil. **Não comprova frequência nem falha sistêmica.** citeturn150084search5 | Esforço adicional e incerteza. O próprio caso foi esclarecido por resposta posterior da CAIXA. |
| **FP-D02** | E5–E7 | Limite institucional: questões de concessão/valor podem sair da esfera de resposta resolutiva da CAIXA. | `[F]` A FAQ CAIXA manda verificar essas dúvidas nos canais MTE. citeturn150084search0 | Exige mudança de canal; continuidade/protocolo compartilhado são `[L]`. |

O **FP-D01 é de comunicação documentada naquele episódio**, não prova defeito do sistema de pagamento. O contrato confirma precisamente a possibilidade descrita na resposta: transferência para outro banco pode ser tratada como paga no processamento e, em dia não útil, liquidada no próximo dia útil. citeturn452304view2

**Hipotéticos / candidatos a validação**

| ID | Etapa | Hipótese de falha | Base da inferência | Confiança |
|---|---|---|---|---|
| **FP-H01** | E2 | Cidadão pode não distinguir se sua dúvida pertence ao 0800 CAIXA ou ao 158/MTE. | `[I]` Os dois canais tratam de aspectos do SD, mas não há evidência de confusão prevalente. citeturn150084search0turn946820view6 | Média |
| **FP-H02** | E3/E5 | Demanda que requeira humano pode surgir fora do horário humano da CAIXA. | `[I]` CAIXA humano: seg–sex 8–21, sáb 10–16; MTE 158: seg–sáb 7–22. O efeito concreto depende do que a URA eletrônica consegue resolver — `[L]`. citeturn150084search3turn946820view6 | Média |
| **FP-H03** | E7 | Migração telefone→digital pode falhar por ausência de conta/acesso digital. | `[I]` O serviço exige conta gov.br, mas **Bronze é suficiente**; logo não existe barreira comprovada de exigência prata/ouro. citeturn946820view7 | Média quanto à dependência digital; nula para “prata/ouro obrigatório” |
| **FP-H04** | E3/E4 | Menu, autenticação ou roteamento podem não corresponder à demanda. | `[L]/[I baixa]` árvore e dados de autenticação não foram encontrados; isso é candidato, não ocorrência comprovada. | Baixa |

O antigo FP baseado apenas no TCU foi retirado: auditoria de controles/processamento sem nexo demonstrado com uma etapa telefônica não constitui, por si só, fail point da URA.

## Normativos e contratos relevantes

| Instrumento | Dispositivo | Aplicabilidade concreta |
|---|---|---|
| **Resolução CODEFAT 957/2022** | arts. 64–65 | `[F]` Define CAIXA como agente pagador e disciplina lotes, pagos/não pagos e alimentação do sistema. citeturn452304view6 |
| **Contrato MTE 07/2026** | cláusulas 1.1 e 5; TR 4.6 e 5.3 | `[F]` Operacionalização do pagamento; preço unitário **R$ 2,25/parcela**. Não há item “URA”. Atendimento ao público aparece apenas como serviço acessório possível. citeturn452304view0turn403732view1turn403732view2 |
| **Contrato 07/2026 — TR** | 5.3.3–5.3.8.19 | `[F]` Documenta arquivos/lotes, crédito, rejeições, canais e retornos; não demonstra integração direta com URA. citeturn452304view1turn452304view2turn452304view3 |
| **Resolução CODEFAT 1.043/2026** | alteração da Res. 957 | `[F]` Atualiza **quantidade de parcelas do trabalhador resgatado**, em razão da Lei 15.455/2026. Pertinência à jornada geral do trabalhador formal é limitada; não serve como evidência de funcionamento da URA. citeturn946820view9 |
| **Carta de serviço “Solicitar Seguro-Desemprego”** | etapas de solicitar, acompanhar e receber; Login Integrado | `[F]` Requerimento+CPF; acompanhamento por CTPS/gov.br; conta gov.br pode ser Bronze, Prata **ou** Ouro; define opções de recebimento. citeturn946820view7 |
| **Decreto 13.135/2026** | arts. 10, 12–13; revogação do Dec. 11.034/2022 | `[F]` Atualiza regime geral de SAC e acessibilidade. `[L/I]` Sua incidência exata sobre o **0800 CAIXA Cidadão de benefício público**, distinto do canal oficialmente chamado “SAC CAIXA”, não foi estabelecida documentalmente nesta pesquisa; portanto não se transplantam automaticamente seus requisitos para a URA analisada. citeturn452304view7 |

A auditoria estava correta ao pedir revisão do nível gov.br, mas não em sua conclusão: a página oficial, atualizada em 25/09/2026, afirma expressamente que **Bronze, Prata ou Ouro** permitem acessar o serviço. Assim, F13 é tratada por defesa/refutação evidenciada, não por incorporação da alegação. citeturn946820view7

## Lacunas e questões para a entrevista adversarial

As lacunas que mais afetam o blueprint são: `[L]` qual é a árvore atual da URA para Seguro-Desemprego; quais dados ela solicita; se existe autenticação do beneficiário e por qual mecanismo; que respostas são efetivamente automatizadas; quando e como ocorre passagem a operador; quais telas e bases o atendente consulta; se o status visto por ele deriva diretamente do processamento contratual MTE–CAIXA; e se SAC/Ouvidoria recebem protocolo ou contexto da chamada anterior.

Também permanece `[L]` se Cartão do Cidadão/Social, senha, número do requerimento ou CPF participam da identificação **telefônica**. Eles são comprovados em outras etapas: Requerimento e CPF na solicitação, e cartão/senha no recebimento residual. Transportá-los para autenticação da URA seria inferência não sustentada. citeturn946820view7turn452304view2turn150084search2

Para a Linha de Visibilidade, a questão central é se “consulta ao status” deve ser representada como Backstage da URA ou apenas como resultado suportado por sistemas externos de pagamento/benefício. A evidência atual sustenta firmemente a existência dos sistemas e arquivos, mas não sua interface com o canal telefônico. Para a Linha de Interação Interna, igualmente está documentada a troca MTE/Dataprev↔CAIXA; falta demonstrar se a central participa diretamente dela.

As notificações merecem distinção semelhante: `[F]` CTPS Digital/gov.br constituem interfaces oficiais de acompanhamento; `[F]` CAIXA Tem permite consulta/movimentação quando o benefício é liberado em conta digital; `[L]` não foi localizada prova suficiente de que o CAIXA Tem emita notificações proativas equivalentes às decisões de concessão, exigência ou recurso do MTE. citeturn946820view7turn150084search6

Por fim, a existência de atendimento humano não autoriza atribuir ao operador uma rotina conhecida. A formulação adequada para F16 é: `[L]` regras de triagem, competências de tela e roteamento do operador não localizadas; `[I, baixa]` algum mecanismo interno de direcionamento provavelmente existe para viabilizar atendimento humano, mas sua forma e capacidade resolutiva não podem ser descritas com confiança maior.

## Referências verificáveis

**[S01] CAIXA — “Perguntas Frequentes sobre o Seguro-Desemprego”.** Natureza: oficial institucional. Seções “Como consultar a liberação da parcela?”, “Fiz o requerimento...”, “Como faço para receber...”. Confirma 0800 726 0207, canais digitais, competência MTE e meios de pagamento. citeturn150084search0  
Link direto: `https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/paginas/default.aspx`

**[S02] CAIXA — “Atendimento”.** Natureza: oficial institucional. Seções “Atendimento CAIXA Cidadão”, “SAC CAIXA”, “Ouvidoria CAIXA” e atendimento para pessoa surda/com deficiência auditiva. Confirma horários e finalidades. citeturn150084search3  
Link direto: `https://www.caixa.gov.br/atendimento/Paginas/default.aspx`

**[S03] MTE/CAIXA — Contrato nº 07/2026, Processo 19965.202436/2025-28.** Natureza: oficial primária/contratual. Contrato, p. 1, cláusulas 1 e 5; Termo de Referência, itens 4.6 e 5.3.3–5.3.23. Objeto, remuneração por parcela, arquivos, pagamentos e retornos. citeturn452304view0turn452304view1turn452304view2turn452304view3  
Link direto: `https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/licitacoes-e-contratos/pca/072026completo.pdf`

**[S04] CODEFAT — Resolução nº 957, de 21/09/2022.** Natureza: oficial normativa. Arts. 64–65, além das regras de habilitação, recurso e pagamento. citeturn452304view6  
Link direto: `https://portalfat.mte.gov.br/wp-content/uploads/2022/09/Resolucao-no-957-de-21-de-setembro-de-2022.pdf`

**[S05] Governo Federal/MTE — “Solicitar o Seguro-Desemprego”.** Natureza: oficial institucional/Carta de Serviço. Última modificação exibida: 25/09/2026. Etapas “Solicitar”, “Acompanhar” e “Receber”; seção “Login Integrado”. citeturn946820view7  
Link direto: `https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego`

**[S06] MTE — “Central Alô Trabalho 158”.** Natureza: oficial institucional. Atualizada em 26/10/2026; informa Seguro-Desemprego no escopo e funcionamento seg–sáb, 7h–22h. citeturn946820view6  
Link direto: `https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2023/marco/central-alo-trabalho-158`

**[S07] CAIXA — “Atendimento em Libras por videochamada”.** Natureza: oficial institucional. ICOM, SAC/presencial, 0800 726 2492 e atendimento 24×7. citeturn150084search4  
Link direto: `https://www.caixa.gov.br/atendimento/libras/Paginas/default.aspx`

**[S08] Dataprev — “Seguro-Desemprego”.** Natureza: oficial institucional. Declara responsabilidade pelo sistema que analisa requisitos e realiza verificação online de dados. citeturn946820view10  
Link direto: `https://dataprev.gov.br/solucoes/casos-de-sucesso/seguro-desemprego`

**[S09] CODEFAT — Resoluções de 2026, Resolução nº 1.043, de 26/08/2026.** Natureza: oficial normativa. Delimita alteração à quantidade de parcelas do trabalhador resgatado. citeturn946820view9  
Link direto: `https://portalfat.trabalho.gov.br/resolucoes-2/resolucoes-por-ano/2026-2/`

**[S10] Presidência da República — Decreto nº 13.135/2026.** Natureza: oficial normativa. Arts. 10 e 12–13 sobre acessibilidade/canais do SAC; revoga o Decreto 11.034/2022. citeturn452304view7  
Link direto: `https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/decreto/d13135.htm`

**[S11] Reclame Aqui — “Atraso no pagamento da quarta parcela do seguro desemprego”, ID 240813717, 16–19/02/2026.** Natureza: relato individual de usuário com resposta pública atribuída à CAIXA. Serve apenas para demonstrar a ocorrência daquele episódio, não prevalência. citeturn150084search5  
Link direto: `https://www.reclameaqui.com.br/caixa-economica-federal/atraso-no-pagamento-da-quarta-parcela-do-seguro-desemprego_5kmdGMQOyynTWdUd/`

**[S12] CAIXA — “Cartão do Cidadão”.** Natureza: oficial institucional. Seções “O que é” e “Senha Cidadão”; comprova cartão/senha para saque de benefícios, não autenticação na URA. citeturn150084search2  
Link direto: `https://www.caixa.gov.br/servicos/cartao-cidadao/Paginas/default.aspx`

**[S13] CAIXA — “Seguro-Desemprego”.** Natureza: oficial institucional. Seções de solicitação/pagamento e CAIXA Tem. citeturn150084search6  
Link direto: `https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/paginas/default.aspx`

**Data de corte da pesquisa: 24/11/2026.**