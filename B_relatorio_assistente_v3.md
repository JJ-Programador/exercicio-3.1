# Diagnóstico AS-IS do atendimento ao Seguro-Desemprego pela URA da CAIXA — v3

**Data de corte:** 24/11/2026. **Escopo:** nacional; jornada do cidadão que busca informação por telefone sobre Seguro-Desemprego. **Método:** revisão da v1, da segunda auditoria e das correções que a auditoria registra como efetivamente presentes na v2; verificação independente em fontes oficiais e relatos públicos. A v2 integral não estava disponível como arquivo nesta execução, portanto não atribuo a ela conteúdo além do que a `audit_v2` reproduz ou confirma. A v1 e a auditoria v2, agora acessíveis, foram usadas diretamente. fileciteturn0file0 fileciteturn0file1

## Tratamento dos pontos da segunda auditoria

| ID motivador | Mudança efetiva na v3 | Seção afetada |
|---|---|---|
| **F02 / N04** | Todas as afirmações do corpo passam a usar **S01, S02...**; referências finais trazem fonte, dispositivo e URL direto. Não se usam marcadores internos como `citeturn...` como sistema de rastreabilidade do relatório. | Todas |
| **F07 / N02** | O **Acórdão 135/2024** é restaurado como fonte histórica de controles/processamento; o **Acórdão 1621/2026** é mantido como auditoria diferente, voltada à qualidade do serviço digital e integração ao eSocial. Nenhum deles é tratado como falha da URA sem nexo operacional demonstrado. | Bastidores; Fail points; Normativos |
| **F15 / N03** | Resolvida a divergência: havia **dois relatos distintos em 16/02/2026**. Um relata **40 minutos e chamada encerrada**; outro relata **mais de 20 minutos e orientação para consultar o app**. O primeiro é preservado como FP documentado; o segundo entra como evidência adicional, sem fusão dos casos. TED e crédito em outra conta são distinguidos. | Fail points |
| **N01** | Recuperados da v1: FP-03 de 15/01/2026, HP-02/03/05/06/07, Contrato 11/2021, timeline, comparação de canais e questões adversariais. Cada item foi **mantido, rebaixado ou descartado** conforme evidência atual. | Matriz; Transferências; Fail points; Normativos; Lacunas |
| **N05** | Confirmado que a página da Central 158 tem URL de 2023, mas está **atualizada em 26/10/2026** e informa seg.–sáb., 7h–22h; portanto o link não é obsoleto apenas pelo slug. A Res. 957 passa a usar a **revisão consolidada de 2026**. | Matriz; Referências |
| **N06** | O método de busca no Contrato 07/2026 é explicitado: PDF oficial de **32 páginas**, texto pesquisável, com busca por termos e leitura dos dispositivos relevantes. Não se afirma “ausência absoluta de URA” como se fosse prova ontológica; afirma-se que **não foi localizado item tarifário específico de URA** e que o preço contratual identificado é R$ 2,25 por parcela. | Bastidores; Normativos |
| **N07** | O item **4.6.1.1** é ligado à lacuna de terceirização: “atendimento ao público” pode ser subcontratado como serviço acessório; isso **não prova** que o 0800 726 0207 seja objeto dessa subcontratação. | Bastidores; Lacunas |
| **N08** | Fail points voltam a ser organizados **por etapa**, separando: ocorrência documentada, restrição estrutural confirmada e hipótese operacional. O rigor da v2 é preservado sem apagar matéria-prima útil da v1. | Fail points |

A auditoria v2 identifica N01 como consequência direta de a versão anterior ter sido reconstruída sem acesso à v1; a própria v1 confirma a existência do segundo relato, das hipóteses HP-02/03/05/06/07, do contrato de 2021 e da timeline agora restaurados. fileciteturn0file0 fileciteturn0file1

## Síntese executiva

[F] A CAIXA divulga o **0800 726 0207 — Atendimento CAIXA Cidadão** para benefícios sociais e Seguro-Desemprego. O atendimento eletrônico funciona 24x7; o humano, de segunda a sexta, 8h–21h, e aos sábados, 10h–16h. O MTE mantém o **158**, automatizado ou humano, de segunda a sábado, 7h–22h. S01, S02, S06. citeturn605260search0turn820577search2

