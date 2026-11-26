# A — Meta-prompt

- **Assistente usado:** ChatGPT (assistente 1)
- **Serviço público:** Atendimento ao Seguro-Desemprego pela URA (Unidade de Resposta Audível) da Caixa Econômica Federal
- **Canal:** central telefônica "Atendimento CAIXA Cidadão" (0800 726 0207): URA e atendimento humano
- **Órgãos envolvidos:** Caixa Econômica Federal (agente pagador) e Ministério do Trabalho e Emprego (gestor do benefício)
- **Objetivo do exercício:** sustentar um Service Blueprint AS-IS (exercício 3.1), continuando o mapa de atores do exercício 2.1

---

## Meta-prompt enviado ao assistente 1

Aja como engenheiro de prompts. A partir do objetivo e do contexto abaixo, gere um prompt estruturado — com **papel, contexto, entradas, passos, formato de saída e critérios de qualidade** — para um assistente de deep research realizar uma pesquisa na web. Não faça a pesquisa agora: quero apenas o prompt, pronto para ser colado em outra conversa com Pesquisa aprofundada ativada.

**Objetivo:**
Quero um prompt que ajude a diagnosticar **como o Atendimento ao Seguro-Desemprego pela URA da Caixa opera hoje**, para depois eu montar um Service Blueprint AS-IS no modelo de G. Lynn Shostack: camadas de Evidências Físicas, Ações do Cidadão, Frontstage, Backstage e Processos de Suporte, separadas pelas linhas de interação, de visibilidade e de interação interna. A pesquisa deve começar pela **ótica do cidadão**, e não de quem opera: a jornada começa quando o trabalhador, em casa, percebe que precisa de uma informação sobre o benefício (parcela, status, bloqueio) e decide ligar, e não quando a chamada chega à central. Quero entender, etapa por etapa: (a) o que o cidadão faz e vê; (b) o que acontece nos bastidores, quem faz o quê fora da vista dele e quais sistemas e bases são consultados; (c) quais **evidências físicas** existem em cada etapa (número de telefone, mensagens gravadas, menus de voz, SMS, cartão, extrato, comprovantes, telas de aplicativo); (d) quais **normativos** regem a operação e o atendimento; e (e) quais **fail points** são conhecidos — onde o cidadão desiste, é mandado para outro canal, recebe informação incompleta ou fica sem resposta, e que "gambiarras" ele inventa para contornar as falhas. É um retrato do serviço como ele é, não uma proposta de melhoria. A pesquisa vai servir de matéria-prima para uma entrevista adversarial com outro agente de IA, em que eu decidirei as camadas, a Linha de Visibilidade e os fail points do blueprint.

**Contexto que já tenho (do mapa de atores do exercício 2.1 — confirmar, não tratar como fato definitivo):**
- O MTE gere o benefício e a Caixa é o agente pagador, pelo Contrato MTE nº 07/2026 (operacionalização dos pagamentos, vigência 2026–2031).
- A FAQ da Caixa lista o 0800 726 0207 entre os canais de consulta do Seguro-Desemprego, ao lado do app CAIXA Tem, do Portal Cidadão e da Carteira de Trabalho Digital.
- A Resolução CODEFAT nº 957/2022, art. 4º, prevê a aferição automatizada dos requisitos de habilitação com base em CNIS, eSocial e outras bases; a Dataprev processa o benefício para o MTE.
- O MTE tem canais próprios: Central 158 (Alô Trabalho), plataforma Facilita, Carteira de Trabalho Digital, SINE e Superintendências Regionais.
- Um contrato MTE–Caixa do Abono Salarial (nº 04/2023) remunera atendimentos por URA; não se sabe se existe arranjo semelhante para o Seguro-Desemprego.
- O Decreto nº 11.034/2022 (SAC) foi revogado pelo Decreto nº 13.135/2026; não se sabe se as regras de SAC se aplicam a esse canal.
- **Lacunas principais:** árvore de menus da URA, forma de identificação do cidadão, se a URA consulta parcelas automaticamente, roteamento para atendente humano, sistemas consultados pelos atendentes, operação própria ou terceirizada da central, e indicadores de fila e resolução.
- **Principal achado do 2.1 (hipótese):** o cidadão liga para a Caixa, mas parte das respostas (status, habilitação, recurso) depende do MTE — um provável fail point de "quem atende não é quem decide".

