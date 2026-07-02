# Roteiro do Protótipo — Horizonte 360

Blueprint das telas para montagem no **Figma**. O protótipo deve contar **um cenário** (não telas soltas): o percurso de uma solicitação de crédito da cliente Maria, passando pela análise e pelo atendimento, e terminando na visão gerencial da diretoria.

> Lembrete do enunciado: não são aceitos protótipos à mão nem telas individuais. Use Figma (ou Axure, Justinmind, Sketch). As telas devem estar **ligadas por fluxo** (prototype connections), simulando a navegação.

---

## Cenário que o protótipo encena

Maria, microempreendedora individual e cliente há 2 anos, solicita pelo app um limite de crédito para capital de giro. O protótipo mostra:

1. O **analista de crédito** abre a solicitação e vê a **visão única** de Maria e o **painel de decisão** com recomendação e justificativa. Aprova com ajuste de limite.
2. Dias depois, Maria liga em dúvida sobre o valor. O **atendente** abre a **visão de atendimento**, vê o motivo da decisão e explica na hora.
3. A **diretoria** acompanha, no **painel gerencial**, o efeito agregado (tempo médio de decisão, aprovação, inadimplência).

---

## Identidade visual sugerida (para consistência no Figma)

- **Cores:** azul-marinho `#0B2545` (primária), azul `#13315C` (secundária), cinza-claro `#F4F6F8` (fundo), verde `#1B7F5C` (aprovado/positivo), âmbar `#B8860B` (atenção), vermelho `#B00020` (recusado/risco). Use cor com moderação: fundo claro, texto escuro.
- **Tipografia:** uma sans-serif (Inter, Roboto ou similar). Títulos em semibold, corpo regular.
- **Layout base (todas as telas internas):** cabeçalho superior fixo (logo "Horizonte 360" à esquerda, busca por CPF/nome ao centro, perfil do usuário logado à direita) + menu lateral esquerdo (Início, Clientes, Crédito, Atendimento, Painéis, Configurações) + área de conteúdo à direita.
- **Componentes reutilizáveis (crie como *components* no Figma):** cartão de indicador (KPI), chip de status (Aprovado / Em análise / Recusado / Risco médio), linha do tempo (timeline), tabela, botão primário/secundário, avatar do cliente, badge de alerta.

---

## Telas

### Tela 0 — Login / seleção de perfil
- **Usuário:** qualquer colaborador (analista, atendente, gestor).
- **Objetivo:** entrar na plataforma e definir o perfil de acesso (o perfil determina o que cada um vê).
- **Elementos:** logo Horizonte 360 centralizado, campo usuário/senha, botão "Entrar", seletor discreto de perfil (Analista de Crédito · Atendimento · Gestão) apenas para a demonstração do protótipo.
- **Ligação:** ao entrar como **Analista**, vai para a Tela 1.

### Tela 1 — Início / Fila de solicitações (Analista)
- **Usuário:** analista de crédito.
- **Objetivo:** ver as solicitações pendentes e abrir uma.
- **Elementos:** cabeçalho + menu lateral; título "Solicitações de crédito"; tabela com colunas (Cliente, Produto solicitado, Data, Status com chip, Prioridade); barra de busca por CPF; filtro por status; **alerta de pendências** (badge indicando solicitações paradas há mais de X horas).
- **Dado do cenário:** uma linha "Maria S. — Limite de crédito — hoje — Em análise".
- **Ligação:** clicar na linha da Maria abre a Tela 2.

### Tela 2 — Visão Única do Cliente (Cliente 360)
- **Usuário:** analista (e, em outra variação, atendente).
- **Objetivo:** consolidar em uma só tela tudo sobre o cliente.
- **Elementos:**
  - **Cabeçalho do cliente:** avatar, nome (Maria S.), CPF mascarado, cliente desde, chip "Cliente ativo".
  - **Cartões de resumo (KPIs do cliente):** renda estimada, score, produtos contratados, tempo de conta.
  - **Abas ou blocos:**
    - *Cadastro* — dados pessoais, contato, ocupação (MEI), renda declarada.
    - *Produtos* — conta, cartão de débito, eventuais produtos ativos.
    - *Movimentações relevantes* — entradas/saídas recentes, comportamento financeiro (sem detalhar cada transação; é leitura, não processamento).
    - *Histórico de solicitações* — pedidos anteriores e suas decisões, em timeline.
    - *Reclamações / atendimento* — chamados abertos e resolvidos (vindos do CRM).
  - Botão primário: **"Analisar crédito"**.