[F] A divisão institucional continua sendo o principal determinante da jornada: o MTE gere e decide aspectos de habilitação/recurso; a Dataprev participa do processamento; a CAIXA é agente pagador. O Contrato 07/2026 remunera a operação em **R$ 2,25 por parcela**, não por ligação identificada no quadro de preços. Seu Termo de Referência permite subcontratar, como serviços acessórios, inclusive “atendimento ao público”, mas não associa essa cláusula especificamente ao 0800 726 0207. S03, S04, S07. citeturn717001view0turn363873view0turn820577search1

[I, confiança alta] A hipótese “quem atende não é necessariamente quem decide” permanece válida, mas não deve ser convertida automaticamente em falha: torna-se fail point quando uma necessidade concreta chega à CAIXA e depende de decisão ou correção sob competência de outro ator.

[F] Três relatos públicos delimitam experiências concretas: espera de 40 minutos com encerramento de chamada; espera superior a 20 minutos com orientação ao app; e parcela “paga” creditada em poupança diferente da esperada. Esses relatos comprovam ocorrência, não frequência. S09–S11. citeturn971412search2turn971412search3turn971412search4

[L] Continuam sem documentação pública suficiente: árvore do Seguro-Desemprego na URA, autenticação, telas do atendente, bases efetivamente consultadas pela chamada, roteamento, handoff CAIXA→MTE, operador efetivo da central e indicadores específicos do benefício.

## Matriz da jornada AS-IS

| Camada | Perceber necessidade | Procurar canal | Ligar/navegar | Identificar/consultar | Receber resposta | Avaliar resolução | Migrar/repetir/encerrar |
|---|---|---|---|---|---|---|---|
| **Evidências físicas** | [F] CTPS Digital, Gov.br, CAIXA Tem, extrato, data/status; requerimento do SD. S05 | [F] páginas CAIXA, 0800, 158. S01,S06 | [F] número 0800; [L] prompts/árvore | [L] dados exigidos pela URA | [F] voz automatizada/humana; [L] script | [F] crédito, extrato, status, orientação | [F] 158, CTPS, Gov.br, agência, SAC/Ouvidoria |
| **Ações do cidadão** | [I] percebe atraso, dúvida, bloqueio ou status | [I] procura canal que pareça adequado | [I] liga e seleciona opções | [L] forma exata de identificação | [I] escuta resposta ou busca atendente | [I] compara resposta com necessidade | [F/I] muda de canal; relatos mostram repetição e reclamação. S09–S11 |
| **— Linha de Interação —** | cidadão ↔ interfaces | cidadão ↔ canais | cidadão ↔ URA | cidadão ↔ URA/atendente | cidadão ↔ serviço | cidadão ↔ resultado | cidadão ↔ novo canal |
| **Frontstage** | [F] status/data visíveis em canais digitais | [F] canais divulgados por instituições diferentes | [F] URA e possibilidade de atendimento humano no CAIXA Cidadão. S02 | [L] autenticação específica | [F] CAIXA comunica informações de pagamento; MTE mantém canais para benefício/recurso | [I, média] eventual orientação conforme competência | [F] 158, SAC, Ouvidoria, agência e digital existem; [L] transferência integrada |
| **— Linha de Visibilidade —** | tudo acima é percebido | idem | voz é visível; roteamento não | entrada é visível; consulta não | resposta visível; origem sistêmica não | efeito percebido | nova interação visível |
| **Backstage** | [I, alta] informação decorre do processamento prévio | [I, média] governança institucional de canais | [L] regra de roteamento da URA | [L] bases/telas usadas pela central | [F] arquivos/lotes de pagamento são recebidos, processados e retornados; [L] elo direto com a URA. S03 | [I, baixa] operador pode classificar demanda; não há manual público | [L] compartilhamento de contexto/protocolo entre canais |
| **— Linha de Interação Interna —** | separa atendimento de infraestrutura | idem | idem | idem | idem | idem | separa instituições |
| **Processos de suporte** | [F] Sistema Seguro-Desemprego, bases e processamento normativo. S04,S07 | [F] portais e centrais | [F] infraestrutura CAIXA; [L] fornecedor específico | [F] bases de pagamento; [L] uso direto pela URA | [F] MTE/CAIXA/Dataprev participam do ciclo de processamento/pagamento | [F] normas de competência e recurso | [F] CTPS/Gov.br/158/SAC/Ouvidoria |

