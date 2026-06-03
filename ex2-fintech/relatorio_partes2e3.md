# Exercício 2 (NovaCred) — Partes 2 e 3 — SSC0120 - Sistemas de Informação

Feito por:

Cauê Paiva Lira - 14675416

Letícia Barbosa Neves - 14588659

Pedro Lucas Figueiredo Bahiense - 14675458

João Pedro Alves Notari Godoy - 14582076

---

# Cadeia de Valor e Integração Estratégica — NovaCred

## 1. Cadeia de Valor

A Cadeia de Valor de Porter permite identificar onde a NovaCred gera valor ao entregar seus produtos financeiros digitais aos clientes e onde os Sistemas de Informação contribuem para eficiência ou diferenciação em cada etapa. A seguir, analisamos as atividades primárias e de apoio da empresa, indicando em cada uma o tipo de ganho obtido.

### 1.1 Atividades Primárias

#### Operações (produtos e serviços financeiros)

O núcleo da NovaCred é a oferta de produtos financeiros digitais: **conta digital** para movimentação e recebimentos, **cartão de crédito sem anuidade** para compras e pagamentos, **empréstimos pessoais com análise automatizada** para acesso a crédito rápido, e uma **plataforma de investimentos simplificada** para aplicações financeiras. Esses quatro produtos compõem o portfólio que atende tanto jovens adultos (que buscam praticidade e baixo custo) quanto microempreendedores (que precisam de crédito acessível e controle financeiro do negócio).

**Como agrega valor:** o cliente abre uma conta em minutos, sem burocracia. Solicita um empréstimo e recebe resposta em segundos, não em dias como em bancos tradicionais. Usa um cartão sem anuidade para compras do dia a dia. Investe em produtos de renda fixa ou variável diretamente no app. A automação dos processos internos permite que a NovaCred ofereça esses produtos a custos mais baixos que bancos tradicionais, repassando essa economia ao cliente (como a isenção de anuidade do cartão).

**Papel do SI:** o SI integra os dados do cliente (cadastrais, transacionais, comportamentais) e os transforma em informação que sustenta cada produto. Na concessão de crédito, por exemplo, o sistema cruza histórico de pagamentos, renda estimada e padrões de consumo para gerar uma avaliação de risco personalizada, permitindo aprovar perfis com histórico financeiro raso (jovens e MEIs) que seriam recusados por modelos tradicionais de scoring bancário. Na conta digital, o SI organiza e apresenta ao cliente suas movimentações de forma estruturada, transformando dados brutos de transações em informação útil para controle financeiro. A automação de processos internos (validação de documentos, conciliação de transações) reduz custos operacionais e viabiliza produtos como o cartão sem anuidade. Os modelos de IA, por sua vez, dependem da equipe de gestão de risco para definir seus parâmetros e ajustar critérios quando o perfil de inadimplência muda, garantindo que as decisões automatizadas continuem adequadas ao público da NovaCred.

**Tipo de ganho:** redução de custo (automação viabiliza produtos como cartão sem anuidade), diferenciação (crédito acessível a perfis subatendidos pelo sistema bancário tradicional), qualidade/tempo (aprovação de crédito e abertura de conta em minutos).

---

#### Canais e Distribuição (como os produtos financeiros chegam ao cliente)

Diferente de um banco tradicional com agências físicas, a NovaCred entrega todos os seus produtos por um único canal: o aplicativo móvel. O app funciona como "vitrine", "balcão" e "caixa" ao mesmo tempo. O cliente acessa conta, cartão, crédito e investimentos 24 horas por dia, de qualquer lugar, contratando serviços em minutos e sem deslocamento.

**Papel do SI:** o SI define como a informação financeira é organizada, priorizada e apresentada ao cliente. Não se trata apenas do aplicativo como software, mas de um conjunto de decisões sobre quais dados mostrar, em que ordem e com que contexto: o saldo aparece junto com os gastos recentes no cartão, as parcelas de empréstimo são exibidas ao lado do rendimento dos investimentos, e o fluxo de caixa do MEI é consolidado a partir de dados de múltiplas fontes. Essas decisões de organização da informação envolvem equipes de produto e negócio (não apenas desenvolvedores) e processos de design que traduzem dados financeiros em uma experiência compreensível para o público da NovaCred. A operação 100% digital elimina custos de agências físicas e permite atender clientes em qualquer localidade do país.

**Tipo de ganho:** redução de custo (eliminação de canais físicos), qualidade/tempo (produtos financeiros disponíveis 24h, contratação instantânea).

---

#### Marketing e Vendas (oferta personalizada de produtos financeiros)

A NovaCred não oferece os mesmos produtos da mesma forma para todos. Utilizando Big Data, a empresa segmenta seu público (jovens adultos e microempreendedores) e ajusta a oferta de cada produto financeiro ao perfil e momento de vida do cliente. Um MEI com faturamento estável recebe oferta de capital de giro com condições específicas para seu negócio. Um jovem adulto com perfil conservador recebe sugestões de investimentos de renda fixa, não de renda variável.