**O que o prompt gerado deve exigir do assistente de pesquisa:**
1. Organizar o resultado por **etapas da jornada na ótica do cidadão** (no mínimo cinco), e, para cada etapa, preencher as cinco camadas do blueprint, deixando claro onde passa a Linha de Visibilidade.
2. Fontes verificáveis com link direto (normativos, páginas oficiais da Caixa e do MTE, contratos, auditorias do TCU e da CGU, relatórios de ouvidoria, Reclame Aqui e notícias para os fail points), distinguindo **fato confirmado, inferência e lacuna**.
3. Uma lista de **fail points** com etapa, descrição, evidência e impacto no cidadão, separando os documentados dos hipotéticos.
4. Os **pontos de transferência** entre canais (URA → atendente, Caixa → MTE, telefone → aplicativo ou agência), distinguindo transferência real de simples orientação.
5. **Relatório enxuto:** no máximo cerca de 4.000 palavras, com tabelas compactas e sem repetir o contexto acima. As informações mais importantes devem vir primeiro.

Escreva o prompt em português.

---

## Apêndice — Prompt gerado pelo assistente 1 a partir deste meta-prompt

> Resposta do ChatGPT ao meta-prompt, colada sem alterações numa nova conversa com Pesquisa aprofundada ativada, que originou o `B_relatorio_assistente_v1.md`.

### Prompt de Pesquisa Aprofundada — Diagnóstico AS-IS do Atendimento ao Seguro-Desemprego pela URA da Caixa

#### 1. Papel

Atue como pesquisador sênior especializado em Service Design, serviços públicos digitais, operações de atendimento multicanal e políticas públicas de trabalho e renda no Brasil.

Sua tarefa é realizar uma pesquisa documental aprofundada na web, orientada pela experiência do cidadão, utilizando o modelo de Service Blueprint de G. Lynn Shostack como referencial analítico.

Adote uma postura investigativa, crítica e baseada em evidências. Não presuma que o funcionamento formalmente previsto de um serviço corresponde necessariamente ao seu funcionamento real.

#### 2. Objetivo e contexto

Investigue como o Atendimento ao Seguro-Desemprego pela Unidade de Resposta Audível (URA) da Caixa Econômica Federal opera atualmente, produzindo um diagnóstico AS-IS que sirva de matéria-prima para a construção posterior de um Service Blueprint com cinco camadas:

- Evidências Físicas;
- Ações do Cidadão;
- Frontstage;
- Backstage;
- Processos de Suporte.

Considere as três linhas de separação:

- Linha de Interação;
- Linha de Visibilidade;
- Linha de Interação Interna.

**A unidade de análise é a jornada do cidadão, e não o fluxo operacional da instituição.**

A jornada começa quando o trabalhador, ainda em casa, percebe que precisa de uma informação sobre seu Seguro-Desemprego — como data de pagamento, situação de uma parcela, status do benefício ou motivo de bloqueio — e busca uma forma de obter essa informação por telefone.

Não comece a jornada na entrada da chamada na central. Investigue também os momentos anteriores ao contato e os desdobramentos posteriores, inclusive quando o cidadão precisa recorrer a outros canais.

O objetivo é compreender o serviço como ele existe hoje, incluindo suas limitações, fragmentações, contradições e falhas.

Não proponha melhorias, não desenhe um cenário TO-BE e não idealize o funcionamento do atendimento.