A documentação de 2026 aceita acesso digital ao serviço por conta gov.br **Bronze, Prata ou Ouro**; portanto não se mantém a hipótese da auditoria v1 de que prata/ouro seriam barreira obrigatória. O requerimento do Seguro-Desemprego e CPF são documentos/dados explicitamente indicados; o recebimento pode ocorrer em conta informada, poupança CAIXA, Poupança Social Digital ou, em certas condições, com Cartão Cidadão. S05. citeturn820577search6turn835097search1

[F] A acessibilidade permanece parte do AS-IS: a CAIXA oferece atendimento para pessoas surdas/com deficiência auditiva e intérprete de Libras via ICOM. [L] A página institucional não demonstra que esse recurso reproduza integralmente a árvore ou as funções específicas da URA 0800 726 0207. S12. citeturn605260search0

## Bastidores, atores e sistemas

| Ator/sistema | Atividade comprovada | Relação com a chamada |
|---|---|---|
| **MTE** | [F] gestor do serviço e contratante da operação de pagamento | Pode ser destino necessário quando a demanda ultrapassa pagamento. S03,S05 |
| **CAIXA** | [F] agente pagador; processa disponibilização e meios de pagamento | Instituição responsável pelo 0800 e por informações/questões na esfera de pagamento. S01–S03 |
| **Dataprev** | [F] participa do processamento e recebe movimentos liquidados no fluxo contratual | [L] não foi comprovada consulta direta da URA a serviços Dataprev. S03,S07 |
| **Sistema Seguro-Desemprego / eSocial / bases** | [F] suportam aferição e eventos do benefício | Processo de suporte; não se deve colocá-los automaticamente como backend da URA. S04,S08 |
| **Operação da central** | [L] prestador específico não identificado | O TR admite subcontratação de “atendimento ao público”, mas não identifica o 0800. S03 |

No PDF oficial do Contrato 07/2026, de 32 páginas, foram pesquisados termos relativos a atendimento e examinados o quadro de preços, subcontratação e rotinas de execução/pagamento. O quadro contratual fixa unidade “parcela”, 170.366.759 parcelas estimadas e preço unitário de R$ 2,25. O item 4.6.1.1 admite subcontratação de serviços acessórios, incluindo atendimento ao público. Não foi localizado item de faturamento específico denominado URA ou ligação. Isso é diferente de afirmar que não exista atendimento telefônico custeado indiretamente dentro da operação. S03. citeturn225875view0turn225875view1

[F] O bastidor do pagamento é mais bem documentado que o da central: arquivos de registros de pagamento chegam à CAIXA; há confirmação de recebimento, rejeição em caso de inconsistência, processamento e movimento diário liquidado enviado à Dataprev/SEPRT, além de retornos sintéticos/analíticos. Esses mecanismos explicam como a instituição pagadora recebe e devolve estados do pagamento, mas **não demonstram** que a URA consulte esses arquivos diretamente. S03. citeturn363873view2turn363873view3

[N07] O item 4.6.1.1 reduz a lacuna “pode haver terceirização?”: **sim, contratualmente pode haver subcontratação de atendimento ao público como atividade acessória**. Ele não resolve “quem opera o 0800 726 0207?”, porque não vincula o dispositivo à central.

## Pontos de transferência entre canais

| Etapa | Origem → destino | Classificação | Continuidade |
|---|---|---|---|
| Dúvida de pagamento | 0800 CAIXA → agência/conta/extrato | [F] orientação/migração possível | [L] protocolo compartilhado |
| Habilitação/recurso | CAIXA → CTPS/Gov.br/158/SINE/SRTE | [I, alta] redirecionamento coerente com competências; transferência técnica não comprovada | [L] |
| Telefone → digital | 0800/158 → CTPS/Gov.br | [F] canais coexistem; [L] reaproveitamento de identificação | [L] |
| Reclamação sobre CAIXA | atendimento → SAC 0800 726 0101 → Ouvidoria 0800 725 7474 | [F] instâncias institucionais existentes; [L] transferência automática | [L] |
| Atendimento frustrado | telefone → Reclame Aqui | [F] migração espontânea observada em relatos | nenhuma continuidade institucional |

