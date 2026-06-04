# Sistemas de Informacao nas Empresas

Fontes: Aula 05 (SI-Empresa), Laudon Cap. 2 (secao 2.2)

---

## Conceitos-chave

### Tipos de SI por nivel organizacional

A empresa possui diferentes niveis e cada um demanda sistemas com caracteristicas proprias. A piramide de SI organiza esses tipos:

### SPT - Sistema de Processamento de Transacoes

- **Nivel**: operacional.
- **Usuarios**: gerentes operacionais, funcionarios de linha.
- **Funcao**: monitorar, registrar e processar as transacoes rotineiras e basicas da organizacao (vendas, recebimentos, depositos, folha de pagamento, fluxo de materiais).
- **Caracteristicas**: altamente estruturado, predefinido, dados acessiveis e precisos. Automatiza tarefas repetitivas.
- **Importancia**: se parar por algumas horas, pode causar colapso na empresa e danos a terceiros.
- **Pergunta tipica**: "Quantas pecas ha em estoque?", "O que aconteceu com o pagamento do Sr. Williams?"
- SPTs sao os maiores produtores de informacao que alimentam os outros sistemas.

### STC - Sistema de Trabalhadores do Conhecimento

- **Nivel**: conhecimento.
- **Usuarios**: engenheiros, cientistas, projetistas, analistas.
- **Funcao**: apoiar a criacao e integracao de novos conhecimentos na organizacao.
- **Exemplos**: sistemas CAD/CAM, ferramentas de simulacao e modelagem, plataformas de e-learning.

### SIG - Sistema de Informacoes Gerenciais

- **Nivel**: gerencial.
- **Usuarios**: gerentes de nivel medio.
- **Funcao**: fornecer relatorios periodicos sobre o desempenho da organizacao, permitindo monitorar, controlar e prever.
- **Fonte de dados**: obtidos dos SPTs, comprimidos e resumidos.
- **Caracteristicas**: respostas a perguntas rotineiras e predefinidas. Pouca flexibilidade analitica. Usam rotinas simples (resumos, comparacoes), nao modelos matematicos avancados.
- **Saida**: relatorios periodicos (semanal, mensal) e dashboards.
- **Pergunta tipica**: "Qual o total de vendas por regiao neste trimestre comparado ao planejado?"

### SAD - Sistema de Apoio a Decisao

- **Nivel**: gerencial (mas com enfoque analitico).
- **Usuarios**: gerentes de nivel medio e analistas de negocio ("superusuarios").
- **Funcao**: auxiliar na tomada de decisoes nao rotineiras, problemas unicos e que se alteram com rapidez, para os quais nao existe procedimento totalmente predefinido.
- **Fonte de dados**: informacoes dos SPTs e SIGs + informacoes de fontes externas (valor de acoes, precos de concorrentes, dados de mercado).
- **Caracteristicas**: utilizam modelos analiticos sofisticados. Alguns focam em Big Data para extrair informacoes uteis.
- **Pergunta tipica**: "Qual o impacto no cronograma de producao se dobrarmos as vendas em dezembro?", "O que acontecera com nosso ROI se a fabrica atrasar 6 meses?"

### SAE - Sistema de Apoio ao Executivo

- **Nivel**: estrategico.
- **Usuarios**: gerencia senior, diretores, presidentes.
- **Funcao**: apoiar decisoes nao rotineiras que exigem avaliacao, percepcao e visao de longo prazo. Questoes estrategicas e tendencias.
- **Fonte de dados**: informacoes resumidas dos SIGs e SADs internos + dados de eventos externos (novas leis, novos concorrentes, tendencias de mercado).
- **Caracteristicas**: interface de facil manuseio (dashboards executivos, portais), graficos e dados de diversas fontes consolidados. Filtram e apresentam apenas o mais importante.
- **Pergunta tipica**: "Quais sao as tendencias de custo do setor no longo prazo?", "Quais produtos devemos produzir daqui a 5 anos?", "Em quais regioes expandir?"

---

## Modelos e frameworks

### Piramide dos tipos de SI

```
        SAE        (Estrategico - Gerentes seniores)
       /   \
      SAD    SIG   (Gerencial - Gerentes medios)
     /         \
    STC          (Conhecimento - Trabalhadores do conhecimento)
   /
  SPT              (Operacional - Gerentes operacionais)
```

- Base (SPT): alto volume, dados transacionais, estruturados.
- Topo (SAE): baixo volume, dados agregados e externos, pouco estruturados.

### Inter-relacionamento entre os SIs

- Os SPTs sao os maiores produtores de informacao requerida pelos outros sistemas.
- SIGs adquirem dados resumidos dos SPTs.
- SADs usam dados de SPTs e SIGs + fontes externas.
- SAEs adquirem informacoes resumidas dos SIGs e SADs.
- Na maioria das organizacoes, as ligacoes entre esses tipos sao menos rigidas do que o diagrama sugere.

### Matriz SI por area funcional

Cada area funcional da empresa pode ter todos os niveis de SI. A aula apresenta tabelas detalhadas:

**Manufatura/Producao**
| Nivel | Tipo | Exemplo |
|---|---|---|
| Operacional | SPT | Controle de chao de fabrica, registro de producao, controle de estoque de materias-primas |
| Conhecimento | STC | CAD/CAM para projetos de produtos e otimizacao de processos |
| Gerencial | SIG | Controle de eficiencia de producao por turno, desempenho de maquinas |
| Gerencial | SAD | Previsao de demanda para ajuste de producao |
| Estrategico | SAE | Analise de tendencias de automacao industrial e planejamento de expansao |

