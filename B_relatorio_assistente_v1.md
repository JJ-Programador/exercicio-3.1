Diagnóstico AS-IS do atendimento ao Seguro-Desemprego pela URA da CAIXA
Data de corte: 24/11/2026. Escopo: nacional. Público: solicitantes e beneficiários do Seguro-Desemprego. O relatório segue os requisitos do arquivo de pesquisa fornecido pelo usuário, cuja orientação central é reconstruir a jornada do cidadão — e não apenas o fluxo interno da instituição — segundo as cinco camadas do Service Blueprint e três linhas de separação. 

Há uma colisão terminológica entre os marcadores pedidos para classificação epistemológica e os marcadores pedidos para tipo de fonte. Para preservar ambos, este relatório usa [F] = fato confirmado, [I] = inferência, [L] = lacuna, conforme o arquivo; nas referências, acrescenta-se o sufixo -F para fonte oficial/primária, -I para informe/indústria e -L para relato, controle, legislativo ou usuário.

Síntese executiva
[F] O canal telefônico da CAIXA explicitamente divulgado para consultas de Seguro-Desemprego é o Atendimento CAIXA Cidadão, 0800 726 0207. A CAIXA informa atendimento eletrônico 24 horas por dia, sete dias por semana, e atendimento humano de segunda a sexta, das 8h às 21h, e aos sábados, das 10h às 16h. A mesma instituição inclui o telefone entre os canais para acompanhar a situação de parcelas do Seguro-Desemprego. 

[F] A arquitetura institucional é fragmentada por desenho: o MTE é o gestor do programa e decide sobre habilitação, valor, suspensão, cancelamento e recurso; a Dataprev mantém o sistema que processa/análise elegibilidade e cruza dados; e a CAIXA atua como agente pagador. A Resolução CODEFAT nº 957/2022, já com alterações vigentes em 2026, atribui ao sistema do Seguro-Desemprego a aferição automatizada de requisitos com bases como CNIS, GFIP e eSocial e prevê recurso administrativo dirigido ao MTE quando houver impedimento à habilitação. 

[F] O Contrato MTE nº 07/2026 confirma a contratação da CAIXA para operacionalização dos pagamentos, com vigência de 16/04/2026 a 16/04/2031 e valor estimado de R$ 383,3 milhões. Entretanto, não foi localizada, na documentação pública recuperada, a íntegra contratual ou cláusula de 2026 que demonstre se a URA é item tarifável específico desse contrato. Há, porém, evidência comparativa robusta de que contratos anteriores do Seguro-Desemprego e o Contrato nº 04/2023 do Abono Salarial tratavam atendimento por URA como serviço remunerado e auditável por quantidade de ligações. 

[I, confiança alta] A hipótese “quem atende não é necessariamente quem decide” é confirmada como característica estrutural, mas com uma distinção importante: a CAIXA pode efetivamente resolver questões de pagamento sob sua esfera, enquanto questões de concessão, valor, impedimento, suspensão/cancelamento e recurso pertencem ao MTE e ao sistema de processamento operado pela Dataprev. Portanto, o fail point não é a mera existência de competências separadas, e sim a ocorrência de uma demanda que chega à CAIXA mas depende de decisão ou correção fora de sua competência. 

[L] Permanecem não documentados publicamente, até a data de corte: árvore completa da URA do 0800 726 0207 para Seguro-Desemprego, prompts, sequência de autenticação, sistemas consultados pela URA, telas usadas por atendentes, regras de roteamento, existência de transferência técnica CAIXA→MTE, taxa de resolução, espera, abandono e reincidência específicas do Seguro-Desemprego.

Matriz da jornada AS-IS
A jornada foi dividida em sete etapas, coerentes com a orientação do arquivo e com as evidências observadas: perceber, procurar, ligar, identificar-se/consultar, receber resposta ou atendimento humano, avaliar resolução, migrar/repetir/encerrar. 