A assimetria de horários da v2 é mantida como **HP-08**, não como falha comprovada: o CAIXA Cidadão humano termina às 21h nos dias úteis e às 16h no sábado, enquanto o 158 funciona até 22h de segunda a sábado. Isso cria uma condição potencial de mudança de canal, mas não comprova abandono ou dano. S02,S06. citeturn605260search0turn820577search2

Comparação sintética recuperada de N01: **0800 CAIXA** — pagamento/benefícios sociais e atendimento humano em horário divulgado; **158** — informações MTE sobre Seguro-Desemprego e outros temas trabalhistas; **CTPS/Gov.br** — solicitação/acompanhamento e serviços digitais; **agência CAIXA** — recebimento e questões de pagamento; **SAC/Ouvidoria** — reclamação/escalonamento institucional. S01,S02,S05,S06,S12.

## Fail points

**Fail points documentados ou restrições estruturais confirmadas**

| ID | Etapa | Tipo | Evidência e impacto |
|---|---|---|---|
| **FP-01** | Obter atendimento | relato documentado | Em 16/02/2026, cidadã relata **40 min de espera** e que a chamada foi encerrada; depois a CAIXA informou que a parcela prevista para sábado seguia por TED à conta indicada e seria efetivada em dia útil. Impacto: repetição/esforço. S09. citeturn971412search2 |
| **FP-02** | Receber resposta | relato documentado | Outro relato, também de 16/02, registra **mais de 20 min** e orientação para consultar o app. É um caso diferente do FP-01; não deve substituí-lo. S10. citeturn971412search3 |
| **FP-03** | Interpretar “paga” | relato documentado, recuperado N01 | Em 15/01/2026, cidadã relata que a parcela constava como paga, mas não aparecia onde esperava; a resposta informou crédito em **conta poupança CAIXA**. Impacto: incerteza e múltiplas ligações. S11. citeturn971412search4 |
| **FP-04** | Resolver habilitação/recurso | restrição estrutural | A CAIXA é agente pagador; decisões do benefício e recursos pertencem ao arranjo MTE. Uma demanda fora da competência do pagador exige mudança de canal. S03–S05 |
| **FP-05** | Interpretar parcela emitida/paga | risco documentado de comunicação | TED para outra instituição depende de dia útil; crédito pode seguir outra modalidade prevista. “Emitida/paga” não prova disponibilidade imediata na conta que o cidadão está consultando. S03,S05,S09–S11 |
| **FP-06** | Processamento | restrição documental | Arquivo inconsistente pode ser rejeitado e exigir regularização pelo contratante. É fail point do processamento de pagamento, não prova falha da URA. S03 |

[F15/N03] A evidência não autoriza afirmar que os casos de 15–16/02 decorreram de “falha sistêmica da URA”. No caso de 40 minutos, a resposta posterior mostra TED para outra instituição e regra de dia útil; no de 15/01, havia crédito em poupança CAIXA. O problema empiricamente demonstrado é a **distância entre o estado do pagamento e a informação efetivamente obtida pelo cidadão no contato**. S09,S11. citeturn971412search2turn971412search4

**Fail points hipotéticos recuperados e reavaliados**

| ID | Hipótese | Decisão N01 |
|---|---|---|
| **HP-01** | menu não cobrir bloqueio/recurso | **Manter [L]**: árvore desconhecida |
| **HP-02** | repetir CPF/NIS ao mudar de canal | **Manter [L]**: não há evidência de SSO/handoff |
| **HP-03** | atendente ver só pagamento e não causa detalhada | **Rebaixar para [I, baixa]**: divisão institucional sustenta possibilidade, mas telas não são públicas |
| **HP-04** | redirecionamento sem protocolo/contexto | **Manter [I, média]**: ausência de integração pública, sem prova de todos os casos |
| **HP-05** | URA informar status sem explicar origem | **Manter [L]**: prompts ausentes |
| **HP-06** | indisponibilidade de backend degradar URA | **Manter [I, baixa]**, explicitamente genérico; não há ocorrência específica comprovada |
| **HP-07** | base da central ficar defasada | **Manter [I, baixa]** como risco de governança, não ocorrência |
| **HP-08** | necessidade de humano fora do horário CAIXA | **Manter [I, média]** pela assimetria de horários; impacto não medido |

