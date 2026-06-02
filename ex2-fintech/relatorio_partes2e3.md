# Exercício 2 (NovaCred) — Partes 2 e 3 — SSC0120 - Sistemas de Informação

Feito por:

Cauê Paiva Lira - 14675416

Letícia Barbosa Neves - 14588659

Pedro Lucas Figueiredo Bahiense - 14675458

João Pedro Alves Notari Godoy - 14582076

---

# Cadeia de Valor e Integração Estratégica — NovaCred

## 1. Cadeia de Valor

A NovaCred é uma empresa de serviços financeiros digitais. Seus produtos principais são: conta digital, cartão de crédito sem anuidade, empréstimos pessoais com análise automatizada e uma plataforma de investimentos simplificada. Toda a operação acontece online, sustentada por inteligência artificial para análise de crédito, big data para personalização e aplicativos móveis como canal de relacionamento. Seu público prioritário são jovens adultos e microempreendedores.

A Cadeia de Valor de Porter permite identificar onde a NovaCred gera valor ao entregar esses produtos financeiros aos seus clientes e onde os Sistemas de Informação contribuem para eficiência ou diferenciação em cada etapa. A seguir, analisamos as atividades primárias e de apoio da empresa, indicando em cada uma o tipo de ganho obtido.

### 1.1 Atividades Primárias

#### Operações (produtos e serviços financeiros)

O núcleo da NovaCred é a oferta de produtos financeiros digitais: **conta digital** para movimentação e recebimentos, **cartão de crédito sem anuidade** para compras e pagamentos, **empréstimos pessoais com análise automatizada** para acesso a crédito rápido, e uma **plataforma de investimentos simplificada** para aplicações financeiras. Esses quatro produtos compõem o portfólio que atende tanto jovens adultos (que buscam praticidade e baixo custo) quanto microempreendedores (que precisam de crédito acessível e controle financeiro do negócio).

**Como agrega valor:** o cliente abre uma conta em minutos, sem burocracia. Solicita um empréstimo e recebe resposta em segundos, não em dias como em bancos tradicionais. Usa um cartão sem anuidade para compras do dia a dia. Investe em produtos de renda fixa ou variável diretamente no app. A automação dos processos internos permite que a NovaCred ofereça esses produtos a custos mais baixos que bancos tradicionais, repassando essa economia ao cliente (como a isenção de anuidade do cartão).

**Papel do SI:** o SI integra os dados do cliente (cadastrais, transacionais, comportamentais) e os transforma em informação que sustenta cada produto. Na concessão de crédito, por exemplo, o sistema cruza histórico de pagamentos, renda estimada e padrões de consumo para gerar uma avaliação de risco personalizada, permitindo aprovar perfis com histórico financeiro raso (jovens e MEIs) que seriam recusados por modelos tradicionais de scoring bancário. Na conta digital, o SI organiza e apresenta ao cliente suas movimentações de forma estruturada, transformando dados brutos de transações em informação útil para controle financeiro. A automação de processos internos (validação de documentos, conciliação de transações) reduz custos operacionais e viabiliza produtos como o cartão sem anuidade.

**Tipo de ganho:** redução de custo (automação viabiliza produtos como cartão sem anuidade), diferenciação (crédito acessível a perfis subatendidos pelo sistema bancário tradicional), qualidade/tempo (aprovação de crédito e abertura de conta em minutos).

---

#### Canais e Distribuição (como os produtos financeiros chegam ao cliente)

Todos os produtos financeiros da NovaCred, conta digital, cartão, empréstimos e investimentos, chegam ao cliente por um único canal: o aplicativo móvel. Não há agências, não há correspondentes bancários. O app é ao mesmo tempo a "vitrine", o "balcão de atendimento" e o "caixa" da empresa. O cliente abre conta, contrata crédito, faz pagamentos via Pix, usa o cartão e aplica em investimentos, tudo no mesmo lugar.

**Como agrega valor:** o cliente acessa todos os seus produtos financeiros 24 horas por dia, de qualquer lugar, sem deslocamento. A contratação de crédito ou abertura de conta acontece em minutos, com fricção mínima. Para o MEI que precisa resolver uma questão financeira do negócio às 22h, o app é o único canal necessário.

**Papel do SI:** o SI unifica todos os produtos financeiros em uma única interface, permitindo que o cliente gerencie conta, cartão, crédito e investimentos em um só lugar. Essa integração de informações é o que diferencia o app de ter quatro produtos separados: o cliente vê seu saldo, seus gastos no cartão, suas parcelas de empréstimo e seus rendimentos de investimento de forma consolidada, com uma visão completa da sua vida financeira. A operação 100% digital elimina custos de agências físicas e permite atender clientes em qualquer localidade do país.