Bloco inicial da jornada
Camada	Perceber a necessidade	Procurar canal	Ligar e navegar
Evidências Físicas	[F] Data prevista, status ou ausência de crédito visível em CTPS Digital, CAIXA Tem, Portal Cidadão ou extrato [S01-F][S05-F]	[F] Página da CAIXA mostra 0800 726 0207; MTE mostra 158 e canais digitais [S01-F][S10-F]	[F] Número 0800 726 0207; mensagem eletrônica da central. [L] árvore/prompts não publicados
Ações do Cidadão	[F] Percebe parcela não liberada, status pendente, bloqueio ou dúvida	[F] Busca CAIXA, MTE, Gov.br ou telefone; pode encontrar mais de um canal	[F] Disca 0800; [L] opções exatas digitadas ou faladas
— Linha de Interação —	Entre cidadão e evidências públicas	Entre cidadão e páginas/canais	Entre cidadão e URA
Frontstage	[F] Interfaces exibem status, valor ou data quando disponíveis	[F] CAIXA e MTE apresentam canais distintos	[F] URA responde eletronicamente; atendimento humano também existe no canal geral [S02-F]
— Linha de Visibilidade —	Tudo acima é percebido pelo usuário	Idem	Voz da URA e eventual atendente ficam acima da linha; roteamento fica abaixo
Backstage	[I, alta] informação deriva de processamento prévio do benefício/pagamento	[I, média] governança de conteúdo define qual canal é divulgado	[L] regras específicas de roteamento, identificação e consulta do Seguro-Desemprego
— Linha de Interação Interna —	separa tratamento da demanda de infraestrutura	idem	separa URA/operação dos sistemas e contratos
Processos de Suporte	[F] Sistema Seguro-Desemprego/Dataprev; bases CNIS/eSocial etc. [S04-F][S06-F]	[F] portais CAIXA, Gov.br, CTPS Digital e central 158	[F] infraestrutura de telesserviço CAIXA; [L] fornecedor/terceirização específica

Bloco de consulta, resposta e pós-atendimento
Camada	Identificar-se e consultar	Receber resposta	Avaliar resolução	Migrar, repetir ou encerrar
Evidências Físicas	[L] dados pedidos pela URA não localizados	[F] resposta eletrônica/humana; [L] conteúdo exato dos scripts	[F] crédito, status, orientação, protocolo se fornecido; [L] regra de protocolo da URA	[F] 158, CTPS Digital, Gov.br, Facilita, SINE, agência CAIXA
Ações do Cidadão	[L] sequência de CPF/NIS/senha não comprovada	[F] escuta orientação ou informação	[F] confronta resposta com problema concreto	[F] recorre a MTE/CAIXA/outro canal ou encerra
— Linha de Interação —	Cidadão ↔ URA/atendente	Cidadão ↔ serviço	Cidadão ↔ resultado percebido	Cidadão ↔ novo canal
Frontstage	[L] autenticação específica; [F] pode haver atendente humano no CAIXA Cidadão	[F] CAIXA informa pagamento; MTE informa habilitação/recurso conforme competência	[I, alta] orientação para MTE em assunto de concessão	[F] 158, Facilita, CTPS Digital, SINE e SRTb são canais MTE
— Linha de Visibilidade —	entradas/voz acima; consultas e decisões internas abaixo	resultado comunicado acima; origem sistêmica abaixo	efeitos percebidos acima	nova interação começa em outro canal
Backstage	[I, média] consulta a dados da CAIXA para pagamento; [L] integração da URA com sistema MTE/Dataprev	[F] CAIXA consulta/produz informação de pagamento; Dataprev processa elegibilidade	[I, alta] operador classifica demanda conforme competência	[L] compartilhamento de identificação/protocolo entre CAIXA e MTE
— Linha de Interação Interna —	separa atendimento dos sistemas corporativos	idem	idem	separa instituições/canais
Processos de Suporte	[F] bases de pagamento CAIXA; Sistema Seguro-Desemprego e Dataprev em processamento geral	[F] MTE/Dataprev/CAIXA operam partes distintas do ciclo	[F] normas de recurso atribuem decisão ao MTE	[F] CTPS Digital, Gov.br, Facilita, 158, SINE; [L] handoff técnico integrado

A posição da Linha de Visibilidade é relativamente sólida entre aquilo que o cidadão ouve/vê e aquilo que ocorre na consulta, roteamento e processamento. A principal ambiguidade é a informação produzida por sistemas externos: ela aparece ao cidadão como resposta da CAIXA, mas sua origem pode ser de processamento do MTE/Dataprev. Isso não transforma o processamento da Dataprev em Frontstage; apenas torna seu resultado visível mediado pela CAIXA. [I, confiança alta] 

