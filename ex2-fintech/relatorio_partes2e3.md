# Exercício 2 (NovaCred) — Partes 2 e 3 — SSC0120 - Sistemas de Informação

Feito por:

Cauê Paiva Lira - 14675416

Letícia Barbosa Neves - 14588659

Pedro Lucas Figueiredo Bahiense - 14675458

João Pedro Alves Notari Godoy - 14582076

---

# Cadeia de Valor e Integração Estratégica — NovaCred

## 1. Cadeia de Valor

A Cadeia de Valor de Porter permite identificar onde a NovaCred gera valor para seus clientes e onde os Sistemas de Informação contribuem para eficiência ou diferenciação. A seguir, analisamos as atividades primárias e de apoio da empresa, indicando em cada uma o tipo de ganho obtido.

### 1.1 Atividades Primárias

#### Logística Interna (captação e integração de dados)

Na NovaCred, a logística interna corresponde à captação, integração e preparação dos dados que alimentam toda a operação. Como a empresa opera 100% online, seus "insumos" não são matérias-primas físicas, mas dados: transações financeiras, informações cadastrais, dados comportamentais do aplicativo e, cada vez mais, dados compartilhados via Open Finance.

**Como agrega valor:** a qualidade dos dados de entrada determina a qualidade de todas as decisões posteriores, desde a análise de crédito até a personalização de ofertas. Dados bem integrados reduzem erros e permitem decisões mais rápidas.

**Papel do SI:** o SI é responsável por coletar dados de múltiplas fontes (APIs do Open Finance, registros internos, dados de parceiros), organizá-los e garantir sua consistência. Ferramentas de Big Data permitem processar grandes volumes com velocidade, enquanto políticas de governança de dados asseguram rastreabilidade e conformidade com as exigências do Banco Central.

**Tipo de ganho:** qualidade/tempo (dados prontos para uso mais rápido), redução de risco (governança previne inconsistências e falhas regulatórias).

---

#### Operações (processamento e decisão)

As operações são o núcleo da NovaCred: é onde ocorre a análise automatizada de crédito via inteligência artificial, o processamento de transações financeiras em tempo real e a automação de tarefas repetitivas como conciliação e validação de documentos no onboarding.

**Como agrega valor:** o cliente recebe uma resposta de crédito em minutos (não em dias, como em bancos tradicionais). As transações são processadas instantaneamente. A automação reduz erros humanos e libera equipes para atividades de maior valor.

**Papel do SI:** a arquitetura em microsserviços permite escalar cada função de negócio de forma independente (o serviço de crédito pode escalar em picos sem afetar o de investimentos). A IA analisa dados históricos e comportamentais para calibrar decisões de crédito, especialmente para perfis com histórico financeiro raso (jovens e MEIs). Processos de automação (RPA combinado com IA) cuidam de tarefas operacionais como validação documental.

**Tipo de ganho:** redução de custo (automação substitui trabalho manual repetitivo), diferenciação (crédito rápido e mais preciso que concorrentes tradicionais), qualidade/tempo (decisões em segundos).

---

#### Logística Externa (distribuição e canais)

A distribuição dos produtos e serviços da NovaCred acontece inteiramente por canais digitais. O aplicativo móvel é o principal ponto de contato, complementado por integrações com meios de pagamento como Pix e cartão de crédito/débito.

**Como agrega valor:** o cliente acessa todos os serviços (conta, crédito, investimentos, pagamentos) em um único aplicativo, sem necessidade de deslocamento físico. A abertura de conta e a contratação de crédito são feitas online, com fricção mínima.

**Papel do SI:** o aplicativo é sustentado por APIs que integram os diversos serviços internos e externos (Pix, bandeiras de cartão, Open Finance). A operação 100% digital elimina custos de agências físicas e permite atender clientes em qualquer localidade. A integração com Pix por aproximação (NFC) e carteiras digitais expande os canais de uso sem exigir infraestrutura adicional.

**Tipo de ganho:** redução de custo (eliminação de canais físicos), qualidade/tempo (serviços disponíveis 24h, contratação instantânea).

---

#### Marketing e Vendas (personalização e segmentação)

O marketing da NovaCred é orientado por dados. A empresa utiliza Big Data para segmentar seu público (jovens adultos e MEIs), entender comportamentos de consumo e oferecer produtos contextualizados ao momento de vida de cada cliente.

**Como agrega valor:** em vez de ofertas genéricas, o cliente recebe recomendações que fazem sentido para sua situação, como um limite de crédito ajustado ao faturamento real do MEI ou alertas de investimento adequados ao perfil de risco do jovem adulto.

**Papel do SI:** motores de recomendação alimentados por dados transacionais e comportamentais permitem hiperpersonalização. Com a integração do Open Finance, a NovaCred pode acessar dados de outras instituições (com consentimento do cliente), criando uma visão mais completa para oferecer produtos mais relevantes. Isso reduz o custo de aquisição ao direcionar esforços para perfis com maior probabilidade de conversão.

