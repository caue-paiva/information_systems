# Tema / Cenário: Banco Horizonte

**SSC0120, Sistemas de Informação | Projeto Final**
**Grupo:** Cauê Paiva Lira (14675416) · João Pedro Alves Notari Godoy (14582076) · Letícia Barbosa Neves (14588659) · Pedro Lucas Figueiredo Bahiense (14675458)

---

## Tema

Integração dos sistemas de informação de um banco digital em expansão, com foco na **decisão de concessão de crédito e no atendimento ao cliente**, por meio de uma plataforma de visão única do cliente (Horizonte 360).

## A empresa

O Banco Horizonte é uma instituição financeira digital brasileira de médio porte, fundada há cerca de oito anos. Nasceu com uma proposta simples e pouco burocrática (conta digital gratuita, cartão de débito e transferências pelo app) e, com o crescimento, ampliou o portfólio para cartão de crédito, empréstimos pessoais, antecipação de recebíveis, investimentos de baixo risco e seguros. Hoje reúne cerca de **3 milhões de clientes**, sendo aproximadamente metade ativa todo mês. Seu público é formado por jovens adultos, trabalhadores informais, microempreendedores individuais e pequenos comerciantes que usam o aplicativo como canal principal.

## O contexto do problema

O crescimento acelerado não veio com uma estrutura tecnológica integrada. Os sistemas foram implantados isoladamente, conforme a necessidade surgia:

- **Cadastro de clientes**: desenvolvido internamente nos primeiros anos.
- **Análise de crédito**: contratada de uma empresa terceirizada.
- **Atendimento**: opera sobre um CRM externo.
- **Risco**: trabalha com planilhas e relatórios manuais.

Esses sistemas formam silos que não se comunicam de forma confiável. Isso passou a gerar problemas conforme o volume de clientes e transações cresceu.

## O problema selecionado (delimitado)

Entre os vários desafios do banco, o grupo delimita o foco na **concessão de crédito e no atendimento a dúvidas dela decorrentes**. Quando um cliente pede cartão de crédito ou empréstimo, seus dados passam por cadastro, validação, análise de renda, verificação de histórico e decisão, etapas que hoje não estão conectadas. As consequências são:

1. **Lentidão**: reunir dados manualmente atrasa a aprovação de bons clientes, gera perda de receita e abre espaço para o cliente migrar.
2. **Inconsistência**: decisões baseadas em informação incompleta recusam bons clientes ou aprovam solicitações arriscadas.
3. **Opacidade no atendimento**: o atendente não enxerga o motivo de uma recusa e precisa consultar várias telas ou abrir chamados, aumentando o tempo de resposta e a insatisfação.

O problema também é **organizacional**: comercial quer aprovar mais, risco quer reduzir inadimplência e atendimento precisa explicar decisões, e cada área usa ferramentas e métricas próprias.

**Fora do escopo:** sistema antifraude e segurança, processamento das transações do dia a dia (Pix, pagamentos, cartão) e substituição dos sistemas legados. São frentes que continuam operando e podem ser integradas em fases futuras.

## Por que o problema importa

O setor bancário é competitivo e regulado, e o cliente é cada vez menos fiel. Se o crédito demora ou é negado sem explicação clara, o cliente troca de banco. A decisão de crédito é núcleo de receita, e a qualidade da informação no atendimento sustenta a confiança. Portanto, integrar a informação desses processos deixa de ser tarefa operacional e passa a ter papel estratégico.

## A solução proposta (em alto nível)

**Horizonte 360**: uma plataforma de visão única do cliente que **não substitui** os sistemas existentes. Ela cria uma camada de integração que reúne, em uma interface consolidada, os dados de cadastro, crédito e atendimento necessários para decidir e explicar uma concessão de crédito. Sobre essa base, oferece um painel de apoio à decisão de crédito, uma visão de atendimento com o motivo das decisões e painéis gerenciais com indicadores atualizados.

**Objetivos:** reduzir o tempo de decisão de crédito, aumentar a consistência das decisões, dar ao atendimento visão completa do cliente e substituir a apuração manual de indicadores por informação confiável.
