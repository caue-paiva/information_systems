# Horizonte 360: Plataforma de Visão Única do Cliente para a Decisão de Crédito e o Atendimento no Banco Horizonte

**Universidade de São Paulo — Instituto de Ciências Matemáticas e de Computação**
**SSC0120 — Sistemas de Informação — 2026/1**

**Projeto Final**

**Integrantes:**

| Nome | NUSP |
|---|---|
| Cauê Paiva Lira | 14675416 |
| João Pedro Alves Notari Godoy | 14582076 |
| Letícia Barbosa Neves | 14588659 |
| Pedro Lucas Figueiredo Bahiense | 14675458 |

---

## Sumário

1. Introdução
   1.1 Contextualização do problema
   1.2 Motivação e justificativa
   1.3 Soluções existentes
2. Solução Proposta
   2.1 Funcionalidades
   2.2 Questões técnicas
   2.3 Questões organizacionais
   2.4 Questões humanas
   2.5 Processos de negócio
3. Processamento da Informação
   3.1 Dados de entrada
   3.2 Processamento
   3.3 Informações geradas
4. Valor Organizacional e Vantagem Competitiva
   4.1 Cadeia de valor
   4.2 Vantagem competitiva
5. Referências Bibliográficas

---

## 1. Introdução

### 1.1 Contextualização do problema

O Banco Horizonte é uma instituição financeira brasileira de médio porte que atua principalmente no ambiente digital. Fundado há cerca de oito anos, começou oferecendo uma proposta simples e pouco burocrática, composta por conta digital gratuita, cartão de débito e transferências pelo aplicativo. Com o crescimento da base de clientes e o acirramento da concorrência no setor, o portfólio se ampliou e passou a incluir cartão de crédito, empréstimos pessoais, antecipação de recebíveis para microempreendedores, investimentos de baixo risco e seguros básicos. Hoje o banco reúne aproximadamente três milhões de clientes cadastrados, dos quais cerca de metade usa a conta todos os meses. Seu público é formado por jovens adultos, trabalhadores informais, microempreendedores individuais e pequenos comerciantes que têm no aplicativo o principal canal de relacionamento com a instituição.

O crescimento acelerado, porém, não veio acompanhado de uma estrutura tecnológica integrada. Os sistemas foram sendo implantados de forma isolada, conforme cada nova necessidade surgia. O cadastro de clientes foi desenvolvido internamente nos primeiros anos. O módulo de análise de crédito foi contratado depois junto a uma empresa terceirizada. O atendimento opera sobre uma plataforma externa de CRM, e a área de risco trabalha com planilhas e relatórios manuais, separados do restante da operação. O resultado é um conjunto de silos de informação que não se comunicam de maneira confiável, exatamente o problema que a disciplina descreve como característico de uma organização sem sistemas integrados.

Diante da amplitude desse cenário, este projeto delimita o problema a um processo específico, e não à integração de todos os sistemas de uma vez. O foco está na **decisão de concessão de crédito e no atendimento às dúvidas dela decorrentes**. Quando um cliente solicita um cartão de crédito ou um empréstimo, seus dados percorrem etapas de cadastro, análise de renda, verificação de histórico interno e decisão. Como essas etapas não estão conectadas, uma informação atualizada no cadastro pode não aparecer no sistema de crédito, e o atendente que recebe a reclamação de um cliente sobre uma recusa raramente enxerga o motivo da decisão. O problema, portanto, é duplo: a decisão de crédito é lenta e inconsistente, e o atendimento não consegue explicá-la ao cliente.

Ficam **fora do escopo** deste projeto o sistema antifraude e as questões de segurança da informação, o processamento de transações do dia a dia (Pix, pagamentos, uso de cartão) e a substituição dos sistemas legados. Essas frentes continuam operando como estão e poderão ser incorporadas em fases posteriores. A escolha por um recorte estreito é deliberada, pois uma proposta que tentasse resolver todos os desafios da organização perderia profundidade e viabilidade.

### 1.2 Motivação e justificativa

