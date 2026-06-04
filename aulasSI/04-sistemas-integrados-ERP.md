# Sistemas Integrados e ERP

Fontes: Aula 08 (SistemasIntegrados-ERP), Laudon Cap. 9 (Secao 9.1)

---

## Conceitos-chave

### O problema que sistemas integrados resolvem

Sem integracao, uma empresa opera com dezenas (ou centenas) de sistemas e bancos de dados independentes que nao se comunicam. Consequencias:
- Informacoes desatualizadas e inconsistentes entre departamentos.
- Tomada de decisao baseada em relatorios impressos defasados.
- Vendas nao sabe se o produto esta disponivel no estoque.
- Producao nao consegue usar os dados de vendas para planejar.
- Processos redundantes e ineficientes.

### Visao tradicional vs visao integrada

- **Tradicional**: cada area funcional (vendas, producao, financas, RH) possui seu proprio sistema isolado. Dados fragmentados, silos de informacao.
- **Integrada**: um unico sistema com banco de dados centralizado que conecta todas as areas. Quando um processo gera informacao, ela fica imediatamente disponivel para todos os outros processos.

### ERP - Enterprise Resource Planning (Planejamento de Recursos Empresariais)

- Suite de modulos de software integrados com banco de dados central comum.
- Coleta dados das diferentes divisoes e departamentos da empresa.
- Abrange processos de manufatura, producao, financas, contabilidade, vendas, marketing e RH.
- Quando um processo acrescenta nova informacao, ela se torna imediatamente disponivel para outros processos de negocio.

### Software integrado

- Desenvolvido em torno de milhares de processos de negocio predefinidos que refletem as melhores praticas.
- A empresa precisa, antes de tudo, selecionar as funcoes que deseja usar e mapear seus processos de acordo com os processos predefinidos do software.
- Usa tabelas de configuracao para adaptar o sistema a forma de operacao da empresa.
- Customizacao profunda pode prejudicar o desempenho e comprometer a integracao, que e o principal beneficio.

---

## Modelos e frameworks

### Funcionamento do sistema integrado (Laudon, Figura 9.1)

Banco de dados centralizado conecta quatro areas funcionais:

```
        Financas e Contabilidade
        (dinheiro em caixa, contas a receber,
         credito ao cliente, receita)
                    |
  Vendas e          |          Recursos
  Marketing    [BD Central]    Humanos
  (pedidos,         |          (horas trabalhadas,
   previsoes,       |           custo do trabalho,
   devolucoes,      |           requisitos de cargo)
   precos)          |
                    |
        Manufatura e Producao
        (materias-primas, programacoes,
         datas de expedicao, capacidade,
         compras)
```

Exemplo: representante de vendas lanca pedido de rodas. O sistema verifica credito do cliente, programa remessa, identifica rota de expedicao, reserva artigos no estoque. Se estoque insuficiente, programa producao e solicita materiais aos fornecedores. Previsoes de vendas sao atualizadas automaticamente.

### Processos de negocio suportados pelo ERP (Tabela 9.1 do Laudon)

**Financeiros e contabeis**: livro-razao, contas a pagar/receber, ativos fixos, contabilidade de custos, contabilidade tributaria, gerenciamento de credito, relatorios financeiros.

**Recursos humanos**: gestao de pessoal, folha de pagamento, planejamento de forca de trabalho, remuneracao, gestao de desempenho, acompanhamento de candidatos, despesas de viagem.

**Producao e manufatura**: selecao de fornecedores, gestao de estoque, compras, expedicao, planejamento de producao, planejamento de necessidade de materiais, controle de qualidade, manutencao.

**Vendas e marketing**: processamento de pedidos, cotacoes, contratos, configuracao de produtos, precificacao, faturamento, verificacao de credito, comissoes, planejamento de vendas.

---

## Beneficios do ERP

### Integracao
- Integra os sistemas de informacao e as diferentes funcoes do negocio.
- Visao global e unificada dos negocios.

### Controle e automacao
- Maior controle dos processos produtivos e de apoio.
- Automatizacao e maior agilidade nos processos de negocio.
- Ganhos de produtividade e velocidade de resposta.

### Qualidade dos dados
- Padronizacao dos dados e otimizacao do fluxo de informacoes.
- Informacoes mais consistentes e confiaveis.
- Facilitacao do acesso aos dados operacionais.
- Dados com definicoes e formatos comuns em toda a organizacao.

### Estrutura organizacional
- Adocao de estruturas organizacionais mais flexiveis.
- Reducao da complexidade do acompanhamento de producao.
- Mais recursos para planejar, diminuir gastos e repensar a cadeia.