**Tipo de ganho:** redução de custo (eliminação de canais físicos), qualidade/tempo (produtos financeiros disponíveis 24h, contratação instantânea).

---

#### Marketing e Vendas (oferta personalizada de produtos financeiros)

A NovaCred não oferece os mesmos produtos da mesma forma para todos. Utilizando Big Data, a empresa segmenta seu público (jovens adultos e microempreendedores) e ajusta a oferta de cada produto financeiro ao perfil e momento de vida do cliente. Um MEI com faturamento estável recebe oferta de capital de giro com condições específicas para seu negócio. Um jovem adulto com perfil conservador recebe sugestões de investimentos de renda fixa, não de renda variável.

**Como agrega valor:** em vez de ofertas genéricas iguais para todos (como um banco tradicional faria), o cliente recebe propostas de crédito, investimento e serviços que fazem sentido para sua situação real. Isso aumenta a chance de o produto ser útil e reduz a inadimplência (crédito oferecido a quem pode pagar).

**Papel do SI:** o SI coleta e organiza dados transacionais e comportamentais de cada cliente, transformando-os em informação que permite segmentar o público e ajustar a oferta. Por exemplo, ao processar os dados de recebimentos via Pix de um MEI, o SI identifica a regularidade do faturamento e gera a informação de que aquele cliente tem capacidade de pagamento estável, o que fundamenta uma oferta de capital de giro com condições adequadas. Com a integração do Open Finance, o SI também acessa dados de outras instituições (com consentimento do cliente), ampliando a visão financeira para oferecer condições de crédito e investimento mais precisas. Isso reduz o custo de aquisição ao direcionar esforços de venda para perfis com maior probabilidade de conversão.

**Tipo de ganho:** diferenciação (ofertas financeiras personalizadas que concorrentes genéricos não conseguem replicar), coordenação/integração (Open Finance conecta dados de múltiplas instituições para análise mais precisa do cliente).

---

#### Serviços (gestão financeira contínua e suporte ao cliente)

Depois que o cliente abre a conta, contrata crédito ou faz investimentos, a NovaCred continua entregando valor por meio de serviços de gestão financeira e suporte. O app oferece alertas de gastos no cartão, notificações de movimentação da conta, acompanhamento de investimentos e histórico financeiro detalhado. Para o MEI, o app funciona como ferramenta de gestão do negócio: controle de fluxo de caixa, alertas de recebimentos via Pix, organização de despesas.

**Como agrega valor:** o cliente não precisa de uma planilha ou outro app para controlar sua vida financeira. Tudo está integrado na mesma plataforma onde ele já tem conta, cartão e crédito. Para o MEI, isso resolve uma dor concreta: organizar as finanças do negócio sem precisar de contador ou software à parte.

**Papel do SI:** o SI monitora continuamente as transações do cliente e transforma padrões de uso em alertas úteis: aviso de gasto acima do habitual no cartão, notificação de recebimento via Pix para o MEI, alerta de vencimento de parcela do empréstimo. Ao consolidar todas essas informações financeiras em um único lugar, o SI transforma dados dispersos (transações, parcelas, rendimentos) em uma visão integrada que o cliente usa para tomar decisões sobre seu dinheiro. O atendimento automatizado resolve dúvidas frequentes sobre os produtos (limite, parcelas, rendimentos), reduzindo custos de suporte.

**Tipo de ganho:** diferenciação (gestão financeira integrada aos produtos, não oferecida separadamente), redução de custo (automação do atendimento sobre os produtos).

---

### 1.2 Atividades de Apoio

#### Infraestrutura da Empresa

A infraestrutura da NovaCred inclui sua arquitetura de computação em nuvem, políticas de segurança, governança de dados e processos de conformidade regulatória.

**Como agrega valor:** garante que todos os serviços funcionem com disponibilidade, segurança e conformidade. Sem infraestrutura confiável, nenhum produto digital funciona.

**Papel do SI:** como a operação é 100% digital, o SI é a própria infraestrutura do negócio. A governança de dados garante que informações financeiras sensíveis dos clientes (saldos, histórico de crédito, dados cadastrais) sejam armazenadas, processadas e compartilhadas em conformidade com as exigências do Banco Central e da LGPD. Políticas de segurança protegem os dados contra acessos indevidos e fraudes. Para a NovaCred, qualquer falha na gestão dessas informações impacta diretamente a confiança do cliente e a conformidade regulatória.

**Tipo de ganho:** redução de risco (conformidade, segurança, continuidade), redução de custo (FinOps evita desperdício).

