# SSC0120 — Sistemas de Informação

Repositório da disciplina Sistemas de Informação (ICMC/USP, 2026/1). Contém exercícios, cases e o projeto final.

## Estrutura do repositório

```
sistemas_infor/
├── aulasSI/              # Material das aulas e resumos
├── ex2-fintech/          # Exercício 2 (NovaCred)
├── ex3-vodafone/         # Exercício 3 (Vodafone, ERP)
├── ex_erp/               # Exercício ERP
├── projeto_final/        # (criar quando iniciar o projeto)
├── md2pdf.py             # Script para gerar PDF a partir de Markdown
├── CLAUDE.md             # Instruções para o assistente IA
├── AGENTS.md             # Configuração de agentes
├── README.md             # Este arquivo
└── .claude/
    └── commands/
        └── review.md     # Skill de revisão automatizada
```

## Organização dos cases e exercícios

Cada exercício ou case deve ter seu **próprio folder** na raiz do repositório:

- Incluir o enunciado (PDF) dentro do folder
- Incluir o relatório (.md) e quaisquer arquivos de apoio
- Quando o projeto final for iniciado, criar o folder `projeto_final/`

Exemplos existentes: `ex2-fintech/` (NovaCred, Porter + Cadeia de Valor), `ex_erp/` (exercício sobre ERP).

## Material das aulas

O folder `aulasSI/` contém:

- **PDFs originais** das aulas e capítulos do livro-texto (Laudon, 2014)
- **Resumos em markdown** organizados por área temática, prontos para consulta rápida:

| Arquivo | Conteúdo |
|---|---|
| `01-conceitos-fundamentais-SI.md` | Dado, informação, conhecimento, SI, 3 dimensões, objetivos organizacionais |
| `02-vantagem-competitiva-porter.md` | 5 forças de Porter, cadeia de valor, estratégias competitivas |
| `03-SI-nas-empresas.md` | Tipos de SI (SPT, SIG, SAD, SAE), pirâmide de níveis |
| `04-sistemas-integrados-ERP.md` | ERP, integração, processos de negócio |
| `05-SI-e-mercado.md` | Mercado de TI, dimensões de problemas empresariais |

O arquivo `01-conceitos-fundamentais-SI.md` é base para todos os exercícios.

## Material de IA (Claude Code)

Este repositório é configurado para uso com Claude Code. Três arquivos controlam o comportamento do assistente:

### CLAUDE.md

Guia operacional principal. Define regras de escrita, conceitos obrigatórios, checklists para Porter e Cadeia de Valor, erros comuns a evitar, padrões de escrita anti-IA e o processo de revisão. O Claude lê este arquivo automaticamente ao abrir o projeto.

### AGENTS.md

Configuração de agentes e subagentes. Compartilha as mesmas instruções do CLAUDE.md para manter consistência quando sub-agentes são usados.

### Skill `/review`

Skill de revisão automatizada em `.claude/commands/review.md`. Executa um processo estruturado de 5 passos para revisar relatórios antes da entrega.

**Como usar:**

```
/review path/do/relatorio.md path/do/enunciado.pdf
```

A skill dispara um sub-agente em background que:
1. Analisa o enunciado e extrai requisitos obrigatórios
2. Entende o contexto e case do exercício
3. Lê os resumos das aulas para validar conceitos
4. Avalia o texto em 5 tópicos (completude, conteúdo SI, especificidade, análise crítica, escrita), nota 0-10 cada
5. Retorna score geral e top 3 problemas com sugestões concretas

## Geração de PDF (`md2pdf.py`)

Script reutilizável que converte qualquer relatório em Markdown para PDF, mantendo o padrão visual usado nos exercícios (fonte sans-serif, títulos em negrito preto, parágrafos justificados). Usa as bibliotecas `markdown` (Markdown → HTML) e `PyMuPDF`/`fitz` (HTML → PDF), sem depender de `pandoc` ou de bibliotecas com dependências de sistema.

### Dependências

```bash
pip3 install --index-url https://pypi.org/simple/ markdown pymupdf
```

### Uso

```bash
# saída implícita: relatorio.md → relatorio.pdf
python3 md2pdf.py ex3-vodafone/relatorio.md

# definindo o arquivo de saída
python3 md2pdf.py ex3-vodafone/relatorio.md -o ex3-vodafone/relatorio.pdf
```

### Campos configuráveis

| Opção | Padrão | Descrição |
|---|---|---|
| `-o`, `--output` | mesmo nome do `.md` | Caminho do PDF de saída |
| `--paper` | `a4` | Tamanho da página (`a4`, `letter`, etc.) |
| `--margin` | `50` | Margem em pontos |
| `--font` | `sans-serif` | Família de fonte CSS |
| `--font-size` | `10.5` | Tamanho da fonte do corpo (pt) |
| `--accent` | `#000000` | Cor de títulos e negritos (ex.: `#0a1f44` para azul) |

Exemplo com ajustes:

```bash
python3 md2pdf.py ex3-vodafone/relatorio.md --margin 60 --font-size 11 --accent "#0a1f44"
```

## Fluxo de desenvolvimento

### 1. Preparação

- Criar folder para o exercício
- Colocar o enunciado (PDF) dentro do folder
- Ler o enunciado e identificar requisitos

### 2. Escrita do relatório

- Claude lê o enunciado, os resumos das aulas e o CLAUDE.md
- Escrever o relatório seguindo os templates e checklists do CLAUDE.md
- Iterar sobre o texto, ajustando conceitos, especificidade e escrita

### 3. Revisão

- Rodar `/review` passando o relatório e o enunciado
- O reviewer (sub-agente independente) avalia sem viés de confirmação
- Analisar o feedback, corrigir os problemas identificados
- Rodar `/review` novamente se necessário até o score estar satisfatório

### 4. Entrega

- Verificar padrões de escrita IA (seção 9.1 do CLAUDE.md) uma última vez
- Comparar com exemplos de outros grupos se disponíveis
- Commitar e entregar