### Tomada de decisao
- Apoio ao processo de tomada de decisao com dados atualizados e integrados.
- A administracao pode descobrir facilmente o desempenho de qualquer unidade a qualquer momento.

### Valor empresarial (Laudon)
- Elevam a eficiencia operacional.
- Ajudam gestores a tomar melhores decisoes.
- Permitem aplicar praticas e dados padronizados globalmente.
- Ajudam a responder rapidamente a pedidos de clientes.
- Producao pode produzir apenas o que foi pedido, comprando a quantidade exata de insumos.

---

## Problemas e desafios do ERP

### Custo e tempo
- Custo alto de implantacao (licencas, consultoria, infraestrutura).
- Tempo longo de implantacao (meses a anos).

### Pessoas e cultura
- Problemas com funcionarios (mudanca cultural e a maior barreira).
- Necessidade de treinamento extensivo.
- Resistencia a mudanca nos processos de trabalho.

### Tecnologia
- Necessidade de infraestrutura adequada.
- Integracao com sistemas legados existentes.
- Testes extensivos antes do go-live.

### Flexibilidade
- Solucao generica: processos predefinidos podem nao se encaixar perfeitamente na empresa.
- Customizacao profunda compromete o principal beneficio (integracao).
- Se a empresa quiser colher os beneficios maximos, precisa mudar sua maneira de trabalhar para se conformar aos processos do software.

---

## Pontos criticos para exercicios e cases

### Distincoes que nao podem ser confundidas

- **ERP != software qualquer**: ERP e um sistema integrado com banco de dados central que conecta todas as areas funcionais.
- **Integracao != automacao**: automacao e tornar processos mais rapidos. Integracao e fazer dados fluirem entre areas sem retrabalho.
- **Customizacao excessiva do ERP e um risco**: quanto mais customiza, mais perde a vantagem da integracao e das melhores praticas embutidas.

### O que a disciplina enfatiza

- A mudanca cultural e tao importante (ou mais) quanto a tecnologia.
- A empresa frequentemente precisa mudar seus processos para se adaptar ao ERP, e nao o contrario.
- Beneficios so se realizam com adocao completa: se um departamento nao usa o sistema, a integracao fica comprometida.
- A dimensao "pessoas" e critica: treinamento, gestao da mudanca, envolvimento dos funcionarios.

### Erros comuns

- Falar de ERP apenas como "software de gestao" sem mencionar o banco de dados central e a integracao.
- Ignorar problemas de implantacao (custo, tempo, resistencia).
- Nao mencionar a necessidade de mudanca nos processos de negocio.
- Esquecer que ERP e uma decisao organizacional, nao apenas tecnologica.

---

## Exemplos da aula e do livro

### Principais fornecedores de ERP
- SAP, Oracle, TOTVS, IBM.
- Versoes sob demanda (fast-start) para pequenas e medias empresas.
- Servicos na nuvem, codigo aberto e plataformas moveis.

### Empresas que usam ERP (mostradas na aula)
UOL, Riachuelo, Mercado Livre, Siemens, Sony, MasterCard, Unibanco, GE, Votorantim, Electronic Arts, Elma Chips, LG, Cisco Systems, CPFL Energia, Pirelli, Portobello, Sebrae SP, Bemol, entre outras.

### Coca-Cola (Laudon)
- Implantou SAP integrado para padronizar e coordenar processos em 200 paises.
- Antes, a falta de integracao impedia de nivelar poder de compra mundial para obter precos mais baixos de materias-primas.

### Alcoa (Laudon)
- Maior produtora mundial de aluminio, com operacoes em 31 paises.
- Antes: sistemas redundantes e ineficientes, cada linha de negocio com seu proprio SI.
- Depois do ERP Oracle: eliminou processos redundantes, reduziu ciclo de aquisicao-pagamento, processamento de contas a pagar caiu 89%, custos mundiais reduzidos em 20%.

### Nvidia (Laudon - caso de abertura Cap. 9)
- Problema: previsao de estoque baseada em planilhas, incapaz de equilibrar oferta e demanda de chips.
- Solucao: SAP APO (Advanced Planning and Optimization) + SAP BusinessObjects para previsao de estoque e dashboards de controle.
- Resultado: taxa de erro de previsao caiu de 5% para 3%, economia de US$ 25 milhoes com estoque de US$ 500 milhoes. Tempo de preparacao de previsao caiu de 140 horas para 30 horas.

### Tasty Baking Company (Laudon)
- Mapeou processos existentes e os transformou nos processos de negocio do SAP ERP.
- Customizou menos de 5% do sistema para obter o maximo de beneficios da integracao.
- SAP possui mais de 3 mil tabelas de configuracao.