A concessão de crédito é uma das principais fontes de receita de um banco e, ao mesmo tempo, um dos pontos de maior atrito com o cliente. No Banco Horizonte, a fragmentação dos sistemas gera três impactos concretos. O primeiro é a lentidão: como os dados precisam ser reunidos manualmente entre cadastro, crédito e histórico, o banco demora mais para aprovar clientes legítimos, o que representa perda direta de receita e abre espaço para que o cliente feche negócio com um concorrente. O segundo é a inconsistência: decisões tomadas com base em informação incompleta ou desatualizada resultam ora em recusas de bons clientes, ora em aprovações arriscadas. O terceiro é a opacidade no atendimento: quando o cliente pergunta pelo aplicativo por que seu crédito foi negado, o atendente consulta várias telas, abre chamados internos ou encaminha a solicitação, o que aumenta o tempo de resposta e passa a impressão de que o banco não controla os próprios processos.

Esses impactos merecem atenção porque atingem o núcleo da relação do banco com seu público. Em um setor no qual o cliente é cada vez menos fiel e migra rapidamente diante de uma falha, o atrito na aprovação de crédito e a falta de explicação clara funcionam como gatilhos de evasão. Além disso, a diretoria depende de indicadores como taxa de aprovação, inadimplência por perfil e tempo médio de atendimento para decidir, mas hoje esses números vêm de extrações manuais e cruzamento de planilhas, um processo lento e sujeito a erro que reduz a capacidade estratégica da empresa.

A solução proposta, apresentada em alto nível, é a **Horizonte 360**, uma plataforma de visão única do cliente. Ela não substitui os sistemas existentes. Em vez disso, cria uma camada de integração que reúne, em uma interface consolidada, os dados de cadastro, de crédito e de atendimento necessários para decidir e explicar uma concessão de crédito. A partir dessa base consolidada, a plataforma oferece um painel de apoio à decisão de crédito, uma visão de atendimento com o histórico e o motivo das decisões, e painéis gerenciais com indicadores atualizados.

Os objetivos principais são reduzir o tempo da decisão de crédito, aumentar a consistência dessas decisões, dar ao atendimento uma visão completa do cliente e substituir a apuração manual de indicadores por informação confiável e tempestiva. Como benefícios esperados, a proposta busca aumentar a aprovação de bons clientes, reduzir o retrabalho operacional, melhorar a experiência no aplicativo e apoiar decisões gerenciais mais rápidas. Metas de referência, a serem calibradas com dados internos, seriam reduzir o tempo médio de decisão de crédito, elevar a taxa de aprovação de bons clientes sem aumentar a inadimplência e diminuir o tempo médio de atendimento das dúvidas ligadas a crédito.

### 1.3 Soluções existentes

O mercado oferece várias abordagens para problemas semelhantes, e vale contrastá-las com a proposta do grupo. Uma primeira categoria são os sistemas de *core banking* integrados, como Temenos e Finastra, que unificam produtos e processos bancários em uma única plataforma. Eles resolvem a fragmentação na origem, mas exigem substituição dos sistemas legados, com custo elevado, prazo longo de implantação e risco de interromper serviços essenciais, algo que o próprio cenário do Banco Horizonte recomenda evitar.

Uma segunda categoria são as plataformas de visão única do cliente, os chamados *Customer 360* e as *Customer Data Platforms*, das quais o Salesforce Financial Services Cloud é um exemplo conhecido no setor financeiro. Elas consolidam o histórico do cliente para áreas de relacionamento e vendas, o que se aproxima da nossa ideia, embora costumem ser genéricas e centradas em marketing, sem foco no processo específico de decisão de crédito.

Uma terceira categoria são os motores de decisão de crédito, oferecidos por empresas como Serasa Experian e FICO, que aplicam regras e modelos de score para automatizar a análise. São poderosos na etapa de decisão, mas trabalham sobre os dados que recebem, de modo que não resolvem, por si só, o problema de reunir e padronizar informação espalhada em vários sistemas. Por fim, há as ferramentas de integração e as de Business Intelligence, como plataformas de iPaaS para conectar sistemas e Power BI ou Tableau para painéis gerenciais, que são peças de infraestrutura úteis, porém não constituem uma solução de negócio pronta para o problema descrito.