Fluxo da jornada
Sim

Não

Sim

Sim

Não

Habilitação, valor, bloqueio ou recurso

Sim

Não

Cidadão percebe dúvida, atraso ou bloqueio

Procura canal

Escolhe CAIXA?

Liga 0800 726 0207

CTPS Digital / Gov.br / 158 / Facilita

URA

Demanda de pagamento?

Informação automatizada ou atendente CAIXA

Resolvido?

Encerra

Repete contato / agência / outro canal

Orientação para canal MTE

MTE / sistema Seguro-Desemprego

Exige recurso ou correção?

Gov.br / CTPS Digital / SINE / SRTb

Análise/decisão MTE



Exibir código
[F] O diagrama distingue deliberadamente redirecionamento de transferência integrada. Não foi encontrada evidência pública de que uma chamada no 0800 da CAIXA seja transferida tecnicamente à Central 158 ou de que CPF, autenticação ou protocolo sejam reaproveitados entre as centrais. 

Bastidores, atores e sistemas
Ator ou sistema	Atividade	Relação com o atendimento	Evidência e classificação
MTE	Gestão do Programa; decisão administrativa; julgamento de recurso	Define regras e resolve questões que ultrapassam pagamento	[F] Recursos são julgados pela Secretaria do Trabalho/MTE [S06-F]
CAIXA	Agente pagador; crédito, pagamento físico/digital e canais de consulta	Pode informar e resolver questões ligadas à disponibilização/pagamento	[F] Res. 957 + FAQ CAIXA + Contrato 07/2026 [S01-F][S03-F][S06-F]
Dataprev	Sistema de análise da elegibilidade; batimentos e processamento	Produz parte essencial da informação sobre habilitação, mas uso direto na URA não foi comprovado	[F] processamento geral; [L] conexão direta com URA [S04-F]
Sistema Seguro-Desemprego	Aferição automática de critérios	Origina deferimentos, impedimentos e notificações	[F] Resolução 957, art. 4º [S06-F]
CNIS	Base usada na verificação de vínculos/remuneração	Suporte à concessão; não prova consulta pela URA	[F] [S06-F]
eSocial/GFIP/FGTS	Fontes de dados de vínculo e obrigações	Suporte à habilitação	[F] [S06-F]
CTPS Digital/Gov.br	Solicitação, acompanhamento e recurso	Canal MTE alternativo ao telefone	[F] [S05-F][S11-F]
Central 158	Informações sobre Seguro-Desemprego e outros serviços do MTE	Canal telefônico competente para temas do benefício	[F] [S10-F]
Facilita/SINE/SRTb	Acertos, atendimento e recurso presencial/remoto	Resolve demandas que podem não ser tratáveis pela CAIXA	[F] [S11-F][S12-F]
URA CAIXA	Atendimento automatizado	Frontstage do 0800 726 0207	[F] existência do canal; [L] sistemas, menus e prompts

A separação fundamental é entre consultar, processar, decidir e pagar. [F] A Dataprev declara ser responsável pelo sistema que analisa se o cidadão atende aos requisitos. [F] A Resolução 957 prevê a aferição automática pelo sistema Seguro-Desemprego. [F] O TCU descreve a CAIXA como agente responsável pelo pagamento, a Dataprev como processadora dos dados e o Ministério como gestor. 

[I, confiança alta] Logo, ver o status de uma parcela na CAIXA não significa que a CAIXA detenha competência para alterar o fundamento que gerou esse status. Essa distinção é crítica para o blueprint: o dado pode aparecer no Frontstage CAIXA enquanto a causa e a governança permanecem no Backstage/Processos de Suporte de outro ator. 

Comparação dos menus e canais
Canal	O que é comprovado	O que não foi comprovado
0800 726 0207 – CAIXA Cidadão	[F] PIS, Benefícios Sociais, FGTS e Cartão Social; eletrônico 24x7; humano em horários definidos	[L] árvore específica Seguro-Desemprego; atalhos; autenticação; opções para bloqueio/recurso
158 – Alô Trabalho	[F] informa sobre Seguro-Desemprego; atendimento automatizado ou humano	[L] árvore atual completa e integração com CAIXA
CTPS Digital / Gov.br	[F] solicitação, acompanhamento e recurso	[L] equivalência exata dos status exibidos com os consultados por atendente CAIXA
Facilita	[F] atendimento/acerto de notificação do Seguro-Desemprego	[L] sincronização de histórico com URA
Agência CAIXA	[F] pagamento e orientação sobre parcela em determinadas situações	[L] acesso a sistemas decisórios do MTE