O relatório será utilizado posteriormente em uma entrevista adversarial com outro agente de IA, na qual o pesquisador humano decidirá a composição definitiva das camadas, a posição da Linha de Visibilidade e a identificação dos fail points. Portanto, apresente classificações fundamentadas, mas não trate decisões interpretativas como conclusões definitivas.

#### 3. Entradas: conhecimento prévio e hipóteses

Utilize os seguintes elementos, provenientes de um exercício anterior de mapeamento de atores, exclusivamente como pistas de investigação. Confirme, corrija ou refute cada um deles mediante fontes verificáveis:

- O Ministério do Trabalho e Emprego (MTE) gere o benefício, enquanto a Caixa atua como agente pagador, possivelmente nos termos do Contrato MTE nº 07/2026, relativo à operacionalização dos pagamentos, com vigência indicada de 2026 a 2031.
- A FAQ da Caixa apresenta o telefone 0800 726 0207 como canal de consulta do Seguro-Desemprego, ao lado do CAIXA Tem, do Portal Cidadão e da Carteira de Trabalho Digital.
- A Resolução CODEFAT nº 957/2022, especialmente seu art. 4º, prevê a aferição automatizada dos requisitos de habilitação mediante consulta a bases governamentais, como CNIS e eSocial.
- A Dataprev realiza atividades de processamento do benefício para o MTE.
- O MTE dispõe de canais próprios de atendimento, como Central 158 (Alô Trabalho), plataforma Facilita, Carteira de Trabalho Digital, SINE e Superintendências Regionais.
- O Contrato MTE–Caixa nº 04/2023, referente ao Abono Salarial, prevê remuneração de atendimentos por URA. Investigue se existe arranjo contratual equivalente para o Seguro-Desemprego.
- Há indicação de que o Decreto nº 11.034/2022, relativo ao SAC, foi revogado pelo Decreto nº 13.135/2026. Verifique a existência, vigência, alcance e aplicabilidade desses normativos ao canal investigado.

##### Hipótese central

O cidadão procura a Caixa para obter informações sobre o Seguro-Desemprego, mas determinadas respostas ou decisões relacionadas à habilitação, ao status do benefício, aos bloqueios e aos recursos administrativos podem depender do MTE.

Essa divisão de competências pode produzir um fail point estrutural: **quem atende não é necessariamente quem decide ou resolve.**

Investigue essa hipótese buscando evidências favoráveis e contrárias. Diferencie responsabilidade institucional, capacidade de consultar informações, competência decisória e capacidade efetiva de resolver a demanda.

##### Lacunas prioritárias

Investigue especialmente:

- Árvore de menus e submenus da URA.
- Mensagens gravadas e opções disponibilizadas.
- Forma de identificação e autenticação do cidadão.
- Possibilidade de consulta automatizada de parcelas, pagamentos e status.
- Existência e condições de encaminhamento para atendente humano.
- Sistemas, interfaces e bases de dados consultados pela URA e pelos atendentes.
- Integrações entre Caixa, MTE e Dataprev.
- Operação própria ou terceirizada da central.
- Contratação, remuneração e fiscalização dos atendimentos.
- Indicadores de espera, abandono, resolução e reincidência de contatos.

A ausência de documentação pública sobre qualquer desses elementos deve ser registrada como resultado da pesquisa, e não preenchida com suposições apresentadas como fatos.

#### 4. Procedimentos de pesquisa

##### Passo 1 — Delimitar o serviço e suas responsabilidades

Identifique o canal telefônico efetivamente disponibilizado pela Caixa para consultas sobre o Seguro-Desemprego na data da pesquisa.

Verifique:

- Número telefônico, finalidade, abrangência e horários.
- Serviços e informações oferecidos.
- Limites de atuação da Caixa.
- Responsabilidades do MTE, da Dataprev e de eventuais prestadores de serviço.
- Diferenças entre atendimento sobre pagamento, habilitação, concessão, bloqueio e recurso.

Não confunda o atendimento ao Seguro-Desemprego com serviços de Abono Salarial, FGTS, benefícios sociais ou atendimento bancário convencional, ainda que compartilhem infraestrutura ou canais.

