# Estudo de Caso — Vodafone: uma implementação ERP global e gigante

Disciplina SSC0120 — Sistemas de Informação (ICMC/USP)

Feito por:

Cauê Paiva Lira - 14675416

Letícia Barbosa Neves - 14588659

Pedro Lucas Figueiredo Bahiense - 14675458

João Pedro Alves Notari Godoy - 14582076

---

## 1. Contexto do caso

A Vodafone Group Plc é a maior provedora de serviço móvel do mundo em receita, com cerca de 400 milhões de clientes na Europa, Oriente Médio, África, Ásia e Estados Unidos. Em 2012, faturou US$ 71,8 bilhões e empregava mais de 86 mil funcionários em mais de 40 países. Boa parte desse crescimento veio da aquisição de operadoras locais, estratégia que permitiu à empresa atender mercados regionais com marcas e equipes já estabelecidas.

O efeito colateral desse modelo foi uma empresa profundamente descentralizada. Cada subsidiária operava como companhia independente, com seus próprios processos de negócio e sistemas. Faltavam práticas comuns, operações centralizadas e compartilhamento de dados entre as operadoras. A Vodafone funcionava como uma rede de operadoras individuais, embora quisesse atuar como uma única empresa global para enfrentar as pressões competitivas do setor.

Em 2006, o conselho aprovou o programa "Evolução Vodafone" (EVO), uma transformação organizacional para remodelar a empresa em uma organização verdadeiramente global, com serviços compartilhados e processos comuns em finanças, recursos humanos e gestão da cadeia de suprimentos. A plataforma tecnológica escolhida para sustentar a mudança foi o ERP da SAP, complementado por ferramentas de Informatica, Opentext, ReadSoft, Sabrix, Redwood, HP e Remedy. O resultado foi uma das maiores implementações de SAP ERP do mundo.

Este documento responde às perguntas 9.13 a 9.17 do estudo de caso, aplicando os conceitos da disciplina: a visão sociotécnica do Sistema de Informação (tecnologia, organização e pessoas), a distinção entre dado e informação, e o papel do ERP como sistema integrado com base de dados central comum.

---

## 2. Questão 9.13 — O problema e os fatores que contribuíram para ele

### 2.1 O problema central

O problema da Vodafone era a **fragmentação operacional decorrente do crescimento por aquisição**. A empresa havia se tornado um conjunto de operadoras independentes, cada uma com processos e sistemas próprios, sem práticas comuns nem compartilhamento de dados. Essa descentralização impedia a Vodafone de operar como uma única empresa global e de explorar sua escala.

Um sintoma concreto aparece na área de compras. Como cada operadora local gerenciava suas próprias aquisições, a Vodafone não conseguia alavancar seu poder de compra massivo junto aos fornecedores como se fosse uma única entidade. A empresa tinha o tamanho de uma gigante, mas comprava como dezenas de empresas pequenas. O mesmo padrão se repetia em finanças e RH, com processos redundantes e custos elevados.

Vale separar dois conceitos que a disciplina enfatiza. A Vodafone não sofria por falta de dados, pois cada operadora coletava muitos. O problema era que esses dados ficavam isolados em silos por país, sem definições e formatos comuns, e por isso não se transformavam em **informação consolidada e comparável** que a administração global pudesse usar para decidir. Coletar dados localmente não é o mesmo que gerar informação útil para a empresa como um todo.

### 2.2 Fatores organizacionais

- Crescimento por aquisição de operadoras locais, que gerou uma federação de empresas autônomas em vez de uma organização unificada.
- Ausência de serviços compartilhados, com cada subsidiária mantendo estruturas próprias de finanças, RH e compras.
- Compras descentralizadas, que desperdiçavam o poder de barganha da escala global.
- Processos de negócio diferentes em cada país, parte deles moldados por requisitos legais locais.

### 2.3 Fatores tecnológicos

- Grande quantidade de sistemas legados incompatíveis. A operadora alemã, sozinha, mantinha mais de 130 sistemas legados customizados.
- Plataformas heterogêneas entre países (a subsidiária húngara, por exemplo, rodava software Oracle).
- Falta de uma base de dados comum, o que impedia uma visão única e integrada do negócio.

### 2.4 Fatores humanos

- Hábitos de trabalho profundamente arraigados, especialmente nas operadoras maiores e mais antigas como a Alemanha.
- Resistência à mudança por parte de funcionários acostumados aos sistemas e processos locais.
- Falta de experiência e de recursos internos para conduzir um projeto dessa complexidade, o que levou à contratação de consultorias (Accenture e IBM).