**Vendas/Marketing**
| Nivel | Tipo | Exemplo |
|---|---|---|
| Operacional | SPT | Registro de pedidos, emissao de notas fiscais |
| Conhecimento | STC | CRM avancado com machine learning para analise de comportamento |
| Gerencial | SIG | Relatorios de vendas por regiao/cliente, performance de vendedores |
| Gerencial | SAD | Analise de comportamento do consumidor para decisoes de marketing e precos |
| Estrategico | SAE | Analise de tendencias de mercado e previsao de demanda para novos produtos |

**Recursos Humanos**
| Nivel | Tipo | Exemplo |
|---|---|---|
| Operacional | SPT | Folha de pagamento, controle de frequencia |
| Conhecimento | STC | Treinamento corporativo online (e-learning com trilhas de carreira) |
| Gerencial | SIG | Relatorios de desempenho, absenteismo, turnover |
| Gerencial | SAD | Projecao de custos de RH e planejamento de contratacoes |
| Estrategico | SAE | Planejamento estrategico de talentos para os proximos anos |

**Financas/Contabilidade**
| Nivel | Tipo | Exemplo |
|---|---|---|
| Operacional | SPT | Contas a pagar/receber, processamento de faturas |
| Conhecimento | STC | Modelagem financeira para simulacoes de investimentos e riscos |
| Gerencial | SIG | Relatorios financeiros mensais (balanco patrimonial, DRE) |
| Gerencial | SAD | Previsao financeira e analise de viabilidade de investimentos |
| Estrategico | SAE | Analise de fusoes, aquisicoes e investimentos de longo prazo |

---

## Pontos criticos para exercicios e cases

### Distincoes que nao podem ser confundidas

- **SIG != SAD**: SIG responde perguntas rotineiras com relatorios padronizados. SAD lida com problemas unicos, nao rotineiros, usando modelos analiticos.
- **SAD != SAE**: SAD e para gerentes medios com enfoque analitico. SAE e para gerencia senior com enfoque estrategico e de longo prazo.
- **SPT e a base de tudo**: sem SPTs funcionando, os outros sistemas ficam sem dados.
- **SIG nao usa modelos sofisticados**: usa rotinas simples (resumos, comparacoes). Modelos analiticos sao do SAD.
- **SAE incorpora dados externos**: alem de dados internos resumidos, usa informacoes sobre leis, concorrentes, tendencias de mercado.

### Dicas para classificar um SI em exercicio

1. Quem usa? (operador, gerente medio, executivo senior)
2. Que tipo de decisao apoia? (rotineira e estruturada vs nao rotineira e desestruturada)
3. Qual a fonte dos dados? (transacoes internas vs dados externos vs ambos)
4. Qual o horizonte temporal? (diario/semanal vs mensal/trimestral vs anos)
5. A saida e um relatorio padrao ou uma analise ad-hoc?

### Erros comuns

- Confundir SIG com SAD porque ambos sao do nivel gerencial. A diferenca esta no tipo de decisao (rotineira vs nao rotineira) e no uso de modelos analiticos.
- Achar que SAE e so um dashboard bonito. SAE aborda questoes estrategicas de longo prazo.
- Esquecer que SPT e critico para a operacao: uma parada causa danos imediatos.
- Nao perceber que os tipos de SI nao sao rigidamente separados: na pratica, as fronteiras sao fluidas.

---

## Exemplos da aula

### Caso SuperMax Rede de Supermercados (linha do tempo de 1 dia)

A aula apresenta como diferentes SI operam ao longo de um unico dia em uma rede de supermercados:

- **06h00 (SPT)**: Abertura dos CDs, sistema registra entrada e saida de mercadorias, atualiza estoques no sistema central.
- **08h00 (SPT)**: Abertura das lojas, sistema de ponto dos funcionarios, sistema de venda nos caixas registra cada produto vendido.
- **10h00 (SIG)**: Gerentes consultam relatorios automaticos de estoque critico (produtos em falta). Decisao de solicitar reposicao imediata ao CD.
- **12h00 (SIG)**: Dashboard mostra desempenho de vendas da manha. Identificacao de lojas com alta demanda para ajustar promocoes locais.
- **15h00 (STC)**: CRM analisa comportamento de compra da manha e recomenda ajustes na promocao de produtos frescos. Geracao automatica de campanhas relampago via app.
- **17h00 (SAD)**: Simulacao de novos cenarios logisticos para otimizar reabastecimento de lojas com vendas acima do previsto. Escolha do melhor plano de rota.
- **19h00 (SIG)**: Consolidacao de vendas diarias em relatorio preliminar. Avaliacao de picos de vendas e gastos operacionais.
- **21h00 (SAE)**: Diretores acessam dashboards estrategicos. Avaliam tendencias de consumo (ex: alta procura por veganos) para planejar ajustes em fornecedores. Discutem expansao para regioes com crescimento expressivo.

### Exemplos do Laudon Cap. 2

- **SPT de folha de pagamento**: captura dados do cartao de ponto, calcula salario, gera cheques e relatorios para contabilidade e governo.
- **SIG de vendas**: tres SPTs (pedidos, producao, contabilidade) alimentam arquivos do SIG que gera relatorios de vendas reais vs planejadas por produto e regiao.
- **SAD de transporte maritimo**: sistema de estimativa de transporte de cargas usando modelos analiticos com dados de custos, restricoes e historico de frete.
- **Leiner Health Products (SAE)**: CEO com painel digital exibindo capital de giro, contas a receber/pagar, fluxo de caixa e estoque em tempo real.
- **Vail Ski Resorts**: usa RFID, EpicMix e SAS Customer Intelligence para transformar dados de esquiadores em experiencias personalizadas e marketing segmentado.