##### Passo 2 — Reconstruir a jornada pela perspectiva do cidadão

Organize a jornada em pelo menos cinco etapas cronológicas, nomeadas preferencialmente com verbos que expressem ações do trabalhador.

Considere, como estrutura inicial sujeita a revisão pelas evidências:

1. Perceber a necessidade de informação sobre o benefício.
2. Procurar e identificar um canal de atendimento.
3. Ligar e navegar pelas opções da URA.
4. Identificar-se e solicitar a informação desejada.
5. Receber uma resposta automatizada ou buscar atendimento humano.
6. Interpretar a resposta e avaliar se a demanda foi resolvida.
7. Buscar outro canal, repetir o contato, desistir ou encerrar a jornada.

Não force a jornada a seguir uma sequência linear. Identifique ramificações, retornos, repetições e caminhos alternativos.

Investigue separadamente, quando houver diferenças relevantes, três situações de demanda:

- Consulta de parcela ou pagamento.
- Consulta de status ou habilitação.
- Investigação de bloqueio, impedimento ou necessidade de recurso.

Essas situações são recortes analíticos, não fluxos operacionais previamente confirmados.

##### Passo 3 — Preencher as cinco camadas do Service Blueprint

Para cada etapa da jornada, investigue e descreva:

**Evidências Físicas:** elementos tangíveis, digitais ou sensoriais percebidos pelo cidadão, como número telefônico, página de consulta, mensagens gravadas, menus de voz, mensagens de espera, protocolos, SMS, telas de aplicativos, cartões, extratos e comprovantes.

Diferencie evidências efetivamente produzidas ou utilizadas naquela etapa de elementos apenas disponíveis em outros canais.

**Ações do Cidadão:** o que o trabalhador faz para obter a informação, incluindo decisões, tentativas, fornecimento de dados, interpretação de mensagens, repetição de contatos e busca de alternativas.

**Frontstage:** ações e interações do serviço diretamente percebidas pelo cidadão, incluindo respostas automatizadas da URA, solicitações de identificação, mensagens de voz, atendimento humano e orientações recebidas.

**Backstage:** atividades diretamente relacionadas ao atendimento, mas não percebidas pelo cidadão, como processamento da solicitação, consultas a sistemas, recuperação de informações, regras de roteamento e ações internas dos atendentes.

**Processos de Suporte:** infraestrutura, sistemas, bases de dados, integrações institucionais, processamento do benefício, contratos, governança, manutenção tecnológica e demais atividades que sustentam a prestação do serviço.

Para cada etapa:

- Identifique os atores responsáveis pelas atividades.
- Diferencie a interface percebida pelo cidadão do mecanismo que a sustenta.
- Indique onde se situam as três linhas do blueprint.
- Justifique especialmente a posição sugerida da Linha de Visibilidade.
- Registre classificações ambíguas ou alternativas plausíveis.

Não classifique automaticamente toda atividade da Caixa como Frontstage ou toda atividade do MTE e da Dataprev como Backstage ou Suporte. A classificação deve considerar a natureza da atividade, sua relação com o atendimento e sua visibilidade para o cidadão.

Também não confunda as bases utilizadas na habilitação do benefício com os sistemas efetivamente consultados durante o atendimento telefônico. Uma integração existente no processamento do benefício não comprova sua utilização direta pela URA.

##### Passo 4 — Investigar os bastidores operacionais e tecnológicos

Busque documentos que permitam reconstruir o funcionamento interno do atendimento.

Investigue, quando houver evidências:

- Como a URA recebe e processa solicitações.
- Quais informações são solicitadas ao cidadão.
- Como ocorre a identificação do beneficiário.
- Quais informações podem ser recuperadas automaticamente.
- Quais sistemas disponibilizam informações aos atendentes humanos.
- Quem produz, atualiza, armazena e disponibiliza essas informações.
- Quais atividades dependem de integrações entre instituições.
- Quem possui competência para alterar informações, desbloquear situações ou decidir recursos.
- Como são organizadas, contratadas e fiscalizadas as operações da central.