**Implicação:** o problema da Vodafone era sociotécnico, e não apenas tecnológico. Trocar sistemas legados por SAP resolveria a dimensão tecnológica, mas só a redefinição de processos (organização) e a gestão da resistência (pessoas) tornariam a transformação efetiva.

---

## 3. Questão 9.14 — Por que tanto tempo lidando com a mudança

A Vodafone gastou tanto tempo com a mudança porque a transformação envolveu dezenas de implantações distintas, cada uma em uma realidade diferente, e não um único projeto uniforme. Vários fatores explicam essa lentidão.

**Escala e diversidade das operadoras.** Eram mais de 40 países, e nenhuma implantação procedia da mesma maneira, porque cada operadora apresentava desafios e demandas próprios. O número de usuários, a quantidade de interfaces, os sistemas legados e os requisitos legais variavam de país para país. A operadora alemã precisava substituir mais de 130 sistemas legados customizados, enquanto a húngara, de médio porte (cerca de dois mil funcionários), partia de uma plataforma Oracle pequena.

**Resistência e hábitos arraigados.** Nas operadoras maiores, os hábitos de trabalho estavam consolidados e havia resistência ao novo. A Alemanha exemplifica bem o desafio, pois respondia por cerca de 20% da receita, tinha 13 mil funcionários e mais de 130 sistemas legados customizados a substituir. Para reduzir riscos, a Vodafone optou por uma implantação incremental e em fases, fazendo uma enorme quantidade de ajustes antes de cada entrada em operação e enviando equipes de suporte para acompanhar os funcionários afetados na transição. Esse cuidado protege a adoção, mas consome tempo.

**Sensibilidade ao contexto local.** A equipe de projeto teve de se adaptar a tendências locais. Em uma operadora situada em país com crise econômica, os funcionários tendiam a ser mais resistentes, vendo a mudança como mais um problema a enfrentar num momento já estressante, e não como melhoria. Lidar com isso exigia ajustar a abordagem caso a caso, inclusive nas reuniões de lançamento, onde o grau de interesse da operadora local sinalizava quanta atenção o projeto exigiria.

**Aprendizado entre implantações.** A cada nova operadora, a equipe incorporava melhorias das implementações anteriores. Testes e opiniões dos funcionários levaram, por exemplo, a reformular o uso de itens que mereciam atenção e a refinar interfaces para torná-las mais fáceis de usar. Esse ciclo de refinamento contínuo alonga o cronograma, mas eleva a qualidade da adoção.

**Implicação:** o material da disciplina é direto ao apontar que, em implantações de ERP, a mudança cultural costuma ser a maior barreira, muitas vezes mais difícil que a parte técnica. A Vodafone tratou a gestão da mudança como atividade central porque o sucesso dependia, acima de tudo, da aceitação das pessoas. Instalar o software era a parte mais previsível do projeto.

---

## 4. Questão 9.15 — Por que um ERP foi necessário

O objetivo da transformação era fazer a Vodafone operar como uma única empresa global, com processos comuns e serviços compartilhados. Esse objetivo de negócio só era alcançável com um sistema que integrasse, de fato, as áreas funcionais sobre uma base de dados comum. É exatamente isso que define um ERP.

**O ERP fornece a base de dados central comum.** Um ERP é uma suíte de módulos integrados que coleta dados das diferentes divisões e os mantém em um banco de dados único. Quando um processo gera uma informação, ela fica imediatamente disponível para os demais. Sem essa base comum, finanças, RH e cadeia de suprimentos das operadoras continuariam isolados, e a Vodafone permaneceria fragmentada.

**Substituir os silos de sistemas legados.** A empresa convivia com centenas de sistemas independentes e incompatíveis (130+ só na Alemanha). Um ERP permitia aposentar esses legados e padronizar dados em definições e formatos comuns em toda a organização, transformando dados locais dispersos em informação corporativa confiável.

**Padronizar processos por meio das melhores práticas embutidas.** O software integrado é construído em torno de processos predefinidos. Adotar o SAP forçava as operadoras a convergir para formas comuns de trabalhar, em vez de cada uma manter o seu jeito. Foi esse mecanismo que viabilizou os serviços compartilhados, a consolidação de operações usadas por várias partes da empresa para reduzir custos e redundância.