Pontos de transferência entre canais
Etapa	Origem → Destino	Tipo	Continuidade	Evidência
Pagamento não liberado/concessão	CAIXA → CTPS Digital/Gov.br	Orientação/redirecionamento	[L] sem evidência de protocolo compartilhado	[F] FAQ CAIXA manda dúvidas de concessão e valor aos canais MTE 
Dúvida geral	CAIXA → 158	Orientação presumível, não transferência técnica comprovada	[L]	[I, média], pela divisão oficial de canais
Bloqueio/recurso	CAIXA → MTE/CTPS Digital/Gov.br/SINE/SRTb	Redirecionamento	[L]	[F] competência e canais de recurso MTE 
Falha digital	CTPS/Gov.br → Facilita/SINE/SRTb	Migração ou orientação	[L]	[F] canais previstos oficialmente 
Problema de pagamento	Telefone → agência CAIXA	Orientação	[L]	[F] FAQ oficial e relatos públicos 
Telefone frustrado	CAIXA → Reclame Aqui/outro canal informal	Migração espontânea	nenhuma continuidade institucional	[F] relatos de 2026 mostram uso do Reclame Aqui após falhas telefônicas 

Não foi localizada evidência de warm transfer CAIXA→MTE. [L] Portanto, não se deve representar no blueprint uma seta de transferência operacional entre o 0800 726 0207 e o 158. A representação mais fiel é “orientar o cidadão a procurar outro canal”, salvo validação posterior por teste de ligação, documento operacional ou evidência contratual.

Fail points
Fail points documentados
ID	Etapa	Descrição	Evidência	Impacto	Contorno
FP-01	Localizar canal	Cidadão pode não identificar qual instituição resolve pagamento versus concessão	[F] coexistem 0800 CAIXA e 158/MTE com escopos sobrepostos na percepção do cidadão	escolha de canal inadequado	[F] consulta a múltiplos sites/canais
FP-02	Obter atendimento	Longa espera e encerramento de chamada relatados	[F] relato de 16/02/2026: 40 min e ligação encerrada	esforço, repetição e atraso	[F] Reclame Aqui 
FP-03	Obter informação	Usuária relatou ligar para diversos números sem conseguir informação sobre parcela “paga” não creditada	[F] relato de 15/01/2026	ansiedade e necessidade de novo canal	[F] Reclame Aqui; CAIXA respondeu posteriormente 
FP-04	Resolver problema	CAIXA não é competente para revisar concessão, valor, suspensão/cancelamento ou recurso	[F] Resolução 957 e FAQ CAIXA	cidadão precisa mudar de instituição/canal	[F] CTPS Digital, Gov.br, 158, Facilita, SINE/SRTb
FP-05	Interpretar status	“Parcela paga” pode não significar valor imediatamente disponível na conta esperada	[F] caso público de TED programada em fim de semana e caso de crédito em conta poupança CAIXA diversa da esperada	incerteza, contato adicional	[F] extrato, agência, outro canal 
FP-06	Resolver bloqueio	Inconsistência nas bases pode impedir habilitação automática e exigir recurso	[F] Res. 957 art. 4º §2º	quebra da jornada automatizada	[F] recurso ao MTE 
FP-07	Obter resposta sobre concessão	A própria FAQ CAIXA direciona atraso superior a 30 dias relacionado à concessão/valor para MTE	[F] orientação oficial	handoff manual	[F] CTPS Digital/Gov.br 
FP-08	Consistência sistêmica	Auditoria do TCU encontrou falhas de controle e inconsistências em processamento do Seguro-Desemprego	[F] auditoria; não prova falha na URA	status/decisões podem depender de dados com problemas	[L] contorno individual varia 

Os relatos FP-02, FP-03 e FP-05 demonstram existência dessas experiências, não frequência ou prevalência. Não há base para afirmar taxa de ocorrência. 