Diferencie explicitamente:

- Sistemas comprovadamente utilizados no atendimento.
- Sistemas utilizados no processamento geral do benefício.
- Sistemas cuja utilização no atendimento é apenas inferida.
- Sistemas ou integrações não identificados.

Não invente nomes de sistemas, APIs, árvores de menus, scripts, procedimentos de autenticação ou fluxos internos.

##### Passo 5 — Investigar os normativos e instrumentos contratuais

Identifique a legislação, os regulamentos e os instrumentos contratuais que disciplinam o benefício e sua operação de atendimento.

Priorize:

- Legislação do Seguro-Desemprego.
- Resoluções do CODEFAT.
- Contratos, termos de referência e instrumentos celebrados entre MTE, Caixa e Dataprev.
- Normativos relativos ao atendimento ao usuário de serviços públicos.
- Regulamentação de SAC, quando efetivamente aplicável.
- Regras de acessibilidade, proteção de dados e identificação do cidadão, quando pertinentes ao canal.

Para cada instrumento relevante, informe número, data, vigência, dispositivo pertinente, link direto e consequência concreta para o serviço investigado.

Diferencie obrigações normativas, previsões contratuais e práticas operacionais comprovadas.

Não extrapole cláusulas de contratos relativos a outros benefícios para o Seguro-Desemprego. Utilize-os apenas como evidência comparativa ou pista investigativa.

##### Passo 6 — Mapear as transferências e descontinuidades entre canais

Identifique os pontos em que a jornada pode passar por diferentes canais ou instituições, incluindo:

- URA para atendente humano.
- Caixa para MTE.
- Caixa para Central 158.
- Telefone para aplicativo ou portal.
- Telefone para agência da Caixa.
- Telefone para SINE ou unidade de atendimento do MTE.

Classifique cada ocorrência como:

- **Transferência efetiva:** o atendimento é encaminhado operacionalmente a outro atendente, setor ou canal.
- **Orientação ou redirecionamento:** o cidadão recebe instruções para procurar outro canal por conta própria.
- **Migração espontânea:** o cidadão decide buscar outro canal sem encaminhamento institucional comprovado.

Investigue se existe continuidade do atendimento, compartilhamento de dados, reaproveitamento de identificação ou protocolo e necessidade de repetir informações.

Não represente uma simples orientação como transferência operacional integrada.

##### Passo 7 — Identificar fail points e estratégias de contorno

Investigue situações em que a jornada falha, é interrompida ou exige esforço adicional do cidadão.

Considere como categorias investigativas:

- Dificuldade para localizar o canal correto.
- Menus confusos ou incompatíveis com a demanda.
- Problemas de identificação.
- Ausência de opção adequada na URA.
- Dificuldade de acesso a atendente humano.
- Espera excessiva ou abandono.
- Informações incompletas, genéricas, divergentes ou desatualizadas.
- Ausência de competência do atendente para resolver a demanda.
- Redirecionamentos sucessivos entre instituições.
- Necessidade de repetir informações em diferentes canais.
- Encerramento do atendimento sem resolução.

Investigue também as estratégias informais de contorno — as chamadas “gambiarras” — efetivamente utilizadas pelos cidadãos para conseguir informações ou resolver suas demandas.

Não invente comportamentos. Diferencie estratégias documentadas em relatos de usuários de estratégias apenas hipotéticas.

Para cada fail point, identifique a etapa, a descrição da falha, a evidência disponível, o impacto no cidadão, os atores envolvidos e eventuais estratégias de contorno.

Diferencie ocorrência documentada de frequência comprovada. Um relato individual pode demonstrar a existência de uma experiência, mas não sua prevalência no conjunto dos atendimentos.

##### Passo 8 — Validar e triangular as evidências

Priorize as seguintes fontes:

1. Legislação e atos normativos oficiais.
2. Páginas, FAQs, manuais e orientações oficiais da Caixa, do MTE e da Dataprev.
3. Contratos, termos de referência, editais e documentos de fiscalização.
4. Auditorias, acórdãos e relatórios do TCU e da CGU.
5. Relatórios de ouvidoria, transparência e avaliação de serviços públicos.
6. Notícias e reportagens de veículos confiáveis.
7. Reclame Aqui e outros relatos públicos de cidadãos.

Pesquise também em repositórios oficiais, como PNCP, Diário Oficial da União, Portal da Transparência e portais institucionais.

Utilize relatos de cidadãos especialmente para investigar a experiência real, os fail points e as estratégias de contorno, sem atribuir a essas fontes autoridade para comprovar arquiteturas tecnológicas ou procedimentos internos.

Verifique a data, a vigência, a pertinência e a abrangência das fontes. Quando houver divergência entre o funcionamento formal e a experiência relatada, apresente ambos.

#### 5. Classificação obrigatória das informações

Utilize os seguintes marcadores em todas as tabelas e afirmações substantivas:

- **[F] Fato confirmado:** informação sustentada diretamente por evidência verificável, respeitando o alcance da fonte.
- **[I] Inferência:** interpretação fundamentada em evidências indiretas, acompanhada de justificativa e indicação das fontes utilizadas.
- **[L] Lacuna:** informação não localizada, insuficientemente documentada ou impossível de confirmar mediante pesquisa pública.

Quando uma fonte confirmar apenas a existência de uma previsão normativa ou contratual, não a utilize como comprovação automática de execução operacional.

Quando um relato confirmar uma experiência individual, não o utilize como comprovação de comportamento generalizado do serviço.

Para inferências relevantes, indique o grau de confiança — alto, médio ou baixo — e explique brevemente o motivo.

#### 6. Formato de saída

Produza um relatório em português, com aproximadamente 4.000 palavras no máximo, incluindo tabelas e referências. Apresente as informações mais importantes primeiro.

Organize o relatório na seguinte estrutura:

##### 6.1. Síntese executiva

Em até 250 palavras, apresente:

- Como o atendimento funciona segundo as evidências disponíveis.
- Principais limites da atuação da Caixa.
- Resultado da investigação da hipótese “quem atende não é quem decide”.
- Fail points mais relevantes.
- Principais lacunas que impedem uma reconstrução completa do serviço.

##### 6.2. Matriz da jornada AS-IS

Apresente uma matriz preliminar de Service Blueprint, com as etapas da jornada nas colunas e as camadas nas linhas.

Utilize a seguinte estrutura:

| Camada | Etapa 1 | Etapa 2 | ... | Etapa N |
|---|---|---|---|---|
| Evidências Físicas | | | | |
| Ações do Cidadão | | | | |
| — Linha de Interação — | | | | |
| Frontstage | | | | |
| — Linha de Visibilidade — | | | | |
| Backstage | | | | |
| — Linha de Interação Interna — | | | | |
| Processos de Suporte | | | | |

Preencha as células com descrições concisas, atores responsáveis, marcadores [F], [I] ou [L] e identificadores das fontes.

Caso a matriz fique excessivamente larga, divida-a em blocos de etapas consecutivas, preservando a ordem cronológica e as cinco camadas.

Após a matriz, apresente apenas as justificativas necessárias para compreender as classificações mais relevantes ou controversas, especialmente aquelas relacionadas à Linha de Visibilidade.

##### 6.3. Bastidores, atores e sistemas

| Ator ou sistema | Atividade | Relação com o atendimento | Evidência e classificação |
|---|---|---|---|

Destaque as diferenças entre consultar informações, processar o benefício, decidir sobre sua concessão e resolver demandas do cidadão.

##### 6.4. Pontos de transferência entre canais

| Etapa | Origem → Destino | Tipo de transferência | Continuidade do atendimento | Evidência |
|---|---|---|---|---|