**Habilitar a centralização das compras.** O exemplo mais claro é o processo de aquisição. Com o ERP, a Vodafone criou uma empresa de compras centralizada em Luxemburgo e passou a negociar como entidade única, alavancando seu poder de compra. O novo processo automatizou o ciclo do pedido ao pagamento, com faturas aprovadas automaticamente pela combinação entre pedidos e recibos. Esse nível de integração e automação entre áreas é inviável com sistemas fragmentados.

**Apoiar a decisão com informação integrada.** Com dados padronizados em um sistema único, a administração passa a enxergar o desempenho de qualquer unidade a qualquer momento. O ERP atua como base de processamento de transações (SPT) que alimenta relatórios gerenciais e análises, sustentando decisões mais rápidas e precisas no nível corporativo.

**Implicação:** o ERP foi a condição estrutural da transformação. Sem base de dados comum, sem processos padronizados e sem integração entre áreas, a meta de operar como empresa global única não se sustentaria.

---

## 5. Questão 9.16 — Questões consideradas para o sucesso

O sucesso da transformação dependeu de tratar as três dimensões do Sistema de Informação de forma integrada. A seguir, o que a equipe de projeto considerou em cada uma.

### 5.1 Questões humanas

- **Gestão da resistência e do contexto local.** A equipe foi sensível a tendências locais, reconhecendo que funcionários em países sob crise econômica reagiriam de modo diferente. A abordagem de cada operadora foi ajustada conforme o grau de receptividade.
- **Suporte e treinamento na transição.** Equipes de suporte foram enviadas para acompanhar os funcionários afetados durante a virada de sistemas.
- **Facilidade de uso para reduzir resistência.** A aposta na mobilidade tem fundamento humano. Segundo Niall O'Sullivan, diretor de transformação financeira, levar as funções para o celular aumenta a facilidade de uso e reduz a resistência, porque as pessoas se dispõem mais a usar um sistema acessível de onde estiverem. A meta era que a maioria das interações ocorresse por dispositivo móvel.
- **Envolvimento das equipes locais.** As reuniões reuniam equipes globais, equipes locais, consultores e fornecedores de TI locais em ambiente amigável, para incentivar o compartilhamento de conhecimento e a abertura à mudança.

### 5.2 Questões organizacionais

- **Sequenciamento por piloto e por prioridade.** A Hungria foi escolhida como piloto por ser de médio porte (cerca de dois mil funcionários) e receptiva à mudança, com uma plataforma de TI pequena já baseada em Oracle. Depois, a implantação avançou priorizando operadoras conforme tamanho, complexidade e disposição para mudar, chegando à Alemanha, maior mercado da empresa com cerca de 20% da receita.
- **Redefinir processos antes da tecnologia.** A empresa passou cerca de um ano identificando e projetando os novos processos e o escopo, antes de implantar o sistema. Optou por começar pelos processos que não eram voltados ao cliente, deixando os processos de linha de frente para fases posteriores, a fim de manter a transformação gerenciável.
- **Novas estruturas organizacionais.** Foram criadas a empresa de compras centralizada em Luxemburgo e organizações de serviços compartilhados em Budapeste e na Índia.
- **Parcerias para suprir competências.** Reconhecendo que não tinha experiência nem recursos internos para um projeto tão complexo, a Vodafone contratou Accenture e IBM, e ajustou estratégias a cada operadora ao longo do tempo.
- **Equilíbrio entre velocidade e qualidade.** A equipe precisou balancear a necessidade de avançar rápido com a garantia de que cada sistema fosse bem implantado.

### 5.3 Questões tecnológicas

- **Substituição e integração de legados.** Aposentar centenas de sistemas legados (130+ na Alemanha) e integrar tudo sobre a base SAP foi um desafio técnico central.
- **Configuração versus customização.** Acomodar os requisitos legais de cada país exigia adaptar o sistema sem cair em customização excessiva, que comprometeria a integração, principal benefício do ERP.
- **Testes e refinamento incremental.** A cada implantação, testes e opiniões dos funcionários alimentaram melhorias, como o refinamento de interfaces para torná-las mais fáceis de usar.
- **Plataforma móvel.** Disponibilizar aplicativos integrados em dispositivos móveis (o primeiro foi o de relatórios de viagem e despesas) foi parte da estratégia tecnológica para ampliar a adoção.