O diferencial da Horizonte 360 está na combinação e no recorte. Em vez de trocar os sistemas, ela integra os que já existem por meio de uma camada intermediária, o que reduz custo e risco para um banco de médio porte. Em vez de uma visão genérica do cliente, ela é desenhada em torno de um processo de negócio bem definido, a concessão de crédito e o atendimento a ela associado. E, diferentemente de um motor de crédito isolado, ela cuida também da consolidação e da governança dos dados que alimentam a decisão, além de devolver essa informação, de forma compreensível, para quem atende o cliente e para quem administra o banco.

## 2. Solução Proposta

### 2.1 Funcionalidades

A Horizonte 360 organiza suas funcionalidades em torno de uma base comum, a visão consolidada do cliente, e de três públicos que a utilizam: o analista de crédito, o atendente e a gestão.

**Visão única do cliente.** Reúne em uma só tela o perfil consolidado: dados de cadastro, produtos contratados, solicitações anteriores de crédito e suas decisões, movimentações financeiras relevantes, reclamações registradas e situação atual da conta. É a fundação sobre a qual as demais funcionalidades operam.

**Painel de decisão de crédito.** Voltado ao analista, apresenta de forma organizada a renda declarada e estimada, o histórico interno de pagamentos, o comportamento financeiro do cliente e o score de crédito. Sobre esse conjunto, o painel exibe uma recomendação de decisão (aprovar, recusar ou aprovar com limite ajustado) acompanhada de uma justificativa estruturada e de um limite sugerido. A recomendação é um apoio, e a decisão final continua com o analista.

**Visão de atendimento.** Oferece ao atendente a mesma base consolidada, adaptada à sua necessidade. Traz um resumo da situação do cliente, o motivo da última decisão de crédito em linguagem clara e os próximos passos possíveis, para que o atendente responda no primeiro contato, sem abrir chamados ou encaminhar a solicitação a outro setor.

**Painel gerencial.** Consolida os indicadores que a diretoria precisa acompanhar: taxa de aprovação de crédito, tempo médio de decisão, inadimplência por perfil de cliente, reclamações recorrentes e rentabilidade por produto. Substitui as extrações manuais por informação atualizada de forma automática.

**Registro e trilha de decisões.** Mantém o histórico de cada decisão de crédito, com os dados que a embasaram e o responsável, o que apoia auditoria interna e conformidade regulatória. Complementa o conjunto uma função de **alertas de pendências**, que sinaliza solicitações paradas em alguma etapa do fluxo de crédito.

### 2.2 Questões técnicas

Do ponto de vista tecnológico, a solução se apoia em quatro camadas, coerentes com a ideia de sistema integrado apresentada na disciplina, porém sem a substituição total que um ERP tradicional exigiria.

**Camada de integração.** Conecta os sistemas de cadastro, crédito e CRM por meio de APIs e de um barramento de integração (padrão de API gateway ou iPaaS). Essa camada é responsável por buscar e enviar informação entre os sistemas de origem, respeitando o funcionamento de cada um.

**Camada de dados.** Um repositório analítico centralizado, no modelo de data warehouse, recebe cópias organizadas dos dados relevantes por meio de rotinas de extração, transformação e carga (ETL). Nesse fluxo, os dados são extraídos dos sistemas de cadastro, crédito e CRM, transformados para um formato comum (padronização de campos, aplicação da chave única de cliente e deduplicação) e carregados no repositório, de onde alimentam a visão única e os painéis. Parte dessas cargas pode ser agendada em lotes periódicos, e os dados mais sensíveis à decisão, como uma atualização de cadastro, podem ser sincronizados de forma quase imediata. Esse repositório sustenta tanto a visão única quanto os painéis gerenciais, sem sobrecarregar os sistemas operacionais de origem.