---

#### Gestão de Recursos Humanos

A NovaCred possui equipes de desenvolvimento de software, análise de dados, marketing digital, atendimento ao cliente e gestão de risco. Como empresa nativa digital, sua cultura organizacional é orientada a experimentação e agilidade.

**Como agrega valor:** equipes especializadas garantem a qualidade dos produtos e a velocidade de inovação. A cultura ágil permite responder rapidamente a mudanças regulatórias e competitivas.

**Papel do SI:** a automação de tarefas repetitivas (conciliação, validação documental) libera profissionais para atividades analíticas e estratégicas. A ausência de legado organizacional, diferente dos bancos tradicionais que enfrentam resistência à mudança em estruturas hierárquicas rígidas, permite que novas tecnologias e processos sejam adotados com menor atrito. Isso exige, porém, investimento contínuo em treinamento para que as equipes acompanhem a evolução das ferramentas de IA, dados e segurança que sustentam a operação.

**Tipo de ganho:** diferenciação (agilidade organizacional superior à de concorrentes com legado).

---

#### Desenvolvimento Tecnológico

O desenvolvimento tecnológico é central para a NovaCred: a empresa investe continuamente nos modelos de IA para análise de crédito, nas formas de coletar e processar dados dos clientes e na integração com novas infraestruturas regulatórias.

**Como agrega valor:** permite lançar novos produtos e adaptar-se a mudanças (como a integração com Drex ou novas regras do Open Finance) mais rapidamente que concorrentes com sistemas legados.

**Papel do SI:** os modelos de IA que sustentam a análise de crédito são treinados continuamente com dados de inadimplência e comportamento dos clientes, melhorando suas decisões com o tempo. Esse refinamento contínuo é um ativo do SI: quanto mais dados acumulados e processados, mais precisas as decisões de crédito. Além disso, o SI precisa se adaptar rapidamente para integrar novas fontes de dados e regulações emergentes (Drex, portabilidade de crédito via Open Finance, Pix por aproximação), garantindo que a NovaCred consiga incorporar essas mudanças antes dos concorrentes.

**Tipo de ganho:** diferenciação (modelos de decisão que melhoram com o tempo e dados acumulados), coordenação/integração (integração com ecossistema regulatório e parceiros), qualidade/tempo (adaptação rápida a mudanças regulatórias).

---

#### Aquisições e Gestão de Fornecedores

A NovaCred depende de parceiros externos críticos: provedores de nuvem, bandeiras de cartão, sistemas de pagamento, instituições financeiras reguladas e o próprio Banco Central como regulador.

**Como agrega valor:** a gestão adequada desses relacionamentos garante a continuidade e a qualidade dos serviços oferecidos ao cliente final.

**Papel do SI:** o SI gerencia o fluxo de informações entre a NovaCred e seus parceiros: dados de transações com bandeiras de cartão, informações de pagamento com o Pix, dados regulatórios compartilhados com o Banco Central. A qualidade e continuidade desses fluxos de informação determinam se os produtos funcionam corretamente para o cliente. Sistemas de monitoramento acompanham a disponibilidade e desempenho de cada parceiro, identificando degradações antes que afetem o cliente final.

**Tipo de ganho:** redução de risco (monitoramento contínuo dos fluxos de informação com parceiros), coordenação/integração (gestão estruturada da troca de dados com múltiplos parceiros externos).

---

## 2. Integração Estratégica

Com base nas análises das Cinco Forças de Porter (Parte 1) e da Cadeia de Valor (acima), propomos duas estratégias para a NovaCred melhorar sua posição competitiva.

### Estratégia 1: Hiperpersonalização baseada em dados integrados

**O que é:** utilizar a combinação de dados internos (transações, comportamento no app) com dados externos (Open Finance) para oferecer a cada cliente produtos e condições ajustados ao seu momento de vida, de forma automatizada e contínua.

**Conexão com a Cadeia de Valor:** essa estratégia integra duas atividades primárias: as operações (modelos de IA que transformam dados em decisões de crédito e recomendações) e o marketing/vendas (ofertas personalizadas entregues no momento certo), apoiadas pelo desenvolvimento tecnológico (refinamento contínuo dos modelos com dados acumulados).

**Conexão com Porter:** a hiperpersonalização mitiga a rivalidade ao criar diferenciação difícil de copiar (não basta ter os mesmos produtos, é preciso ter os mesmos dados e modelos calibrados). Também mitiga o poder de barganha dos clientes ao gerar switching cost por valor acumulado, pois quanto mais o cliente usa a plataforma, mais preciso o serviço se torna, e migrar para outro player significa perder essa "inteligência" construída sobre seu perfil.