O antigo FP-08 da v1, baseado no TCU, permanece **descartado como fail point da URA**. O Acórdão 135/2024 registra problemas de controle/processamento do programa, e o 1621/2026 audita qualidade do serviço digital e determina integração ao eSocial; nenhum, isoladamente, demonstra que uma chamada da URA falhou. S07,S08. citeturn820577search1turn971412search0

## Normativos, contratos e linha do tempo

| Instrumento | Dispositivo | Implicação AS-IS |
|---|---|---|
| Lei 7.998/1990 | programa e agente pagador | base legal |
| Res. CODEFAT 957/2022, **revisão 2026** | concessão, processamento, pagamento, notificações e recurso | referência normativa consolidada. S04 |
| Res. 1.043/2026 | parcelas do **trabalhador resgatado** | mantida apenas para essa modalidade; não generalizada ao trabalhador formal. S13 |
| Contrato MTE–CAIXA 07/2026 | cláusulas 1 e 5; TR 4.6.1.1 e 5.3 | R$ 2,25/parcela; subcontratação acessória possível; fluxo de arquivos. S03 |
| Contrato 11/2021 | operação anterior de pagamentos | restaurado como antecedente contratual, não como prova do desenho atual. S14 |
| Acórdão 135/2024-TCU | auditoria de pagamentos/controles | contexto de governança, não fail point URA. S07 |
| Acórdão 1621/2026-TCU | serviço digital, eSocial | auditoria distinta; não substitui o 135/2024. S08 |

A correção N02 é, portanto, **não escolher um acórdão “em lugar” do outro**. O 135/2024 examinou eficiência e regularidade dos pagamentos e controles do programa no período auditado; o 1621/2026 avaliou o serviço público digital do trabalhador formal e determinou integração ao eSocial para reduzir entrada duplicada e melhorar tempestividade. São evidências de escopos diferentes. S07,S08. citeturn820577search1turn971412search0

**Timeline restaurada:** 2021 — Contrato 11/2021 CAIXA/MTE; 21/09/2022 — Res. 957; 31/01/2024 — Acórdão TCU 135/2024; 16/04/2026 — início do Contrato 07/2026; 24/06/2026 — Acórdão 1621/2026; 26/08/2026 — Res. 1.043; 25/09/2026 — atualização da carta de serviço; 26/10/2026 — atualização da página Central 158; 24/11/2026 — corte analítico. S03–S08,S13,S14. citeturn820577search0turn971412search0turn820577search2turn820577search6

## Lacunas, questões adversariais e referências

As lacunas de maior impacto continuam operacionais. [L] Não foi possível reconstruir de fonte pública: árvore completa e prompts da URA; identificação/autenticação; serviço consultado após a identificação; telas e permissões do operador; transferência técnica para 158/MTE; compartilhamento de protocolo; fornecedor que efetivamente opera o 0800; TMA, abandono, FCR ou reincidência específicos do Seguro-Desemprego.

As questões adversariais recuperadas de N01 permanecem relevantes: qual menu aparece após ligar para 0800 726 0207 e em que ponto há atendente? Quais dados são exigidos? A URA lê base própria CAIXA, arquivo de pagamento, réplica ou serviço externo? O operador vê motivo de impedimento ou apenas situação do pagamento? Há abertura de ocorrência? Existe handoff técnico ou só orientação? O “atendimento ao público” subcontratável do item 4.6.1.1 inclui contact center, e, em caso positivo, qual contrato/suboperador executa a central? Quais logs e métricas são segregados por Seguro-Desemprego? Onde deve ficar a Linha de Visibilidade quando um dado originado fora da CAIXA é apenas verbalizado pela URA? Essas perguntas devem permanecer abertas até evidência operacional.

**S01 — CAIXA. “Seguro-Desemprego — Benefícios Trabalhador”.** Papel de agente pagador, meios de recebimento, Cartão Social, CAIXA Tem e TED. [URL direta](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx). citeturn820577search3