**Implicação:** nenhuma das três dimensões funcionaria isolada. A tecnologia do SAP só gerou valor porque veio acompanhada do redesenho de processos (organização) e de um esforço deliberado de aceitação e treinamento (pessoas).

---

## 6. Questão 9.17 — Benefícios e mudanças na operação e na decisão

### 6.1 Benefícios quantificáveis

- Redução de custos anuais de US$ 719 milhões, resultado da maior eficiência organizacional e da transformação dos processos de negócio.
- Redução do custo total de propriedade (TCO, do inglês *total cost of ownership*, que soma os gastos de aquisição, operação e manutenção da tecnologia ao longo do tempo) da tecnologia da informação, com a aposentadoria de centenas de sistemas legados redundantes.
- Ganhos de escala em compras, já que negociar como entidade única em Luxemburgo permitiu explorar o poder de barganha que antes se perdia na descentralização.

### 6.2 Benefícios qualitativos e de longo prazo

- Uma forma consistente de trabalhar em todo o mundo e uma estrutura organizacional mais unificada.
- Operadoras locais passando a pensar e agir de maneira mais uniforme, sob o modelo de serviços compartilhados, com expectativa de maior rentabilidade no longo prazo, ainda que parte dos ganhos não seja imediatamente quantificável.

### 6.3 Como mudou a tomada de decisão

Antes, os dados estavam presos em silos por país, sem formato comum, o que dificultava qualquer leitura consolidada do negócio. Com o ERP, esses dados passaram a ser padronizados e integrados em uma base comum, virando informação confiável e comparável entre operadoras. Isso permite à administração avaliar o desempenho de qualquer unidade a qualquer momento, com mais precisão e rapidez. O ERP funciona como a base transacional que alimenta os relatórios e análises gerenciais, sustentando decisões corporativas que antes esbarravam na falta de informação consolidada.

### 6.4 Como mudou a forma de operar

A Vodafone deixou de funcionar como uma federação de operadoras independentes e passou a operar como uma empresa global integrada. Processos antes locais e redundantes foram padronizados e centralizados em serviços compartilhados. O ciclo de compras, por exemplo, passou de aquisições isoladas para um fluxo automatizado do pedido ao pagamento, com faturas conciliadas automaticamente. A mobilidade ampliou o alcance do sistema: a empresa selecionou quatro aplicativos integrados para dispositivos móveis, sendo o primeiro o de relatórios de viagem e despesas, no qual o funcionário fotografa o recibo e emite ou aprova a solicitação sem papel. Mais de 60 mil funcionários já usavam o sistema em todo o mundo, com meta de cerca de 80% das transações por um único dispositivo móvel e previsão de 80 mil usuários até o fim de 2012.

### 6.5 Ressalvas e trade-offs

Os ganhos vieram acompanhados de limitações que convém registrar. Parte dos benefícios da uniformização não é imediatamente quantificável, sendo esperada apenas no longo prazo. A necessidade de acomodar requisitos legais de cada país pressionava por customizações que, se levadas longe demais, ameaçariam a própria integração que justifica o ERP. E a falta de competências internas tornou o projeto dependente de consultorias externas (Accenture e IBM), o que adiciona custo e cria dependência de fornecedores durante a transição.

**Implicação:** o valor da transformação está em mecanismos concretos, não em uma promessa vaga de eficiência. Integração reduz redundância e custo, padronização viabiliza a escala em compras, e a informação consolidada melhora a decisão. Esses três efeitos juntos converteram o tamanho da Vodafone, antes um obstáculo, em vantagem competitiva.

---

## 7. Conclusão

O caso Vodafone ilustra com clareza por que um Sistema de Informação não se reduz a software. A empresa tinha tecnologia de sobra e dados em abundância, mas operava fragmentada porque seus sistemas, processos e equipes não convergiam. O que de fato destravou a transformação foi o trabalho simultâneo nas três dimensões do Sistema de Informação: na **tecnologia**, ao substituir os sistemas legados por uma base de dados comum e integrada no SAP; na **organização**, ao padronizar processos e criar serviços compartilhados; e nas **pessoas**, ao administrar a resistência, o treinamento e a facilidade de uso.

O retorno apareceu em custo (US$ 719 milhões por ano e TCO menor), em escala (compras centralizadas) e em decisão (informação consolidada e comparável). A lição central, alinhada à disciplina, é que transformação organizacional bem-sucedida nasce de uma abordagem sociotécnica, na qual tecnologia, organização e pessoas mudam ao mesmo tempo.