**Tipo de ganho:** diferenciação (ofertas personalizadas que concorrentes genéricos não conseguem replicar), coordenação/integração (Open Finance conecta dados de múltiplas fontes para análise mais precisa).

---

#### Serviços (pós-venda e suporte)

Os serviços incluem atendimento ao cliente, monitoramento de transações, alertas financeiros e ferramentas de gestão integradas ao aplicativo.

**Como agrega valor:** o cliente tem controle financeiro na palma da mão: alertas de gastos, notificações de movimentação, histórico detalhado. Para o MEI, o app oferece funcionalidades de controle de fluxo de caixa, alertas de recebimentos e organização financeira que vão além de uma simples conta bancária.

**Papel do SI:** sistemas de monitoramento em tempo real detectam comportamentos suspeitos e protegem o cliente contra fraudes. Chatbots e atendimento automatizado resolvem dúvidas frequentes sem necessidade de intervenção humana, reduzindo custos de suporte. A integração de todas essas funcionalidades no mesmo aplicativo cria conveniência que aumenta a retenção.

**Tipo de ganho:** diferenciação (ferramentas de gestão financeira que outros serviços não oferecem de forma integrada), redução de custo (automação do atendimento).

---

### 1.2 Atividades de Apoio

#### Infraestrutura da Empresa

A infraestrutura da NovaCred inclui sua arquitetura de computação em nuvem, políticas de segurança, governança de dados e processos de conformidade regulatória.

**Como agrega valor:** garante que todos os serviços funcionem com disponibilidade, segurança e conformidade. Sem infraestrutura confiável, nenhum produto digital funciona.

**Papel do SI:** a empresa utiliza estratégia multicloud (múltiplos provedores de nuvem) para evitar dependência de um único fornecedor e garantir continuidade operacional. Políticas de segurança Zero Trust protegem cada chamada de API individualmente. A governança de dados atende às exigências do Banco Central e da LGPD. Práticas de FinOps (gestão financeira da nuvem) otimizam custos ao evitar recursos ociosos.

**Tipo de ganho:** redução de risco (conformidade, segurança, continuidade), redução de custo (FinOps evita desperdício).

---

#### Gestão de Recursos Humanos

A NovaCred possui equipes de desenvolvimento de software, análise de dados, marketing digital, atendimento ao cliente e gestão de risco. Como empresa nativa digital, sua cultura organizacional é orientada a experimentação e agilidade.

**Como agrega valor:** equipes especializadas garantem a qualidade dos produtos e a velocidade de inovação. A cultura ágil permite responder rapidamente a mudanças regulatórias e competitivas.

**Papel do SI:** ferramentas de colaboração e gestão de projetos sustentam o trabalho distribuído. A automação de tarefas repetitivas libera profissionais para atividades analíticas e estratégicas. A ausência de legado organizacional (diferente dos bancos tradicionais, que enfrentam resistência à mudança em estruturas hierárquicas rígidas) permite que novas tecnologias e processos sejam adotados com menor atrito.

**Tipo de ganho:** diferenciação (agilidade organizacional superior à de concorrentes com legado).

---

#### Desenvolvimento Tecnológico

O desenvolvimento tecnológico é central para a NovaCred: a empresa investe continuamente em sua arquitetura de microsserviços, em modelos de IA para análise de crédito e em integrações com novas infraestruturas regulatórias.

**Como agrega valor:** permite lançar novos produtos e adaptar-se a mudanças (como a integração com Drex ou novas regras do Open Finance) mais rapidamente que concorrentes com sistemas legados.

**Papel do SI:** a arquitetura baseada em microsserviços e APIs permite que cada componente seja atualizado independentemente. Modelos de IA são treinados continuamente com dados de inadimplência e comportamento, melhorando com o tempo. A integração com regulações emergentes (Drex, Pix por aproximação, portabilidade de crédito via Open Finance) é viabilizada por essa arquitetura flexível.

**Tipo de ganho:** diferenciação (inovação mais rápida), coordenação/integração (APIs conectam com ecossistema regulatório e parceiros), qualidade/tempo (atualizações sem parar o sistema).

---

#### Aquisições e Gestão de Fornecedores

A NovaCred depende de parceiros externos críticos: provedores de nuvem, bandeiras de cartão, sistemas de pagamento, instituições financeiras reguladas e o próprio Banco Central como regulador.

**Como agrega valor:** a gestão adequada desses relacionamentos garante a continuidade e a qualidade dos serviços oferecidos ao cliente final.

**Papel do SI:** APIs desacopladas permitem trocar ou adicionar fornecedores com menor impacto na operação. O monitoramento automatizado dos SLAs (Service Level Agreements, ou acordos de nível de serviço) de cada parceiro permite identificar problemas antes que afetem o cliente. A estratégia multicloud e o uso de padrões abertos (como Kubernetes) reduzem o risco de lock-in tecnológico.