**Camada de aplicação.** Comporta o painel de decisão de crédito, a visão de atendimento e o motor de regras que gera as recomendações. Para os painéis gerenciais, integra-se uma ferramenta de Business Intelligence.

**Infraestrutura.** A operação em nuvem é adequada ao volume de cerca de três milhões de clientes, por oferecer escalabilidade de processamento e de armazenamento, além de disponibilidade e conectividade compatíveis com um banco digital cujo canal principal é o aplicativo. Ainda que a segurança não seja o foco do projeto, a proteção dos dados pessoais é obrigatória: criptografia em trânsito e em repouso, controle de acesso por perfil de usuário e aderência à Lei Geral de Proteção de Dados são requisitos técnicos inegociáveis. A qualidade dos dados depende de mecanismos de deduplicação e de um catálogo com definições comuns, para que o mesmo dado tenha o mesmo significado em todas as áreas.

### 2.3 Questões organizacionais

A adoção da Horizonte 360 depende de mudanças que vão além da tecnologia. A mais importante é a instituição de uma **governança de dados**. É necessário definir quem é responsável por cada conjunto de informação, padronizar definições (o que conta como renda, como se classifica uma reclamação) e estabelecer regras de qualidade e atualização. Sem isso, a visão única apenas reúne dados inconsistentes em um lugar só.

O **processo de concessão de crédito** precisa ser revisto para que as etapas de cadastro, análise e decisão passem a compartilhar a mesma base, em vez de operar em sequência isolada. Isso exige redefinir papéis e responsabilidades e criar, ainda que de forma enxuta, uma área ou comitê de dados que coordene a iniciativa. Em termos de recursos, o projeto demanda uma equipe de integração, profissionais de análise de dados e, sobretudo, patrocínio da diretoria, pois se trata de uma decisão organizacional, e não de uma escolha restrita à área de tecnologia.

Entre as barreiras previsíveis está a resistência das áreas acostumadas aos silos, em especial a de risco, que hoje domina suas planilhas e pode ver a mudança como perda de controle. Há também a dependência do fornecedor terceirizado de crédito, que precisa disponibilizar acesso a seus dados por meio de integração, o que envolve negociação contratual. Somam-se a esses pontos os riscos usuais de projetos de integração: a dificuldade de conectar sistemas legados, a qualidade incerta dos dados antigos, o custo e o prazo. A gestão da mudança, com comunicação clara dos ganhos e envolvimento das áreas desde o início, é o principal instrumento para reduzir esses riscos.

### 2.4 Questões humanas

Os efeitos sobre as pessoas variam conforme o papel de cada uma. Para o **atendente**, a mudança tende a ser positiva no dia a dia, já que ele deixa de percorrer várias telas e passa a resolver dúvidas sobre crédito no primeiro contato, com mais autonomia e menos encaminhamentos. Em contrapartida, precisa ser treinado na nova ferramenta e aprender a confiar na informação apresentada, o que só acontece se os dados forem, de fato, confiáveis.

Para o **analista de crédito**, a plataforma reduz o trabalho manual de reunir dados e oferece uma recomendação de apoio. Existe aqui um ponto de atenção humano relevante: o analista pode sentir que a recomendação automática ameaça sua autonomia. Por isso a solução deixa explícito que a decisão final é humana, e que o sistema informa, mas não decide. Para a **diretoria e a gerência**, o ganho está em substituir a consolidação manual de planilhas por painéis atualizados, o que muda a rotina de acompanhamento e exige alguma familiarização com as novas visões.

Para o **cliente**, que é quem sustenta o negócio, os efeitos são sentidos como aprovação mais rápida e explicações mais claras sobre as decisões, o que reduz frustração e reforça a confiança no banco. Já a **área de risco** vive a transição mais delicada, pois sai de um modo de trabalho baseado em planilhas próprias para um ambiente compartilhado, o que demanda acompanhamento e apoio ao longo da adoção.

### 2.5 Processos de negócio