Fail points hipotéticos
ID	Etapa	Hipótese de falha	Base da hipótese	Impacto potencial	Como testar
HP-01	Navegar URA	Menu não conter opção suficientemente específica para bloqueio/recurso	[L] árvore não publicada	seleção incorreta/repetição	mystery calling sistemático
HP-02	Identificação	Repetição de CPF/NIS após migração de canal	[L] ausência de evidência de SSO/handoff	esforço e abandono	teste multicanal + logs
HP-03	Atendimento humano	Atendente CAIXA enxergar apenas dados de pagamento, sem motivo detalhado do impedimento	[I, média] separação institucional	resposta genérica	manual de atendimento/telas
HP-04	Redirecionamento	Cidadão ser enviado ao MTE sem protocolo ou contexto	[I, alta] nenhuma integração pública identificada	repetição da narrativa	observar chamadas reais
HP-05	Resposta automatizada	URA apresentar status sem explicar origem ou competência institucional	[L] prompts desconhecidos	interpretação equivocada	gravação autorizada/teste
HP-06	Sistema	Indisponibilidade de backend degradar consulta da URA	[I, baixa] possível tecnicamente; não documentado especificamente	indisponibilidade	logs/SLA/relatórios operacionais
HP-07	Governança	Base da central ficar defasada após mudança normativa	[I, baixa] risco conhecido em centrais; contrato do Abono exige atualização explícita	orientação incorreta	comparar base de conhecimento e vigência

Normativos, contratos e timeline
Instrumentos relevantes
Instrumento	Dispositivo/cláusula	Vigência/aplicabilidade	Implicação	Fonte
Lei nº 7.998/1990	Programa Seguro-Desemprego	vigente, com alterações	base legal do benefício e do FAT	[F] referência na Res. 957 e serviço Gov.br
Resolução CODEFAT nº 957/2022	arts. 4º-5º; 27-31; 64-66	vigente com alterações até 2026	aferição automática, recurso e papel do agente pagador	[F] [S06-F]
Resolução CODEFAT nº 1.043/2026	altera Res. 957	vigente desde 2026	demonstra atualização normativa recente	[F] 
Contrato MTE nº 07/2026	objeto: operacionalização de pagamentos	16/04/2026–16/04/2031	confirma papel contratual atual da CAIXA	[F] [S03-F]
Contrato nº 11/2021 MTE/CAIXA	pagamento do Seguro-Desemprego	contrato anterior	comprova precedente contratual da operação	[F] [S08-F]
Contrato MTE nº 04/2023 – Abono	atendimento URA tarifado; relatórios de ligações	2023 em diante	apenas comparativo; não prova cláusulas do SD atual	[F] [S07-F]
Contrato MTE/Dataprev nº 17/2021	cruzamentos e elegibilidade	referência histórica auditada pelo TCU	comprova relação de processamento; sucessor atual não identificado	[F]/[L] [S09-L]
Decreto nº 13.135/2026	novo regime de SAC	vigente desde 2026; revogou Decreto 11.034/2022	alcance ao serviço público Seguro-Desemprego da CAIXA é juridicamente incerto	[F] norma; [L] aplicabilidade específica
Decreto nº 11.034/2022	SAC	revogado em 2026	não é norma vigente na data de corte	[F] 

O Decreto nº 13.135/2026 entrou em vigor 20 dias após sua publicação e substituiu expressamente o Decreto nº 11.034/2022. [F] Ele disciplina SAC nas relações de consumo. [L] Não foi localizada manifestação oficial específica afirmando que o atendimento ao Seguro-Desemprego no CAIXA Cidadão constitui SAC sujeito a esse decreto. Como o objeto analisado decorre de execução de política pública e não, necessariamente, de uma relação de consumo, aplicar automaticamente suas regras ao Seguro-Desemprego seria extrapolação. 