**Como agrega valor:** em vez de ofertas genéricas iguais para todos (como um banco tradicional faria), o cliente recebe propostas de crédito, investimento e serviços que fazem sentido para sua situação real. Isso aumenta a chance de o produto ser útil e reduz a inadimplência (crédito oferecido a quem pode pagar).

**Papel do SI:** o SI coleta e organiza dados transacionais e comportamentais de cada cliente, transformando-os em informação que permite segmentar o público e ajustar a oferta. Por exemplo, ao processar os dados de recebimentos via Pix de um MEI, o SI identifica a regularidade do faturamento e gera a informação de que aquele cliente tem capacidade de pagamento estável, o que fundamenta uma oferta de capital de giro com condições adequadas. Com a integração do Open Finance, o SI também acessa dados de outras instituições (com consentimento do cliente), ampliando a visão financeira para oferecer condições de crédito e investimento mais precisas. Isso reduz o custo de aquisição ao direcionar esforços de venda para perfis com maior probabilidade de conversão.

**Tipo de ganho:** diferenciação (ofertas financeiras personalizadas que concorrentes genéricos não conseguem replicar), coordenação/integração (Open Finance conecta dados de múltiplas instituições para análise mais precisa do cliente).

---

#### Serviços (gestão financeira contínua e suporte ao cliente)

A relação com o cliente não termina na contratação. O app oferece alertas de gastos, notificações de movimentação, acompanhamento de investimentos e histórico financeiro detalhado. Para o microempreendedor, funciona como ferramenta de gestão do negócio: controle de fluxo de caixa, organização de despesas e acompanhamento de recebimentos, eliminando a necessidade de planilhas ou softwares à parte.

**Papel do SI:** o SI transforma padrões de uso em alertas acionáveis (gasto acima do habitual, vencimento de parcela, queda no faturamento mensal do negócio) e consolida dados dispersos em uma visão que o cliente usa para tomar decisões financeiras. O atendimento automatizado resolve dúvidas frequentes sobre os produtos, reduzindo custos de suporte.

**Tipo de ganho:** diferenciação (gestão financeira integrada aos produtos, não oferecida separadamente), redução de custo (automação do atendimento).

---

### 1.2 Atividades de Apoio

#### Infraestrutura da Empresa

A infraestrutura da NovaCred inclui sua arquitetura de computação em nuvem, políticas de segurança, governança de dados e processos de conformidade regulatória.

**Como agrega valor:** garante que todos os serviços funcionem com disponibilidade, segurança e conformidade. Sem infraestrutura confiável, nenhum produto digital funciona.

**Papel do SI:** como a operação é 100% digital, o SI é a própria infraestrutura do negócio. Por ser uma instituição financeira regulada, a governança de dados da NovaCred vai além da LGPD: precisa atender requisitos específicos do Banco Central, como rastreabilidade de operações de crédito, sigilo bancário e auditoria de transações. Informações financeiras sensíveis dos clientes (saldos, histórico de crédito, dados cadastrais) precisam ser armazenadas e compartilhadas segundo essas regras. Políticas de segurança protegem os dados contra acessos indevidos e fraudes. Para a NovaCred, qualquer falha na gestão dessas informações não é apenas um problema técnico, mas uma infração regulatória que pode resultar em sanções do Banco Central.

**Tipo de ganho:** redução de risco (conformidade, segurança, continuidade), redução de custo (gestão eficiente dos recursos de nuvem evita desperdício).

---

#### Gestão de Recursos Humanos

A NovaCred possui equipes de desenvolvimento de software, análise de dados, marketing digital, atendimento ao cliente e gestão de risco. Diferente de uma empresa de tecnologia comum, a NovaCred precisa de profissionais que combinam competência técnica com conhecimento do setor financeiro: analistas de risco de crédito que entendem inadimplência, especialistas em compliance bancário que acompanham regulações do Banco Central, e equipes de dados que sabem interpretar padrões financeiros. Como empresa nativa digital, sua cultura organizacional é orientada a experimentação e agilidade.

**Como agrega valor:** essa combinação de perfis técnicos e financeiros permite tanto inovar rapidamente (cultura ágil) quanto manter conformidade regulatória, algo que empresas puramente de tecnologia não conseguem e que bancos tradicionais fazem com menos agilidade.

**Papel do SI:** a automação de tarefas repetitivas (conciliação, validação documental) libera esses profissionais especializados para atividades analíticas e estratégicas, como calibrar modelos de risco e interpretar mudanças regulatórias. A ausência de legado organizacional, diferente dos bancos tradicionais que enfrentam resistência à mudança em estruturas hierárquicas rígidas, permite que novas tecnologias e processos sejam adotados com menor atrito. Isso exige, porém, investimento contínuo em treinamento para que as equipes acompanhem a evolução tanto das ferramentas de IA e dados quanto das regulações financeiras.

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