- **Ligação:** "Analisar crédito" abre a Tela 3.

### Tela 3 — Painel de Decisão de Crédito (Analista)
- **Usuário:** analista de crédito.
- **Objetivo:** apoiar a decisão com dados consolidados + recomendação explicável.
- **Elementos:**
  - **Resumo da solicitação:** produto (limite de crédito), valor pedido.
  - **Coluna de evidências:** renda declarada e estimada, histórico interno de pagamentos (em dia), comportamento financeiro, score, consulta a bureau externo (Serasa/SPC).
  - **Bloco de recomendação (destaque):** chip grande "Recomendação: Aprovar com limite ajustado", **limite sugerido** (ex.: R$ 4.500), e uma **justificativa estruturada** em bullets ("renda compatível", "histórico interno sem atrasos", "score de risco médio").
  - **Ações do analista:** botões "Aprovar", "Aprovar com ajuste", "Recusar" + campo de observação. Deixar visível o texto "A decisão final é do analista".
- **Ligação:** ao "Aprovar com ajuste", mostra confirmação e registra na trilha (Tela 3b opcional). Depois, transição narrativa para o atendimento (Tela 4).

### Tela 3b (opcional) — Confirmação e trilha de decisão
- Modal/tela curta: "Decisão registrada". Mostra quem decidiu, quando, com base em quais dados. Reforça auditoria e conformidade.

### Tela 4 — Visão de Atendimento
- **Usuário:** atendente.
- **Objetivo:** responder à dúvida de Maria com visão completa, sem abrir chamado.
- **Elementos:**
  - Mesmo cabeçalho do cliente (reaproveitar componente da Tela 2).
  - **Resumo da situação:** "Limite de crédito aprovado com ajuste — R$ 4.500".
  - **Motivo da decisão em linguagem clara:** texto amigável explicando por que o limite foi esse (não o jargão do analista).
  - **Próximos passos:** o que Maria pode fazer (aceitar, solicitar revisão), com botões.
  - **Histórico de contatos:** contatos anteriores no CRM.
- **Ligação:** botão "Ver painel gerencial" (transição de papel para a demonstração) abre a Tela 5.

### Tela 5 — Painel Gerencial (Diretoria / BI)
- **Usuário:** diretoria e gerência.
- **Objetivo:** acompanhar o desempenho agregado do crédito e do atendimento.
- **Elementos:**
  - Linha de **KPIs** (cartões): taxa de aprovação, tempo médio de decisão, inadimplência por perfil, tempo médio de atendimento, reclamações recorrentes, rentabilidade por produto.
  - **Gráficos:** série temporal de tempo médio de decisão (mostrando queda após a plataforma), barras de aprovação por perfil de cliente, pizza de motivos de recusa.
  - **Filtros:** período, produto, perfil de cliente.
  - Nota de rodapé: "Dados atualizados automaticamente" (contraste com o processo manual antigo).
- **Ligação:** fecha o fluxo do protótipo.

---

## Fluxo de prototipagem (conexões no Figma)

```
Tela 0 (Login) 
   └─▶ Tela 1 (Fila) 
          └─▶ Tela 2 (Cliente 360) 
                 └─▶ Tela 3 (Decisão de crédito) 
                        └─▶ Tela 3b (Confirmação) 
                               └─▶ Tela 4 (Atendimento) 
                                      └─▶ Tela 5 (Painel gerencial)
```

Configure cada seta como um *prototype link* (on click → navigate to). Assim o avaliador percorre o cenário completo clicando pelas telas.

---

## Checklist de entrega do protótipo

- [ ] Todas as telas seguem o mesmo layout base (cabeçalho + menu + conteúdo).
- [ ] Componentes reutilizados (KPI, chip de status, cliente) são consistentes entre telas.
- [ ] As telas estão ligadas por fluxo clicável (não são imagens soltas).
- [ ] O cenário da Maria é reconhecível do início ao fim.
- [ ] Dados fictícios plausíveis (CPF mascarado, valores realistas).
- [ ] Nada fora de escopo aparece como funcionalidade central (antifraude/segurança não são o foco).
- [ ] Link do Figma com permissão de visualização incluído na entrega.
