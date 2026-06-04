# Sistemas de Informação — Guia operacional (CLAUDE)

Este arquivo define como um assistente deve ajudar neste repositório (SSC0120).
Objetivo: produzir respostas e relatórios **bem estruturados**, coerentes com as aulas e sem “chute” genérico.

Use isto como um “prompt permanente” para resolver:
- exercícios (Porter, cadeia de valor),
- dúvidas conceituais,
- relatórios e estudos de caso (ex.: fintechs),
- resumos para prova.

## Material de referência da disciplina

Resumos organizados por área temática estão disponíveis em `aulasSI/`:

- `aulasSI/01-conceitos-fundamentais-SI.md` — dado/informação/conhecimento, SI, 3 dimensões, objetivos organizacionais
- `aulasSI/02-vantagem-competitiva-porter.md` — 5 forças de Porter, cadeia de valor, estratégias competitivas
- `aulasSI/03-SI-nas-empresas.md` — tipos de SI (SPT, SIG, SAD, SAE), pirâmide de níveis
- `aulasSI/04-sistemas-integrados-ERP.md` — ERP, integração, processos de negócio
- `aulasSI/05-SI-e-mercado.md` — mercado de TI, dimensões de problemas empresariais

**Como usar:** leia esses arquivos para contexto on-demand, conforme o assunto do exercício ou caso. O arquivo `01-conceitos-fundamentais-SI.md` é relevante para **todos** os exercícios e casos, pois contém as definições base da disciplina (dado ≠ informação, SI sociotécnico, 3 dimensões). Os demais devem ser lidos conforme o tema (Porter → arquivo 02, tipos de SI → arquivo 03, ERP → arquivo 04).

---

## 1) Regras de ouro (sempre cumprir)

1. **SI é sociotécnico**: toda solução precisa abordar tecnologia + organização + pessoas.
2. **Contexto transforma dado em informação**: não confundir “coletar dados” com “gerar informação útil”.
3. **Começar pelo problema de negócio**: objetivo, restrições e métricas vêm antes da ferramenta.
4. **Justificativa explícita**: para cada afirmação importante, apontar evidência do cenário e o mecanismo.
5. **Evitar generalidades**: em estudo de caso, sempre citar elementos concretos do enunciado.

---

## 2) Conceitos que devem aparecer corretamente (definições úteis)

### 2.1 Dado
- fato bruto, unidade básica, pouca utilidade isolado.
- não tem significado amplo sem contexto.

### 2.2 Informação
- dado organizado/ordenado em um contexto.
- útil para decisão: reduz incerteza.

### 2.3 Conhecimento
- interpretação internalizada (experiência + informação).
- orienta ação e julgamento.

### 2.4 Sistema
- conjunto de partes inter-relacionadas com entradas → processamento → saídas.

### 2.5 Sistema de Informação (SI)
- conjunto integrado de **pessoas**, **processos**, **dados** e **tecnologia**
  que coleta/processa/armazena/distribui informação
  para apoiar operações, gestão, decisões e estratégia.

**Não reduzir** SI a “aplicativo” ou “software”.
**Não confundir** SI com infraestrutura de TI: servidores, nuvem e redes são componentes do SI, não sinônimos.

---

## 3) Exemplos de referência (preferir os citados em aula)

### 3.1 Dado vs informação (exemplo canônico)
- “MANGA / 33 / 4,9” = dados (soltos, sem contexto).
- “Cliente comprou 33 mangas por R$ 4,90” = informação (contexto + significado).

### 3.2 Contexto muda significado
- “manga” (fruta) vs “manga” (camisa).
- “33” (temperatura) vs “33” (idade).

### 3.3 Vantagem competitiva (empresas líderes citadas)
- Amazon (varejo online)
- Walmart (varejo offline)
- Spotify (música online)
- Google (busca na web)

Use esses exemplos como analogia quando precisar ilustrar “vantagem competitiva”.

---

## 4) Checklists obrigatórios em estudos de caso

### 4.1 Dimensões do SI (sociotécnico)
Antes de finalizar uma resposta, confirmar que existe pelo menos 1 parágrafo/bullets para:
- **Tecnologia**: sistemas, dados, integração, infraestrutura.
- **Organização**: processos, políticas, estrutura, governança.
- **Pessoas**: usuários, papéis, incentivos, treinamento, resistência.

### 4.2 Porter — 5 forças
Percorrer sistematicamente:
- rivalidade entre concorrentes
- ameaça de novos entrantes
- poder de barganha dos clientes
- poder de barganha dos fornecedores
- ameaça de substitutos

Para cada força:
- intensidade (baixa/média/alta),
- evidências do cenário,
- como SI mitiga/intensifica (mecanismo).

### 4.3 Cadeia de Valor (Porter)
Localizar impactos em:
- **primárias**: logística interna, operações, logística externa, marketing/vendas, serviços
- **apoio**: infraestrutura, RH, desenvolvimento tecnológico, compras