**Conexão com Porter:** a hiperpersonalização mitiga a rivalidade ao criar diferenciação difícil de copiar (não basta ter os mesmos produtos, é preciso ter os mesmos dados e modelos calibrados). Também mitiga o poder de barganha dos clientes ao aumentar o custo percebido de troca: quanto mais o cliente usa a plataforma, mais preciso o serviço se torna, e migrar para outro player significa perder essa "inteligência" construída sobre seu perfil.

**Como o SI sustenta:** o SI viabiliza toda a cadeia dado → informação → conhecimento. Dados brutos de transações são transformados em informação contextualizada (padrões de consumo, risco de inadimplência, sazonalidade do faturamento do MEI) e, ao longo do tempo, em conhecimento organizacional incorporado nos modelos de IA. Sem o SI integrando processos, pessoas e tecnologia, esses dados permaneceriam fragmentos isolados sem utilidade para decisão.

**Riscos e trade-offs:** acumular mais dados do cliente para personalização aumenta a superfície de ataque e a responsabilidade sob a LGPD, exigindo investimento contínuo em segurança e conformidade. Há também o risco de viés algorítmico: modelos de IA treinados com dados históricos podem reproduzir padrões de exclusão em vez de incluir perfis subatendidos, o que contraria a proposta de valor da NovaCred. Por fim, manter a infraestrutura de dados integrados (Open Finance + dados internos + modelos de IA) tem custo operacional significativo que precisa ser justificado pelo retorno em retenção e conversão.

---

### Estratégia 2: Plataforma integrada de gestão financeira para MEIs

**O que é:** transformar o aplicativo da NovaCred em uma plataforma completa de gestão financeira para microempreendedores, indo além de conta e crédito para oferecer controle de fluxo de caixa, alertas de recebimentos, organização de despesas e crédito contextualizado ao histórico do negócio.

**Conexão com a Cadeia de Valor:** essa estratégia combina serviços (ferramentas de gestão e controle no app), operações (crédito automatizado ajustado ao fluxo de caixa real do MEI) e marketing/vendas (segmentação específica para um público com dores distintas do consumidor pessoa física).

**Conexão com Porter:** mitiga a ameaça de substitutos ao oferecer uma jornada integrada que nenhum produto isolado (Pix, plataforma de investimento, app de gestão) consegue replicar sozinho. Também cria barreiras contra novos entrantes, pois os dados acumulados sobre o comportamento financeiro dos MEIs ao longo dos cinco anos de operação da NovaCred são um ativo que um entrante novo não possui.

**Como o SI sustenta:** o SI integra dados de recebimentos via Pix, pagamentos com cartão, histórico de crédito e padrões sazonais do negócio para gerar informação útil para decisão (por exemplo, identificar que o faturamento do MEI cai em janeiro e oferecer capital de giro preventivo). O atendimento automatizado (alertas inteligentes, notificações de fluxo de caixa) reduz o custo de suportar essa base de clientes com margens menores.

**Riscos e trade-offs:** o principal risco é de escopo. Tentar ser "tudo para o MEI" (conta, crédito, gestão, pagamentos, contabilidade) pode diluir o foco e aumentar a complexidade operacional, elevando custos de desenvolvimento e suporte. A NovaCred precisa definir até onde vai e o que é melhor resolvido por parceiros via integração. Além disso, parte dos dados usados para contextualizar o crédito do MEI vem de terceiros via Open Finance, cujo acesso depende de regulação que pode mudar. Se o Banco Central alterar as regras de compartilhamento, a base de dados da estratégia pode ser comprometida.

---

## 3. Considerações Finais

A análise da Cadeia de Valor revela que o SI da NovaCred não é uma camada de suporte isolada, mas o elemento que conecta e potencializa todas as atividades da empresa. Desde a oferta dos produtos financeiros (operações) até o atendimento pós-venda (serviços), passando pela distribuição via app (canais) e pela personalização de ofertas (marketing/vendas), cada elo da cadeia depende do SI para funcionar e gerar valor.

As duas estratégias propostas, hiperpersonalização e plataforma para MEIs, são viáveis justamente porque a NovaCred já possui as atividades de apoio necessárias: infraestrutura com governança de dados, equipes com cultura ágil, desenvolvimento tecnológico com modelos de IA que se refinam continuamente e gestão estruturada de fornecedores. Isso não seria possível em uma organização que tratasse SI apenas como "o sistema que roda no computador".

Para que essas estratégias se concretizem, é necessário atenção às três dimensões do SI como sistema sociotécnico:

- **Tecnologia**: manter a arquitetura flexível para integrar novas fontes de dados (Open Finance, Drex) e novos canais (Pix por aproximação).
- **Organização**: governança de dados robusta para garantir conformidade (LGPD, Banco Central) e processos ágeis para lançar funcionalidades rapidamente.
- **Pessoas**: equipes capacitadas para interpretar modelos de IA e traduzir dados em valor para o cliente, além de atendimento preparado para as particularidades do público MEI.
