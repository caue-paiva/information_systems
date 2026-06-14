# Estudo de Caso: Graybar decide realizar análise de clientes

Disciplina SSC0120: Sistemas de Informação (ICMC/USP)

Feito por:

Cauê Paiva Lira - 14675416

Letícia Barbosa Neves - 14588659

Pedro Lucas Figueiredo Bahiense - 14675458

João Pedro Alves Notari Godoy - 14582076

---

## 1. Contexto do caso

A Graybar é uma empresa da lista Fortune 500, com sede em St. Louis (Missouri), e uma das maiores companhias norte-americanas cujos proprietários são os próprios empregados. Atua como distribuidora atacadista líder de produtos elétricos, de comunicações e de rede, e também oferece gestão da cadeia de suprimentos e serviços de logística associados a esses produtos. Com receita superior a US$ 5,4 bilhões, compra, armazena e entrega cerca de um milhão de produtos vindos de 4.100 fabricantes para 117 mil clientes, apoiada por 7.400 funcionários e mais de 240 centros de distribuição nos Estados Unidos, Canadá e Porto Rico. Por ser atacadista, não vende diretamente ao consumidor de varejo.

Apesar do sucesso, a Graybar não seguia as melhores práticas de análise e atendimento de clientes que vinham se tornando essenciais para distribuidores. Para reagir, em julho de 2011 o vice-presidente de desenvolvimento de negócios iniciou um projeto de estratificação de clientes, baseado nos próprios dados da empresa e inspirado em uma pesquisa da Universidade A&M do Texas. O projeto evoluiu de uma planilha para um painel construído no BusinessObjects Dashboards da SAP e, por fim, para o SAP Customer Value Intelligence, software analítico da suíte SAP Customer Analytics rodando sobre a plataforma em memória SAP HANA.

Este documento responde às quatro perguntas do estudo de caso, aplicando os conceitos da disciplina: a visão sociotécnica do Sistema de Informação (tecnologia, organização e pessoas), a distinção entre dado e informação, e o papel do CRM, em especial do CRM analítico, na transformação do relacionamento com o cliente.

---

## 2. Questão 1: O problema da Graybar e seu impacto no desempenho

### 2.1 O problema central

O problema da Graybar era a **incapacidade de distinguir clientes lucrativos de clientes não lucrativos e de alocar seus recursos comerciais de acordo com isso**. Como distribuidora atacadista, a empresa estava espremida entre fabricantes e clientes que pressionavam por preços menores, prazos de entrega mais curtos e melhores serviços, mas se recusavam a pagar pelos serviços adicionais. O resultado setorial era o arrochamento das margens de lucro.

Diante dessa pressão, os representantes de venda concentravam atenção principalmente nos clientes que gastavam mais. O negócio é muito transacional, com 21 mil pedidos e 90 mil itens de linha por dia, e aproximadamente 97% dos 117 mil clientes fecham negócios menores que US$ 25 mil por ano. Focar apenas nas grandes contas deixava a imensa maioria dos clientes sem atenção e sem critério para decidir quais valiam um relacionamento mais próximo e quais deveriam ser preteridos.

### 2.2 Dado não é informação

A Graybar não sofria por falta de dados. Pelo contrário, já mantinha cerca de 95% dos dados de cliente de que precisava. O problema é que parte desses dados se perdia e, sobretudo, a empresa não dispunha de ferramentas analíticas para segmentar os clientes segundo linhas de recomendação. Havia dado bruto em abundância (volume de vendas, devoluções, pedidos), mas faltava transformá-lo em **informação** capaz de responder à pergunta de negócio: quem é lucrativo, quem drena recursos e onde o esforço comercial rende mais.

### 2.3 Impacto no desempenho

- **Margens corroídas**: sem segmentar, a empresa atendia no mesmo nível clientes que davam lucro e clientes que davam prejuízo, agravando a pressão sobre as margens.
- **Força de vendas mal alocada**: o tempo dos representantes era investido por intuição e por tamanho de conta, não por retorno. Um modelo de alocação por geografia ou por linha de produto não garantia que os clientes mais lucrativos recebessem atenção proporcional.
- **Clientes service drain destruindo valor**: clientes de alto volume que exigiam atendimento constante, preços baixos e devolviam muito consumiam recursos sem retorno equivalente.
- **Oportunidades perdidas**: sem visão analítica, a Graybar não conseguia identificar quais clientes pouco rentáveis poderiam ser desenvolvidos para se tornarem lucrativos.

**Implicação:** o problema era de gestão da informação para decisão, não de coleta. Enquanto os dados não viravam segmentação acionável, a empresa decidia no escuro sobre onde investir sua capacidade comercial, o ativo mais caro em um negócio de margem apertada.

---

## 3. Questão 2: Questões humanas, organizacionais e tecnológicas

Desenvolver a solução de análise de clientes exigiu tratar as três dimensões do Sistema de Informação de forma integrada, e não apenas instalar um software. A seguir, o que a Graybar precisou considerar em cada uma.