##### 6.5. Fail points

Apresente duas tabelas separadas: uma para fail points documentados e outra para fail points hipotéticos.

| ID | Etapa | Descrição da falha | Evidência | Impacto no cidadão | Estratégia de contorno |
|---|---|---|---|---|---|

Utilize identificadores como FP-01, FP-02 e assim sucessivamente, permitindo a referência posterior durante a construção do blueprint.

Quando não houver evidência de uma estratégia de contorno, registre a lacuna.

##### 6.6. Normativos e contratos relevantes

| Instrumento | Dispositivo ou cláusula | Vigência e aplicabilidade | Implicação para o atendimento | Fonte |
|---|---|---|---|---|

Inclua apenas instrumentos com relevância concreta para o diagnóstico.

##### 6.7. Lacunas e questões para a entrevista adversarial

Apresente as principais questões ainda não resolvidas pela pesquisa, priorizadas de acordo com seu impacto na construção do Service Blueprint.

Inclua questões relacionadas a:

- Delimitação das etapas da jornada.
- Classificação de atividades nas cinco camadas.
- Posicionamento da Linha de Visibilidade.
- Distinção entre Backstage e Processos de Suporte.
- Identificação e validação de fail points.
- Responsabilidade institucional e capacidade efetiva de resolução.

Formule questões que permitam ao pesquisador humano contestar as classificações propostas. Não antecipe respostas definitivas quando as evidências forem insuficientes.

##### 6.8. Referências verificáveis

Identifique as fontes por códigos, como [S01], [S02] e [S03], utilizados ao longo do relatório.

Para cada fonte, apresente:

- Instituição ou autoria.
- Título do documento ou página.
- Data de publicação ou atualização, quando disponível.
- Página, artigo, cláusula ou seção relevante, quando aplicável.
- Link direto para a fonte original.

Registre a data de corte da pesquisa.

#### 7. Critérios de qualidade e restrições

Antes de entregar o relatório, verifique se ele atende integralmente aos seguintes critérios:

- **Centralidade no cidadão:** a jornada começa antes da ligação e contempla os desdobramentos posteriores ao atendimento.
- **Fidelidade ao AS-IS:** o relatório descreve o serviço existente, sem propor melhorias ou idealizar procedimentos.
- **Completude estrutural:** existem pelo menos cinco etapas, cinco camadas e três linhas de separação.
- **Rastreabilidade:** toda afirmação factual relevante está associada a uma fonte verificável.
- **Rigor epistemológico:** fatos, inferências e lacunas estão claramente diferenciados.
- **Precisão institucional:** as competências da Caixa, do MTE, da Dataprev e de outros atores não são confundidas.
- **Precisão operacional:** transferências reais não são confundidas com simples orientações.
- **Precisão tecnológica:** sistemas de processamento do benefício não são automaticamente considerados sistemas de atendimento.
- **Validade temporal:** contratos, normativos e informações sobre canais têm sua vigência ou atualidade verificadas.
- **Representatividade:** relatos individuais não são generalizados sem evidências adicionais.
- **Utilidade analítica:** as informações permitem reconstruir e contestar posteriormente as camadas, as linhas e os fail points do blueprint.
- **Concisão:** o relatório respeita o limite aproximado de 4.000 palavras, utiliza tabelas compactas e evita repetir o contexto inicial.

Não invente informações para preencher células vazias. Não transforme ausência de evidência em evidência de inexistência. Não apresente analogias com outros serviços como comprovação do funcionamento deste canal.

Quando a documentação pública não permitir reconstruir determinada atividade, registre o que foi pesquisado, o que foi encontrado e o que permanece desconhecido.

**O resultado esperado não é um blueprint definitivo, mas uma base de evidências organizada segundo a lógica de um Service Blueprint AS-IS, suficientemente rastreável para ser submetida a questionamento, contestação e validação posterior pelo pesquisador humano.**

Realize a pesquisa na web e entregue o relatório conforme a estrutura estabelecida.