Se renomear ou adaptar uma atividade ao contexto (ex.: "Logística Externa" → "Canais e Distribuição" para fintech), mencionar o nome original do modelo de Porter e justificar a adaptação.

Sempre declarar o tipo de ganho:
- redução de custo,
- diferenciação,
- coordenação/integração,
- qualidade/tempo,
- redução de risco.

---

## 5) Estruturas prontas de resposta (templates)

### 5.1 Template curto (exercício)
1. Resumo do cenário (5–10 linhas)
2. Objetivo da empresa + restrições
3. Porter (5 forças) com intensidade e justificativa
4. Papel do SI (mitigar/intensificar) por força
5. Conclusão: força mais crítica + 2 ações prioritárias

### 5.2 Template completo (relatório)
1. Introdução e contexto
2. Objetivo do negócio e escopo
3. Mapeamento do processo e atores (texto + bullets)
4. Dados → informação → decisões (o que falta para decidir)
5. Análise do setor (Porter)
6. Diagnóstico interno (cadeia de valor + gargalos)
7. Proposta de SI (funcionalidades, dados, integrações)
8. Impactos organizacionais e plano de adoção (pessoas)
9. Métricas (KPIs) e governança de dados
10. Riscos e trade-offs (segurança, privacidade, dependência)
11. Conclusão (mecanismo de valor e próximos passos)

### 5.3 Template “uma força de Porter” (formato padrão)
Use sempre a mesma estrutura para cada força:
- **Intensidade**: (baixa/média/alta)
- **Evidências do cenário**: (3–6 bullets)
- **Como SI influencia**:
  - Mitigação: (1–3 bullets)
  - Intensificação: (1–3 bullets, se aplicável)
- **Implicação estratégica**: (1 parágrafo curto)

---

## 6) Como “amarrar” SI com vantagem competitiva (mecanismos)

Quando propor SI, sempre explicar o mecanismo, por exemplo:
- **Eficiência**: automação reduz tempo/erro → custo menor.
- **Escala**: sistemas permitem crescer sem crescer proporcionalmente headcount.
- **Personalização**: dados + segmentação → experiência melhor e retenção.
- **Barreiras**: dados históricos, modelos, compliance e integrações → dificultam entrada.
- **Switching cost**: histórico, benefícios, integrações e conveniência → cliente troca menos.
- **Coordenação**: integração reduz atrito entre áreas e entre empresa-parceiros.

Evitar frases vazias do tipo “melhora a competitividade” sem explicar como.

---

## 7) Diagnóstico por perguntas (para começar qualquer caso)

Quando receber um enunciado, fazer perguntas (mesmo que respondendo implicitamente):
- Quem são os clientes e o segmento?
- Qual produto/serviço e qual proposta de valor?
- Onde está o maior custo ou o maior risco?
- Quais são os gargalos do processo (tempo/erro/fraude/retrabalho)?
- Quais dados existem? Quais faltam? Que informação é necessária para decidir?
- Quais parceiros e dependências externas existem?
- Qual o ponto regulatório/compliance mais relevante?

---

## 8) Erros comuns (evitar explicitamente)

- Propor tecnologia sem:
  - explicar impacto no processo,
  - lidar com pessoas (treino/resistência),
  - medir resultado (KPIs).
- Confundir “coletar dados” com “gerar informação útil”.
- Definir Porter e parar na definição (sem evidência do caso).
- Não justificar intensidade (baixa/média/alta) com o cenário.
- Não citar trade-offs (segurança, privacidade, dependência, custo).
- Ignorar fornecedores/parceiros (ex.: cloud, bandeiras, reguladores) em setores como financeiro.
- Escrever “Papel do SI” como se fosse vantagem de tecnologia (APIs, microsserviços, nuvem). O foco deve ser: como dados viram informação para decisão, quem usa essa informação e como o processo muda.
- Omitir subseções exigidas pelo enunciado para “variar a escrita”. Ler o enunciado e listar os requisitos por atividade antes de começar.

---

## 9) Heurísticas para escrever melhor (clareza e nota)

- Preferir bullets com substantivos concretos (“parcerias com cloud e bandeiras”) em vez de adjetivos (“muito competitivo”).
- Sempre fechar cada seção com “implicação”: o que isso significa para estratégia e SI.
- Repetir a estrutura por força (padronização ajuda correção e leitura).
- Manter coerência de termos: “dado” ≠ “informação”.
- Estrutura repetida entre seções **não é formulaico** quando o enunciado a exige. Se o exercício pede “como agrega valor” e “papel do SI” para cada atividade, repetir essas subseções é seguir o exercício. O que deve variar é o conteúdo e a abertura dentro de cada subseção.

### 9.1) Padrões de escrita a evitar (remetem a texto gerado por IA)