**S02 — CAIXA. “Telefones App — Atendimento CAIXA Cidadão”.** 0800 726 0207; eletrônico 24x7; humano seg.–sex. 8h–21h e sáb. 10h–16h. [URL direta](https://www.caixa.gov.br/atendimento/telefones-app/Paginas/default.aspx). citeturn605260search0

**S03 — MTE/CAIXA. Contrato nº 07/2026 e Termo de Referência.** Cl. 1 e 5; TR 4.6.1.1; itens 5.3.8 e 5.3.18–5.3.20. [PDF direto](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/licitacoes-e-contratos/pca/072026completo.pdf). citeturn717001view0turn363873view0turn363873view2

**S04 — CODEFAT/MTE. Resolução nº 957/2022, revisão do Seguro-Desemprego publicada em 2026.** Arts. 4–8 e capítulos de processamento/pagamento. [PDF revisado](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/09/Resolucao-no-957-de-21-de-setembro-de-2022-Revisao-do-SD.pdf). citeturn605260search8

**S05 — Governo Federal/MTE. “Solicitar o Seguro-Desemprego”.** Última modificação 25/09/2026; requerimento, CPF, acompanhamento, meios de recebimento e 158. [URL direta](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego). citeturn820577search6

**S06 — MTE. “Central Alô Trabalho 158”.** Atualizada em 26/10/2026; seg.–sáb., 7h–22h. O slug contém “2023”, mas a própria página registra atualização de 2026. [URL direta](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2023/marco/central-alo-trabalho-158). citeturn820577search2

**S07 — TCU. Acórdão 135/2024-Plenário.** Auditoria sobre eficiência, regularidade e controles do Programa do Seguro-Desemprego. [URL direta](https://pesquisa.apps.tcu.gov.br/doc/acordao-completo/135/2024/Plen%C3%A1rio). citeturn820577search1

**S08 — TCU. Acórdão 1621/2026-Plenário.** Auditoria operacional do serviço digital; item 9.1 determina integração ao eSocial. [URL direta](https://pesquisa.apps.tcu.gov.br/documento/acordao-completo/%2A/NUMACORDAO%253A1621%2520ANOACORDAO%253A2026/DTRELEVANCIA%2520desc%252C%2520NUMACORDAOINT%2520desc%252C%2520COPIACOLEGIADO%2520desc/0). citeturn971412search0

**S09 — Reclame Aqui, 16/02/2026, ID 240831467.** Relato de espera de 40 minutos e encerramento; resposta CAIXA sobre TED e dia útil. [URL direta](https://www.reclameaqui.com.br/caixa-economica-federal/atraso-no-pagamento-do-seguro-desemprego-e-dificuldade-de-atendimento_Wk1HS6Uvofya2oTG/). citeturn971412search2

**S10 — Reclame Aqui, 16/02/2026, ID 240813717.** Relato distinto: mais de 20 minutos e orientação para consultar app; resposta posterior sobre TED. [URL direta](https://www.reclameaqui.com.br/caixa-economica-federal/atraso-no-pagamento-da-quarta-parcela-do-seguro-desemprego_5kmdGMQOyynTWdUd/). citeturn971412search3

**S11 — Reclame Aqui, 15/01/2026, ID 237787045.** Parcela constava paga; resposta informa crédito em poupança CAIXA. [URL direta](https://www.reclameaqui.com.br/caixa-economica-federal/dificuldade-em-obter-informacoes-sobre-seguro-desemprego-e-pagamento-nao-creditado_0qXMe5KrTixW7ql6/). citeturn971412search4

**S12 — CAIXA. “Atendimento”.** SAC 0800 726 0101, Ouvidoria 0800 725 7474 e atendimento em Libras/acessibilidade. [URL direta](https://www.caixa.gov.br/atendimento/Paginas/default.aspx). citeturn605260search2

**S13 — Portal FAT. Resolução CODEFAT/MTE nº 1.043/2026.** Altera a Res. 957 especificamente quanto à quantidade de parcelas do trabalhador resgatado. [URL direta](https://portalfat.trabalho.gov.br/resolucoes-2/resolucoes-por-ano/2026-2/). citeturn820577search4

**S14 — MTE/CAIXA. Contrato nº 11/2021.** Antecedente contratual para operacionalização dos pagamentos do Seguro-Desemprego; usado apenas como linha histórica. [PDF direto](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/licitacoes-e-contratos/contratos/pdf/11_2021.pdf). citeturn835097search6

**Data de corte das conclusões:** 24 de novembro de 2026. O resultado central permanece assimétrico: a arquitetura normativa e o processamento do pagamento são razoavelmente documentáveis; a micro-operação da URA — menus, autenticação, consulta, roteamento, operação terceirizada específica, logs e indicadores — continua sendo a principal lacuna do blueprint AS-IS.