Três processos de negócio são diretamente afetados. O primeiro, e mais importante, é o **processo de concessão de crédito**. Hoje ele é fragmentado, com etapas que não trocam informação de forma automática. Com a solução, o processo é aprimorado: as etapas passam a operar sobre a mesma visão consolidada, a análise recebe um apoio de recomendação e a decisão fica registrada com sua justificativa. O benefício esperado é uma decisão mais rápida, mais consistente e rastreável.

O segundo é o **processo de atendimento a dúvidas sobre crédito e conta**. Atualmente, o atendente depende de consultas a múltiplos sistemas e de chamados internos. O processo é redesenhado para que a informação necessária esteja disponível em uma única visão, o que reduz o tempo de resposta e a necessidade de transferir o cliente entre setores.

O terceiro é o **processo de acompanhamento gerencial**. Ele deixa de depender de extrações e cruzamentos manuais de planilhas e passa a ser sustentado por painéis alimentados de forma automática. Trata-se, na prática, de um processo aprimorado e parcialmente automatizado, cujo benefício é a disponibilidade de indicadores confiáveis para decisão. Nenhum desses processos é criado do zero, o que reforça o caráter incremental da proposta.

## 3. Processamento da Informação

### 3.1 Dados de entrada

A solução se alimenta de dados que já existem na organização, obtidos dos próprios sistemas por meio da camada de integração. Do sistema de **cadastro** vêm os dados pessoais, o CPF, os dados de contato, a ocupação e a renda declarada. Do sistema de **crédito** terceirizado vêm o score, o histórico de solicitações e decisões anteriores e a análise de renda. Da plataforma de **CRM** vêm as reclamações, os chamados e o histórico de contatos. Dos sistemas **transacionais** da conta vêm as movimentações relevantes, os pagamentos e a contratação de produtos, que revelam o comportamento financeiro do cliente.

A esses dados internos somam-se fontes **externas** consultadas no momento da análise, como os bureaus de crédito (Serasa e SPC) e, de forma opcional e mediante consentimento, dados de Open Finance. A origem de cada dado é sempre um sistema já existente ou um serviço externo já utilizado pelo banco, o que reforça que a plataforma reúne e organiza informação, sem criar uma nova base de coleta.

Cabe uma distinção importante em relação ao escopo. A plataforma **lê** as movimentações da conta para compor o comportamento financeiro do cliente, mas não **processa** as transações em si. O processamento de Pix, pagamentos e uso de cartão continua a cargo dos sistemas transacionais atuais, que permanecem fora do escopo do projeto. A Horizonte 360 consome esses registros como insumo de análise, sem interferir na operação que os gera.

### 3.2 Processamento

O processamento transforma dados brutos em informação útil para a decisão, e é aqui que se aplica a distinção central da disciplina entre dado e informação. Um registro isolado como "score 620" ou "três Pix devolvidos no mês" é apenas um dado, sem significado suficiente para decidir. O tratamento realizado pela plataforma dá contexto a esses fatos.

O primeiro passo é a **unificação e a padronização**. Os dados vindos de sistemas diferentes são reconciliados por uma chave única de cliente, o CPF, com deduplicação de registros e padronização de formatos e definições. Em seguida, a informação é **consolidada** na visão única do cliente. Sobre essa base, um **motor de regras e score** combina renda, histórico interno de pagamentos, comportamento financeiro e informações de bureau para produzir uma avaliação de risco e uma recomendação de decisão. Esse motor aplica regras de negócio explícitas, o que permite gerar, junto com a recomendação, uma **justificativa estruturada** que torna a decisão explicável.

Paralelamente, o processamento realiza **agregações** para os indicadores gerenciais, calculando, por exemplo, a taxa de aprovação em um período ou a inadimplência por perfil de cliente. É nesse ponto que o dado bruto se converte em informação: "score 620, renda compatível e histórico interno sem atrasos" passa a significar "cliente de risco médio, apto a um limite sugerido de determinado valor", uma afirmação que reduz a incerteza de quem decide.