**Como o SI sustenta:** o SI viabiliza toda a cadeia dado → informação → conhecimento. Dados brutos de transações são transformados em informação contextualizada (padrões de consumo, risco de inadimplência, sazonalidade do faturamento do MEI) e, ao longo do tempo, em conhecimento organizacional incorporado nos modelos de IA. Sem o SI integrando processos, pessoas e tecnologia, esses dados permaneceriam fragmentos isolados sem utilidade para decisão.

**Riscos e trade-offs:** acumular mais dados do cliente para personalização aumenta a superfície de ataque e a responsabilidade sob a LGPD, exigindo investimento contínuo em segurança e conformidade. Há também o risco de viés algorítmico: modelos de IA treinados com dados históricos podem reproduzir padrões de exclusão em vez de incluir perfis subatendidos, o que contraria a proposta de valor da NovaCred. Por fim, manter a infraestrutura de dados integrados (Open Finance + dados internos + modelos de IA) tem custo operacional significativo que precisa ser justificado pelo retorno em retenção e conversão.

---

### Estratégia 2: Plataforma integrada de gestão financeira para MEIs

**O que é:** transformar o aplicativo da NovaCred em uma plataforma completa de gestão financeira para microempreendedores, indo além de conta e crédito para oferecer controle de fluxo de caixa, alertas de recebimentos, organização de despesas e crédito contextualizado ao histórico do negócio.

**Conexão com a Cadeia de Valor:** essa estratégia combina serviços (ferramentas de gestão e controle no app), operações (crédito automatizado ajustado ao fluxo de caixa real do MEI) e marketing/vendas (segmentação específica para um público com dores distintas do consumidor pessoa física).

**Conexão com Porter:** mitiga a ameaça de substitutos ao oferecer uma jornada integrada que nenhum produto isolado (Pix, plataforma de investimento, app de gestão) consegue replicar sozinho. Também cria barreiras contra novos entrantes, pois os dados acumulados sobre o comportamento financeiro dos MEIs ao longo dos cinco anos de operação da NovaCred são um ativo que um entrante novo não possui.

**Como o SI sustenta:** o SI integra dados de recebimentos via Pix, pagamentos com cartão, histórico de crédito e padrões sazonais do negócio para gerar informação acionável (por exemplo, identificar que o faturamento do MEI cai em janeiro e oferecer capital de giro preventivo). O atendimento automatizado (alertas inteligentes, notificações de fluxo de caixa) reduz o custo de suportar essa base de clientes com margens menores.

**Riscos e trade-offs:** o principal risco é de escopo. Tentar ser "tudo para o MEI" (conta, crédito, gestão, pagamentos, contabilidade) pode diluir o foco e aumentar a complexidade operacional, elevando custos de desenvolvimento e suporte. A NovaCred precisa definir até onde vai e o que é melhor resolvido por parceiros via integração. Além disso, parte dos dados usados para contextualizar o crédito do MEI vem de terceiros via Open Finance, cujo acesso depende de regulação que pode mudar. Se o Banco Central alterar as regras de compartilhamento, a base de dados da estratégia pode ser comprometida.

---

## 3. Considerações Finais

A análise da Cadeia de Valor revela que o SI da NovaCred não é uma camada de suporte isolada, mas o elemento que conecta e potencializa todas as atividades da empresa. Desde a oferta dos produtos financeiros (operações) até o atendimento pós-venda (serviços), passando pela distribuição via app (canais) e pela personalização de ofertas (marketing/vendas), cada elo da cadeia depende do SI para funcionar e gerar valor.

As duas estratégias propostas, hiperpersonalização e plataforma para MEIs, são viáveis justamente porque a NovaCred já possui as atividades de apoio necessárias: infraestrutura com governança de dados, equipes com cultura ágil, desenvolvimento tecnológico com modelos de IA que se refinam continuamente e gestão estruturada de fornecedores. Isso não seria possível em uma organização que tratasse SI apenas como "o sistema que roda no computador".

Para que essas estratégias se concretizem, é necessário atenção às três dimensões do SI como sistema sociotécnico:

- **Tecnologia**: manter a arquitetura flexível para integrar novas fontes de dados (Open Finance, Drex) e novos canais (Pix por aproximação).
- **Organização**: governança de dados robusta para garantir conformidade (LGPD, Banco Central) e processos ágeis para lançar funcionalidades rapidamente.
- **Pessoas**: equipes capacitadas para interpretar modelos de IA e traduzir dados em valor para o cliente, além de atendimento preparado para as particularidades do público MEI.