Timeline de eventos relevantes
Data	Evento	Relevância
11/01/1990	Lei nº 7.998 institui o Programa	marco legal
2021	Contrato MTE/Dataprev nº 17/2021 e Contrato CAIXA nº 11/2021	arquitetura contratual anterior
21/09/2022	Resolução CODEFAT nº 957	consolida concessão, processamento, pagamento e recursos
2023	Contrato MTE nº 04/2023 para Abono inclui URA tarifável	evidência comparativa de governança de telesserviço
2024	TCU, Acórdão 135/2024-Plenário	documenta papéis e falhas de controle
2025	alterações à Res. 957, inclusive pescador artesanal	muda escopo de regras
16/04/2026	inicia Contrato nº 07/2026 MTE–CAIXA	contrato vigente de pagamentos
26/08/2026	Resolução CODEFAT nº 1.043 altera a 957	atualização do programa
09–13/10/2026	Decreto nº 13.135/2026 é editado/publicado	novo regime geral de SAC
24/11/2026	data de corte desta pesquisa	AS-IS deste relatório

Uma evidência contratual comparativa merece destaque. No contrato de Abono Salarial, a URA era tarifada por ligação, com relatório sintético e analítico, ligações registradas por dia e total mensal; a documentação também estabelecia que a CAIXA atenderia demandas relativas exclusivamente ao pagamento e orientaria os usuários a procurar o MTE em questões fora desse escopo. 
 [I, confiança média] O padrão é altamente compatível com a atual divisão de responsabilidades do Seguro-Desemprego, mas não pode ser transposto como cláusula vigente do Contrato nº 07/2026 sem a íntegra desse instrumento.

Lacunas e questões para a entrevista adversarial
As lacunas de maior impacto no Service Blueprint são operacionais, não normativas. [L] A pesquisa pública permite reconstruir bem quem administra, processa e paga, mas não permite reconstruir com igual precisão como uma chamada individual percorre a infraestrutura da CAIXA. Isso deve ser tratado como achado, não preenchido por analogia.

As questões prioritárias para contestação humana são:

Árvore e conteúdo da URA: qual é a sequência exata de menus do 0800 726 0207 quando o cidadão busca Seguro-Desemprego? Há opção explícita de parcela, pagamento, benefício bloqueado ou atendente? Os prompts mudam por reconhecimento do CPF?
Autenticação: quais dados a URA solicita? CPF, NIS, data de nascimento, senha, identificação positiva ou biometria de voz? Quais tentativas e fallback existem?
Fonte da informação: quando a URA informa “parcela liberada”, “paga” ou “não disponível”, consulta banco próprio da CAIXA, arquivo recebido do MTE, réplica de dados, serviço da Dataprev ou outro middleware?
Frontstage versus Backstage: uma informação de impedimento gerada pela Dataprev mas verbalizada pela URA deve ser classificada como Frontstage apenas na camada de comunicação, mantendo processamento no suporte/backstage?
Atendente humano: o operador vê somente pagamento ou também motivo de impedimento? Pode abrir ocorrência, alterar dados ou apenas orientar?
Handoff: existe transferência real para equipe especializada, ou apenas redirecionamento? Há passagem de ANI, CPF, protocolo ou contexto?
Contrato atual: o Contrato nº 07/2026 remunera URA por chamada, por atendimento, por tempo ou embute o custo na tarifa do pagamento?
Operação própria ou terceirizada: qual entidade opera infraestrutura, atendentes e plataforma de contact center? A documentação pública recuperada não permitiu atribuição segura.
Métricas: existem indicadores segregados de TMA, nível de serviço, abandono, FCR, reincidência, indisponibilidade e chamadas por motivo especificamente para Seguro-Desemprego?
Logs: quais eventos são registrados — entrada na URA, opções selecionadas, identificação, consulta, mensagem retornada, transferência, abandono — e por quanto tempo?
Linha de Visibilidade: deve-se colocar a recuperação automática do status como Backstage ou, por ser parte inseparável da resposta automatizada, subdividir a etapa em ação visível da URA e consulta invisível?
Responsabilidade: quando um status correto do MTE é comunicado de forma insuficiente pela CAIXA, o fail point é de governança de informação da CAIXA, do desenho interinstitucional ou de ambos?
FP-01: a dificuldade de localizar o canal correto é estrutural ou apenas potencial? Seria necessária pesquisa de busca/usabilidade para medir prevalência.
FP-02/03: relatos de usuários demonstram ocorrência, mas não frequência. Quais bases de ouvidoria e reclamação permitiriam dimensioná-las?
Estratégias de contorno: além de Reclame Aqui, agência e mudança para canais MTE, há uso recorrente de redes sociais, PROCON, Ouvidoria CAIXA ou Fala.BR que possa ser quantificado?
Referências verificáveis
[S01-F] CAIXA Econômica Federal. “Perguntas Frequentes — Seguro-Desemprego”. Consulta em 24/11/2026. Confirma 0800 726 0207, canais de consulta, limites para questões de concessão e pagamento. 