1. **Travessão (— ou --) no lugar de vírgula.** Usar vírgula para intercalações e pausas, não travessão.
2. **Ponto e vírgula (;) no lugar de ponto final.** Preferir frases mais curtas com ponto final em vez de encadear com ponto e vírgula.
3. **Enumerações sempre com exatamente 3 itens.** Variar a quantidade: às vezes 2, às vezes 4, conforme o conteúdo exigir.
4. **Fórmula “Você pode achar X, mas na verdade Y”.** Evitar construções retóricas que antecipam e corrigem o leitor. Ir direto ao ponto.

---

## 10) Regras de formatação para entregas

- Usar títulos e subtítulos.
- Não deixar parágrafos longos demais (máx. 6–8 linhas).
- Em Porter, uma seção por força.
- Em propostas de SI, separar:
  - funcionalidades,
  - dados,
  - integrações,
  - impactos e KPIs,
  - riscos.

---

## 11) Processo de revisão antes da entrega

Use a skill `/review` para executar o processo abaixo automaticamente. Exemplo: `/review path/do/relatorio.md path/do/enunciado.pdf`

A revisão é executada por um **sub-agente em background**, sem acesso ao contexto do chat principal. O sub-agente recebe apenas: o path do arquivo a revisar, o path do enunciado, os paths do material das aulas e as instruções abaixo. Isso evita viés de confirmação.

### Passo 1 — Análise do enunciado (fonte da verdade)

Ler o enunciado por completo e destilar:
- **Requisitos obrigatórios**: seções, subseções e elementos que a resposta deve ter. Lista exaustiva, item por item. Essa lista é a fonte da verdade da revisão.
- **Elementos que elevam nota**: observações do enunciado (ex.: "demonstre análise crítica", "evite respostas genéricas") que não são seções obrigatórias mas diferenciam a entrega.

### Passo 2 — Compreensão do contexto e case

Entender a fundo o cenário do exercício:
- Empresa, setor, produtos/serviços, público-alvo, desafios de negócio.
- Stakeholders, parceiros, reguladores, concorrentes.
- Cruzar o que é pedido (passo 1) com o contexto: para cada requisito, quais elementos concretos do cenário devem aparecer na resposta?

### Passo 3 — Material da disciplina

Ler os resumos em `aulasSI/` (arquivos .md). **Sempre** ler `aulasSI/01-conceitos-fundamentais-SI.md` (contém as definições base usadas em todos os exercícios). Ler os demais conforme o tema do exercício (Porter → `02-vantagem-competitiva-porter.md`, tipos de SI → `03-SI-nas-empresas.md`, ERP → `04-sistemas-integrados-ERP.md`).
- Identificar quais conceitos da disciplina o exercício exige.
- Verificar definições, modelos e exemplos usados nas aulas para validar se o relatório os aplica corretamente.
- O contexto do modelo (LLM) não é suficiente como fonte. O reviewer deve ler os arquivos.

### Passo 4 — Avaliação por tópicos (nota 0-10 cada)

Para cada tópico, o reviewer analisa o texto, dá a nota, lista pontos positivos, problemas encontrados (com número de linha) e sugestões concretas.

**Tópico 1: Completude (requisitos do enunciado)**
- Todas as seções e subseções exigidas estão presentes?
- Falta algum elemento explicitamente pedido?
- Avaliação binária por item: tem ou não tem.

**Tópico 2: Conteúdo de SI (alinhamento com a disciplina)**
- Conceitos usados corretamente? (dado ≠ informação ≠ conhecimento, SI sociotécnico, SI ≠ software/infraestrutura de TI)
- "Papel do SI" fala de gestão de dados/informação/decisão/pessoas ou de tecnologia genérica (APIs, nuvem, microsserviços)?
- As 3 dimensões (tecnologia, organização, pessoas) aparecem?
- Verificar contra o material das aulas (passo 3).

**Tópico 3: Especificidade ao cenário**
- Usa elementos concretos do enunciado (empresa, produtos, público, parceiros, regulação)?
- As respostas são específicas do caso ou poderiam descrever qualquer empresa?
- Cada afirmação importante tem evidência do cenário?

**Tópico 4: Análise crítica**
- Explica mecanismos (como e por quê) ou apenas afirma resultados?
- Aponta limitações, riscos ou trade-offs?
- Demonstra julgamento próprio sobre o cenário?

**Tópico 5: Escrita**
- Texto claro, fluido, parágrafos com tamanho adequado?
- Padrões de escrita IA ausentes? (ver seção 9.1)
- Conteúdo dentro das subseções variado (aberturas e exemplos diferentes entre seções)?
- Estrutura repetida entre seções **não é problema** quando o enunciado a exige.

### Passo 5 — Resultado final

- Score geral (média dos tópicos).
- Top 3 problemas em ordem de prioridade, com sugestão de correção concreta.
- Indicar se o relatório está pronto para entrega ou se precisa de mais uma rodada.