### 3.3 Informações geradas

As informações produzidas são direcionadas a cada público. Para o **analista de crédito**, a plataforma gera a recomendação de decisão, a justificativa que a sustenta e o limite sugerido, o que apoia uma análise mais rápida e fundamentada. Para o **atendente**, gera um resumo da situação do cliente, o motivo da última decisão de crédito em linguagem acessível e os próximos passos, o que permite responder ao cliente com clareza e no primeiro contato.

Para a **diretoria e a gerência**, produz os indicadores consolidados, taxa de aprovação, tempo médio de decisão, inadimplência por perfil, reclamações recorrentes e rentabilidade por produto, apresentados em painéis atualizados. Essas informações apoiam a organização em diferentes níveis, o que dialoga com a pirâmide de tipos de sistemas de informação estudada na disciplina. No nível operacional e de atendimento, a plataforma se aproxima de um Sistema de Processamento de Transações ao apoiar decisões rotineiras e imediatas sobre cada cliente. No nível gerencial, os painéis de acompanhamento funcionam como um Sistema de Informações Gerenciais, ao consolidar relatórios periódicos que permitem monitorar o desempenho do crédito e identificar desvios, enquanto o motor de recomendação de crédito exerce papel próximo de um Sistema de Apoio à Decisão, ao tratar uma análise não totalmente estruturada. No nível estratégico, os indicadores oferecem à diretoria uma base confiável, ao modo de um Sistema de Apoio ao Executivo, para decidir sobre expansão, ajuste de política de crédito e priorização de investimentos, decisões que hoje são prejudicadas pela demora e pela imprecisão dos relatórios manuais.

## 4. Valor Organizacional e Vantagem Competitiva

### 4.1 Cadeia de valor

A cadeia de valor de Porter, embora concebida para empresas industriais, pode ser adaptada a um banco digital, com o cuidado de renomear atividades que no modelo original tratam de bens físicos. As **atividades primárias** do Banco Horizonte podem ser lidas da seguinte forma. A logística interna corresponde à captação e ao registro de clientes e de seus dados, isto é, o cadastro e o onboarding. As operações, coração do negócio, correspondem à análise e à concessão de crédito e ao processamento das transações. A logística externa, que no modelo original trata da distribuição de produtos físicos, aqui equivale à entrega dos produtos financeiros, como a liberação de um limite de crédito e sua disponibilização no aplicativo. O marketing e vendas correspondem à oferta e à precificação dos produtos. Os serviços correspondem ao atendimento e ao pós-venda.

As **atividades de apoio** incluem a infraestrutura da empresa, que abrange a gestão e, de forma destacada neste caso, a tecnologia e a governança de dados, a gestão de recursos humanos, o desenvolvimento tecnológico, entendido como a construção dos sistemas e da própria plataforma, e as compras, que aqui envolvem fornecedores estratégicos como a empresa terceirizada de crédito, os provedores de nuvem e os bureaus.

A Horizonte 360 atua com mais força em duas atividades primárias e em duas de apoio. Nas **operações**, melhora a decisão de crédito ao reunir e qualificar a informação, com ganho de tempo e de consistência, o que reduz tanto a recusa de bons clientes quanto as aprovações mal fundamentadas. Nos **serviços**, qualifica o atendimento ao dar visão completa do cliente, com ganho de qualidade e de tempo de resposta. No **desenvolvimento tecnológico** e na **infraestrutura**, a camada de integração e a governança de dados criam um ativo reutilizável que reduz o retrabalho e prepara o terreno para integrações futuras. Os tipos de ganho, portanto, combinam qualidade e tempo, redução de custo operacional pela eliminação de tarefas manuais e coordenação, ao fazer a informação fluir entre áreas que antes trabalhavam isoladas.

### 4.2 Vantagem competitiva