[S02-F] CAIXA Econômica Federal. “Telefones App — Atendimento CAIXA Cidadão”. Consulta em 24/11/2026. Confirma 0800 726 0207, atendimento eletrônico 24x7 e horários do atendimento humano. 

[S03-F] Ministério do Trabalho e Emprego. “Contratos — 2026 — Contrato nº 07/2026”. Vigência 16/04/2026–16/04/2031; processo 19965.202436/2025-28; valor estimado R$ 383.325.207,75. 

[S04-F] Dataprev. “Seguro-Desemprego”. Declara que a Dataprev é responsável pelo sistema que analisa os requisitos e faz verificação online de dados. 

[S05-F] Governo Federal/MTE. “Solicitar o Seguro-Desemprego”. Atualizado em 25/09/2026. Detalha solicitação, acompanhamento, recebimento e canais. 

[S06-F] CODEFAT/MTE. Resolução nº 957, de 21/09/2022, versão consolidada em 2026. Art. 4º: aferição automática por CNIS, FGTS, GFIP e eSocial; arts. 27–31: recursos; arts. 64–66: pagamento. 

[S07-F] MTE/CAIXA. Contrato nº 04/2023 — Abono Salarial, Projeto Básico e anexos. Evidência comparativa: URA como serviço tarifado, relatório de ligações, limite do atendimento CAIXA a demandas de pagamento e orientação ao MTE. 

[S08-F] MTE/CAIXA. 2º Termo de Apostilamento ao Contrato Administrativo nº 11/2021. Confirma objeto de operacionalização dos pagamentos do Seguro-Desemprego no contrato anterior. 

[S09-L] Tribunal de Contas da União. Acórdão 135/2024-Plenário e notícia de auditoria. Fonte de controle externo: descreve arquitetura MTE–Dataprev–CAIXA e falhas em controles/processamento. 

[S10-F] Ministério do Trabalho e Emprego. “Central Alô Trabalho 158”. Atualizado em 26/10/2026. Informa atendimento a Seguro-Desemprego, automatizado ou humano, de segunda a sábado, 7h–22h. 

[S11-F] Governo Federal/MTE. “Cadastrar recurso relativo ao Seguro-Desemprego”. Confirma recurso ao MTE via canais digitais, SINE e Superintendências. 

[S12-F] MTE. “Facilita — Plataforma de Serviços”. Confirma atendimento para acerto ou informação sobre notificação do Seguro-Desemprego. 

[S13-L] Reclame Aqui, 16/02/2026. “Atraso no pagamento do seguro desemprego e dificuldade de atendimento”. Relato individual de espera de 40 minutos e encerramento da chamada; resposta posterior da CAIXA esclareceu TED em dia útil. 

[S14-L] Reclame Aqui, 15/01/2026. “Dificuldade em obter informações sobre seguro desemprego e pagamento não creditado”. Relato individual de múltiplas tentativas telefônicas; CAIXA esclareceu que a parcela havia sido creditada em conta poupança. 

[S15-F] Ministério da Justiça e Segurança Pública / Presidência da República. Decreto nº 13.135, de 09/10/2026. Regulamenta SAC nas relações de consumo e revoga o Decreto nº 11.034/2022; aplicabilidade específica ao Seguro-Desemprego não foi confirmada. 

[S16-F] Portal FAT. Resoluções CODEFAT de 2026. Registra a Resolução nº 1.043, de 26/08/2026, que altera a Resolução nº 957/2022. 

Data de corte de todas as conclusões: 24 de novembro de 2026. O principal resultado do levantamento é assimétrico: há documentação pública suficiente para sustentar a divisão institucional entre decisão/processamento/pagamento, mas documentação insuficiente para reconstruir, sem observação direta ou acesso interno, a micro-operação da URA — menus, autenticação, consultas, roteamento, logs, indicadores e handoffs. Essa assimetria deve permanecer explícita no blueprint AS-IS e na entrevista adversarial, em vez de ser resolvida por analogia com outros benefícios.