### 3.1 Questões organizacionais

- **Equipe multifuncional.** O projeto reuniu representantes de marketing, operações, finanças e sistemas de informação, além de membros das operações de campo, que garantiram atenção às necessidades reais dos clientes atendidos.
- **Adoção de uma estratégia de estratificação.** A empresa adaptou ao seu negócio as melhores práticas da pesquisa da A&M do Texas, definindo quatro segmentos de cliente (principal, oportunista, marginal e service drain) a partir de vendas, lucratividade bruta, fidelidade e custo de atendimento.
- **Redesenho de políticas comerciais.** Cada segmento exige uma abordagem distinta de alocação da força de vendas, preços, marketing e compensação. Mudar isso significa rever a cultura de priorizar apenas grandes contas.

### 3.2 Questões humanas

- **Mudança no trabalho dos representantes.** Eles precisaram passar a alocar tempo e recursos com base na segmentação, em vez de seguir a intuição de focar quem gasta mais.
- **Apoio da liderança.** O patrocínio veio do vice-presidente de desenvolvimento de negócios, condição que o material da disciplina aponta como fundamental para o sucesso de um CRM.
- **Resistência à mudança de incentivos.** Como cada segmento passa a ter uma política própria de preços e de compensação da força de vendas, há risco de resistência dos representantes acostumados a serem remunerados pelo volume das grandes contas. Tratar essa mudança de incentivos é parte da gestão da mudança.
- **Informação fácil de usar.** A equipe queria a informação em formato visual e compreensível, o que levou à criação do painel. Na fase de teste, quase todos os vendedores quiseram rapidamente ver os clientes estratificados de suas regiões e fazer análises em tempo real, sinal de adesão quando a ferramenta responde à necessidade deles.

### 3.3 Questões tecnológicas

- **Aproveitamento do ERP e do data warehouse.** A equipe identificou no sistema ERP existente os campos necessários e escreveu as consultas para extrair os dados do data warehouse SAP NetWeaver.
- **Modelagem analítica.** Fatores como receita, poder de compra do cliente e penetração das linhas de produto receberam pesos conforme as necessidades do negócio.
- **Evolução da plataforma.** A solução começou em uma planilha com muitas linhas de dados, ganhou um painel no BusinessObjects Dashboards da SAP e culminou no SAP Customer Value Intelligence, da suíte SAP Customer Analytics.
- **Processamento em memória.** O SAP HANA acelerou a análise de grandes volumes transacionais e viabilizou o trabalho em tempo real, com dados de cliente em nível muito mais detalhado do que antes.
- **Qualidade dos dados.** Como parte dos dados se perdia, a confiabilidade da base era um requisito, ainda que a empresa já mantivesse 95% do necessário.

**Implicação:** a tecnologia (HANA, NetWeaver, Customer Value Intelligence) só gerou valor porque veio acompanhada do redesenho de processos comerciais (organização) e da mudança na forma de trabalhar e decidir dos vendedores (pessoas).

---

## 4. Questão 3: Como o CRM analítico mudou o negócio

### 4.1 O que é CRM analítico

O CRM analítico reúne as aplicações que analisam os dados de cliente gerados pelas operações da empresa, apoiando-se em um data warehouse que consolida informações de várias fontes para captar, processar, interpretar e apresentar esses dados. Diferente do CRM operacional, voltado às atividades de contato direto (vendas, atendimento, marketing), o CRM analítico existe para transformar o histórico do cliente em segmentação e recomendação. No caso da Graybar, ele é exatamente o motor que converte os dados transacionais em uma classificação acionável de clientes.

### 4.2 Antes do CRM analítico

- Foco concentrado nos clientes que gastavam mais, definido por intuição e tamanho de conta.
- Alocação da força de vendas por geografia ou linha de produto, sem garantir atenção proporcional aos clientes mais lucrativos.
- Maioria dos 117 mil clientes sem atenção e sem critério de priorização.
- Dados de cliente abundantes, porém dispersos, às vezes perdidos e sem ferramenta de segmentação.
- Relacionamento reativo, sem visão única e consolidada de cada cliente.

### 4.3 Depois do CRM analítico

- Clientes estratificados em quatro categorias (principal, oportunista, marginal e service drain) com base em vendas, lucratividade, fidelidade e custo de atendimento.
- Painel visual que mostra, para cada representante, a distribuição de seus clientes por categoria, orientando a alocação de tempo e recursos.
- Análise em tempo real por região geográfica, com perfis que explicam por que um cliente recebeu determinada classificação (por exemplo, pedidos inconsistentes em um oportunista ou alto volume de devoluções em um service drain).
- Recomendações para elevar o valor do cliente e identificar quais clientes pouco rentáveis podem ser desenvolvidos.
- Visão consolidada e detalhada do cliente, deslocando o foco do volume puro para a lucratividade.

### 4.4 O mecanismo da mudança