O setor bancário brasileiro é ao mesmo tempo altamente competitivo e regulado. Bancos tradicionais modernizam seus aplicativos, fintechs oferecem serviços especializados e empresas de tecnologia avançam sobre pagamentos e crédito, ao passo que os clientes se mostram cada vez menos fiéis e trocam de instituição diante de qualquer falha. Nesse ambiente, a capacidade de decidir crédito com rapidez e de explicar as decisões deixa de ser detalhe operacional e passa a influenciar diretamente a retenção de clientes.

A solução contribui para a competitividade por meio de mecanismos claros. Pela **eficiência**, decisões mais rápidas convertem mais solicitações em contratos e reduzem o custo operacional das análises e do atendimento. Pela **diferenciação**, a transparência na explicação de uma recusa, algo raro entre concorrentes, fortalece a confiança e melhora a experiência no aplicativo, que é o principal ponto de contato do banco. Pela **intimidade com o cliente**, a visão consolidada do histórico permite ofertas mais adequadas e apoia a retenção, elevando o custo de mudança percebido pelo usuário. E pela **melhor tomada de decisão**, os painéis gerenciais dão à diretoria agilidade estratégica que o processo manual atual não permite.

À luz das estratégias competitivas genéricas discutidas na disciplina, a proposta posiciona o Banco Horizonte principalmente na combinação de intimidade com o cliente e diferenciação, apoiada por ganhos de eficiência operacional. Os resultados esperados são a redução do tempo de aprovação, o aumento da aprovação de bons clientes, a diminuição de perdas causadas por decisões inconsistentes e a redução do churn associado ao atrito no crédito e no atendimento. Para tornar esses resultados verificáveis, o banco pode acompanhar indicadores como o tempo médio de decisão de crédito, a taxa de aprovação de bons clientes frente à inadimplência observada, o tempo médio de resolução das dúvidas sobre crédito no atendimento e a taxa de retenção de clientes que passaram por uma análise de crédito. Esses indicadores, já produzidos pelos painéis gerenciais, permitem medir se a solução entrega o valor prometido, e não apenas afirmá-lo. Convém, por fim, reconhecer os trade-offs. A solução aumenta a dependência de fornecedores externos, exige investimento e prazo de implantação, impõe cuidados permanentes de privacidade sob a LGPD e traz o risco de excesso de confiança na recomendação automática, motivo pelo qual a decisão final permanece com o analista humano. O reconhecimento desses limites é parte do que torna a proposta viável, e não apenas desejável.

## 5. Referências Bibliográficas

LAUDON, Kenneth C.; LAUDON, Jane P. *Sistemas de Informação Gerenciais*. 11. ed. São Paulo: Pearson Education do Brasil, 2014.

PORTER, Michael E. *Estratégia Competitiva: técnicas para análise de indústrias e da concorrência*. Rio de Janeiro: Elsevier, 2004.

PORTER, Michael E. *Vantagem Competitiva: criando e sustentando um desempenho superior*. Rio de Janeiro: Campus, 1989.

BRASIL. Lei nº 13.709, de 14 de agosto de 2018. *Lei Geral de Proteção de Dados Pessoais (LGPD)*. Brasília, 2018.

BANCO CENTRAL DO BRASIL. *Open Finance no Brasil*. Disponível no portal do Banco Central do Brasil.

TOTVS. *Cadeia de valor: o que é, para que serve e como aplicar*. Material de apoio da disciplina SSC0120.

Material didático da disciplina SSC0120 — Sistemas de Informação (ICMC/USP), aulas sobre conceitos fundamentais de SI, vantagem competitiva e forças de Porter, tipos de SI nas empresas e sistemas integrados (ERP).

---

## Nota sobre o uso de ferramentas de Inteligência Artificial

Em conformidade com a exigência de transparência do enunciado, o grupo registra que ferramentas de Inteligência Artificial foram utilizadas como apoio nas seguintes etapas: organização da estrutura do texto conforme o roteiro do projeto, revisão de redação e de coesão, e apoio à sistematização das ideias discutidas pelo grupo. A definição do problema, o recorte de escopo, as decisões de solução e a validação do conteúdo à luz do material da disciplina foram conduzidas pelos integrantes.