**Tipo de ganho:** redução de risco (diversificação de fornecedores, contingência), coordenação/integração (APIs padronizadas facilitam gestão de múltiplos parceiros).

---

## 2. Integração Estratégica

Com base nas análises das Cinco Forças de Porter (Parte 1) e da Cadeia de Valor (acima), propomos duas estratégias para a NovaCred melhorar sua posição competitiva.

### Estratégia 1: Hiperpersonalização baseada em dados integrados

**O que é:** utilizar a combinação de dados internos (transações, comportamento no app) com dados externos (Open Finance) para oferecer a cada cliente produtos e condições ajustados ao seu momento de vida, de forma automatizada e contínua.

**Conexão com a Cadeia de Valor:** essa estratégia integra três atividades: a logística interna (captação e integração de dados de múltiplas fontes), as operações (modelos de IA que transformam dados em decisões de crédito e recomendações) e o marketing/vendas (ofertas personalizadas entregues no momento certo).

**Conexão com Porter:** a hiperpersonalização mitiga a rivalidade ao criar diferenciação difícil de copiar (não basta ter os mesmos produtos, é preciso ter os mesmos dados e modelos calibrados). Também mitiga o poder de barganha dos clientes ao gerar switching cost por valor acumulado, pois quanto mais o cliente usa a plataforma, mais preciso o serviço se torna, e migrar para outro player significa perder essa "inteligência" construída sobre seu perfil.

**Como o SI sustenta:** o SI viabiliza toda a cadeia dado → informação → conhecimento. Dados brutos de transações são transformados em informação contextualizada (padrões de consumo, risco de inadimplência, sazonalidade do faturamento do MEI) e, ao longo do tempo, em conhecimento organizacional incorporado nos modelos de IA. Sem o SI integrando processos, pessoas e tecnologia, esses dados permaneceriam fragmentos isolados sem utilidade para decisão.

---

### Estratégia 2: Plataforma integrada de gestão financeira para MEIs

**O que é:** transformar o aplicativo da NovaCred em uma plataforma completa de gestão financeira para microempreendedores, indo além de conta e crédito para oferecer controle de fluxo de caixa, alertas de recebimentos, organização de despesas e crédito contextualizado ao histórico do negócio.

**Conexão com a Cadeia de Valor:** essa estratégia combina serviços (ferramentas de gestão e controle no app), operações (crédito automatizado ajustado ao fluxo de caixa real do MEI) e marketing/vendas (segmentação específica para um público com dores distintas do consumidor pessoa física).

**Conexão com Porter:** mitiga a ameaça de substitutos ao oferecer uma jornada integrada que nenhum produto isolado (Pix, plataforma de investimento, app de gestão) consegue replicar sozinho. Também cria barreiras contra novos entrantes, pois os dados acumulados sobre o comportamento financeiro dos MEIs ao longo dos cinco anos de operação da NovaCred são um ativo que um entrante novo não possui.

**Como o SI sustenta:** o SI integra dados de recebimentos via Pix, pagamentos com cartão, histórico de crédito e padrões sazonais do negócio para gerar informação acionável (por exemplo, identificar que o faturamento do MEI cai em janeiro e oferecer capital de giro preventivo). A arquitetura em microsserviços permite adicionar novas funcionalidades de gestão sem redesenhar o sistema. O atendimento automatizado (chatbots, alertas inteligentes) reduz o custo de suportar essa base de clientes com margens menores.

---

## 3. Considerações Finais

A análise da Cadeia de Valor revela que o SI da NovaCred não é uma camada de suporte isolada, mas o elemento que conecta e potencializa todas as atividades da empresa. Desde a captação de dados (logística interna) até o atendimento pós-venda (serviços), passando pela análise de crédito automatizada (operações) e pela personalização de ofertas (marketing), cada elo da cadeia depende do SI para funcionar e gerar valor.

As duas estratégias propostas, hiperpersonalização e plataforma para MEIs, são viáveis justamente porque a NovaCred já possui as atividades de apoio necessárias: infraestrutura em nuvem escalável, equipes com cultura ágil, desenvolvimento tecnológico baseado em microsserviços e gestão de fornecedores diversificada. Isso não seria possível em uma organização que tratasse SI apenas como "o sistema que roda no computador".

Para que essas estratégias se concretizem, é necessário atenção às três dimensões do SI como sistema sociotécnico:

- **Tecnologia**: manter a arquitetura flexível para integrar novas fontes de dados (Open Finance, Drex) e novos canais (Pix por aproximação).
- **Organização**: governança de dados robusta para garantir conformidade (LGPD, Banco Central) e processos ágeis para lançar funcionalidades rapidamente.
- **Pessoas**: equipes capacitadas para interpretar modelos de IA e traduzir dados em valor para o cliente, além de atendimento preparado para as particularidades do público MEI.