A transformação segue a lógica de dado para informação para decisão. Os mesmos dados transacionais que antes ficavam subaproveitados passaram a alimentar uma segmentação que diz a cada vendedor onde concentrar esforço. O negócio deixou de ser conduzido pela máxima de servir melhor quem compra mais e passou a ser conduzido pela leitura de quem gera valor e de quem pode passar a gerar. Esse é o ganho central do CRM analítico, coerente com o princípio de CRM de que uma fração dos clientes costuma concentrar a maior parte do resultado, exatamente o que a estrutura da Graybar sugere, com vendas concentradas em poucas contas grandes enquanto 97% dos clientes fecham menos de US$ 25 mil por ano.

**Implicação:** o CRM analítico não substituiu o relacionamento, mas o tornou seletivo e informado. A Graybar passou a praticar uma gestão de carteira orientada por lucratividade, sustentando ações de retenção, redução da taxa de cancelamento e venda cruzada nos segmentos certos.

---

## 5. Questão 4: Três decisões melhoradas pelo novo sistema

**1. Como cada representante aloca seu tempo e seus recursos.** O mapa visual de vendas mostra quantos dos clientes de um representante são principais, oportunistas, marginais ou service drain. Em vez de distribuir esforço pela intuição de tamanho de conta, o vendedor passa a decidir, com base na distribuição real da carteira, onde investir atenção para maximizar retorno.

**2. Quais clientes desenvolver, renegociar ou preterir.** Os perfis detalhados permitem decidir caso a caso. Um service drain com alto volume de devoluções pode ter preços e condições de serviço renegociados. Um oportunista com pedidos inconsistentes pode receber ações para regularizar a compra. Um marginal que só dá prejuízo pode deixar de consumir recursos prioritários. A decisão de transformar um service drain em cliente lucrativo, antes impossível de fundamentar, agora se apoia em dados.

**3. Definição de preços, marketing e compensação por segmento.** A estratificação embasa políticas comerciais diferenciadas por categoria de cliente. A empresa decide preços, campanhas de marketing e a forma de remunerar a força de vendas de acordo com o segmento, e ganha apoio para decisões de cobertura por mercado geográfico, já que os vendedores passaram a enxergar a estratificação de suas regiões específicas.

**Implicação:** as três decisões compartilham a mesma raiz, que é substituir o palpite por evidência. O sistema não decide pela Graybar, mas dá ao gestor e ao vendedor a informação que faltava para escolher melhor onde aplicar um recurso comercial escasso.

---

## 6. Ressalvas e trade-offs

Os ganhos do CRM analítico vêm acompanhados de limitações que convém registrar.

- **Dependência de fornecedor.** A solução está fortemente ancorada no ecossistema SAP (ERP, data warehouse NetWeaver, HANA e Customer Value Intelligence). O material da disciplina alerta que aplicações integradas geram custos de mudança e tornam a empresa dependente do fornecedor para manter e atualizar seus produtos.
- **Custo, complexidade e qualidade dos dados.** A segmentação só é confiável se a base for confiável. Como parte dos dados se perdia, a Graybar depende de limpeza e governança contínuas dos dados, além do investimento em infraestrutura analítica.
- **Risco de rótulos estáticos.** Despriorizar clientes marginais ou oportunistas pode fazer a empresa perder clientes que cresceriam com o tempo. A própria Graybar reconhece que um cliente service drain pode ser transformado em lucrativo, o que mostra que as categorias precisam ser revistas periodicamente, e não tratadas como sentença definitiva.
- **Privacidade e foco interno.** Concentrar grande volume de dados de cliente exige cuidado com segurança e privacidade, e a régua de lucratividade não pode se sobrepor por completo à relação de longo prazo que sustenta um distribuidor atacadista.

**Implicação:** a estratificação é uma ferramenta de decisão, não um veredito. Seu valor depende de revisão periódica dos segmentos e de equilíbrio entre lucratividade de curto prazo e construção de relacionamento.

---

## 7. Conclusão

O caso Graybar mostra que o gargalo de uma empresa rica em dados pode estar justamente na ausência de meios para transformá-los em informação útil. A Graybar já tinha 95% dos dados de cliente, mas operava sem segmentação, sem visão consolidada e sem critério de priorização, o que pressionava margens já apertadas e desperdiçava o tempo da força de vendas. O CRM analítico, sustentado pelo data warehouse SAP NetWeaver, pelo SAP Customer Value Intelligence e pelo processamento em memória do SAP HANA, converteu esse acervo de dados em uma classificação acionável de clientes.

O ganho, porém, não veio só da tecnologia. Ele dependeu das três dimensões do Sistema de Informação atuando juntas. Na **tecnologia**, a empresa extraiu e analisou os dados em tempo real. Na **organização**, montou uma equipe multifuncional e redesenhou as políticas de preço, marketing e compensação por segmento. Nas **pessoas**, mudou a forma como os vendedores priorizam clientes e entregou a informação em um painel que eles efetivamente quiseram usar. O resultado é uma gestão de relacionamento orientada por lucratividade, que apoia retenção, redução da taxa de cancelamento e venda cruzada onde elas de fato compensam.
