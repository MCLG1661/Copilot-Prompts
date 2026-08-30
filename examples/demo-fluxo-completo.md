# 🧪 Demonstração do Fluxo Multiagente

Este documento apresenta uma **simulação fictícia** do funcionamento do Mentor de Carreira em Tecnologia.

O objetivo é demonstrar como os dois agentes especializados trabalham em sequência:

```text
Usuário
   ↓
Agente 1 — Entrevistador de Carreira
   ↓
Perfil Profissional Estruturado
   ↓
Handoff de Contexto
   ↓
Agente 2 — Planejador de Carreira
   ↓
Recomendações + Roadmap
```

> **Nota:** este exemplo é demonstrativo. O perfil, as respostas e as recomendações abaixo são fictícios e foram criados exclusivamente para ilustrar a arquitetura do projeto.

---

## 👤 Cenário

Uma profissional da área administrativa deseja avaliar possibilidades de transição para tecnologia.

### Informações iniciais

- **Área atual:** Administração
- **Experiência:** 5 anos
- **Objetivo:** transição para tecnologia
- **Conhecimento técnico:** iniciante
- **Interesses:** dados, automação e Inteligência Artificial
- **Disponibilidade para estudo:** 6 horas por semana
- **Horizonte:** até 12 meses

---

# 1️⃣ Agente Entrevistador

O primeiro agente é responsável pela **descoberta e estruturação do perfil profissional**.

Ele não deve definir imediatamente uma carreira. Sua função principal é coletar contexto suficiente para que a etapa seguinte possa realizar uma análise mais fundamentada.

## Exemplo de entrevista

**Agente:** Qual é sua experiência profissional atual?

**Usuária:** Trabalho há cinco anos na área administrativa. Utilizo planilhas, preparo relatórios e acompanho alguns indicadores da operação.

---

**Agente:** O que desperta seu interesse em tecnologia?

**Usuária:** Gosto de trabalhar com dados e tenho interesse em entender como automação e Inteligência Artificial podem ser aplicadas às empresas.

---

**Agente:** Você possui experiência com programação ou ferramentas de dados?

**Usuária:** Tenho conhecimentos básicos de Python e Power BI adquiridos em cursos online. Também utilizo Excel e Google Sheets.

---

**Agente:** Quanto tempo consegue dedicar ao desenvolvimento profissional?

**Usuária:** Aproximadamente seis horas por semana.

---

**Agente:** Qual é seu principal objetivo?

**Usuária:** Quero migrar para uma função em tecnologia que também aproveite minha experiência de negócio.

---

## 📋 Saída do Agente 1

Ao finalizar a entrevista, o agente transforma a conversa em uma estrutura que poderá ser utilizada pelo próximo agente.

```text
PERFIL PROFISSIONAL ESTRUTURADO

Experiência atual:
Área administrativa, com experiência em relatórios,
planilhas e acompanhamento de indicadores.

Nível técnico:
Iniciante.

Conhecimentos atuais:
- Excel
- Google Sheets
- Power BI básico
- Python básico

Interesses:
- Data Analytics
- Business Intelligence
- Automação
- Inteligência Artificial aplicada a negócios

Disponibilidade:
6 horas por semana.

Objetivo:
Realizar transição para tecnologia em até 12 meses.

Preferências:
Funções que combinem tecnologia, análise e visão de negócio.

Pontos fortes:
- Experiência empresarial
- Familiaridade com indicadores
- Organização
- Pensamento analítico

Lacunas identificadas:
- SQL
- Python aplicado à análise de dados
- Estatística
- Projetos práticos
- Portfólio técnico
```

---

# 2️⃣ Handoff de Contexto

O resultado estruturado do primeiro agente passa a ser a entrada do segundo.

```text
Agente Entrevistador
        │
        ▼
Perfil Profissional Estruturado
        │
        ▼
Handoff de Contexto
        │
        ▼
Agente Planejador
```

Essa separação evita que o segundo agente precise reconstruir todo o histórico da conversa.

Cada agente recebe uma responsabilidade específica dentro do workflow.

---

# 3️⃣ Agente Planejador

O segundo agente recebe o perfil estruturado e avalia possíveis trajetórias profissionais.

## 🥇 1. Analista de Dados

**Aderência: Alta**

Principais motivos:

- aproveita a experiência anterior com indicadores;
- permite combinar conhecimento de negócio e tecnologia;
- apresenta uma trajetória progressiva de desenvolvimento técnico;
- cria fundamentos úteis para futuras especializações em IA.

---

## 🥈 2. Business Intelligence Analyst

**Aderência: Alta**

Principais motivos:

- forte relação com indicadores e relatórios;
- aproveitamento do conhecimento inicial de Power BI;
- conexão direta entre dados e tomada de decisão;
- possibilidade de aproveitar experiência empresarial anterior.

---

## 🥉 3. Analista de Automação e IA aplicada a negócios

**Aderência: Média**

Principais motivos:

- alinhamento com o interesse em Inteligência Artificial;
- possibilidade de trabalhar com melhoria e automação de processos;
- aproveitamento da experiência de negócio.

Entretanto, essa trajetória exigiria maior desenvolvimento técnico antes de uma transição direta.

---

# 🎯 Recomendação Principal

## Analista de Dados

Entre as possibilidades analisadas, a carreira de **Analista de Dados** apresenta uma combinação favorável entre:

```text
Experiência profissional
        +
Conhecimentos atuais
        +
Interesses
        +
Disponibilidade
        +
Competências a desenvolver
```

A estratégia proposta é utilizar a experiência empresarial existente como diferencial enquanto as competências técnicas são desenvolvidas progressivamente.

---

# 🗺️ Roadmap de 120 dias

## Dias 1–30 — Fundamentos de Dados

### Objetivos

- fundamentos de SQL;
- revisão de estatística;
- aprofundamento em Excel;
- fundamentos de análise de dados.

### Entregável

Uma pequena análise exploratória documentada.

---

## Dias 31–60 — Python para Análise

### Objetivos

- Python;
- Pandas;
- NumPy;
- tratamento de dados;
- análise exploratória;
- visualização.

### Entregável

Projeto de análise de dados em Python publicado no GitHub.

---

## Dias 61–90 — Business Intelligence

### Objetivos

- Power Query;
- modelagem de dados;
- DAX;
- dashboards;
- definição de KPIs;
- storytelling com dados.

### Entregável

Dashboard executivo acompanhado de análise dos indicadores.

---

## Dias 91–120 — Portfólio e Mercado

### Objetivos

- organizar GitHub;
- documentar projetos;
- revisar LinkedIn;
- estudar cases de negócio;
- praticar entrevistas;
- iniciar candidaturas direcionadas.

### Entregável

Portfólio com pelo menos três projetos documentados.

---

# 💻 Projeto de Portfólio Sugerido

## Customer Performance Analytics

### Problema

Uma empresa possui dados de clientes e vendas, mas precisa compreender melhor o comportamento e o desempenho de sua base.

### Proposta

Construir uma análise que contemple:

- tratamento dos dados;
- análise exploratória;
- definição de KPIs;
- segmentação;
- dashboard;
- identificação de padrões;
- recomendações de negócio.

### Tecnologias sugeridas

```text
Python
Pandas
SQL
Power BI
GitHub
```

### Competências demonstradas

- Data Analytics;
- Business Intelligence;
- tratamento de dados;
- visualização;
- análise de indicadores;
- comunicação de insights;
- visão de negócio.

---

# 🎤 Preparação para Entrevistas

O planejamento também pode incluir questões para desenvolvimento e preparação profissional:

1. Como você utilizaria dados para apoiar uma decisão de negócio?
2. Qual é a diferença entre análise descritiva e análise preditiva?
3. Como você trataria valores ausentes em um dataset?
4. Para que serve um `JOIN` em SQL?
5. Como você definiria os principais KPIs de um dashboard?
6. Conte um exemplo em que dados ajudaram você a compreender um problema.

---

# 📊 Resultado Esperado do Plano

Ao final do ciclo proposto, o perfil poderia ter desenvolvido:

```text
SQL
 +
Python para Dados
 +
Business Intelligence
 +
Projetos práticos
 +
GitHub estruturado
 +
Posicionamento profissional
```

O roadmap representa uma **estrutura de desenvolvimento**, e não garantia de contratação ou transição profissional.

---

# 🧠 O que o exemplo demonstra

A arquitetura distribui responsabilidades entre os agentes.

### Agente 1 — Entrevistador

```text
Pergunta → Descobre → Organiza → Estrutura
```

### Agente 2 — Planejador

```text
Analisa → Prioriza → Recomenda → Planeja
```

A saída estruturada do primeiro agente funciona como contexto de entrada para o segundo.

Isso demonstra, de forma conceitual, a aplicação de:

- **Prompt Engineering**
- **AI Agent Design**
- **Context Engineering**
- **Handoff entre agentes**
- **Decomposição de tarefas**
- **Structured Outputs**
- **Decision Support**

---

## ⚠️ Limitações

O Mentor de Carreira é um protótipo educacional de apoio à reflexão e ao planejamento.

As recomendações produzidas por modelos de IA:

- não constituem avaliação profissional definitiva;
- não substituem orientação especializada;
- não garantem adequação a determinada carreira;
- não garantem contratação ou resultados profissionais;
- dependem da qualidade e completude das informações fornecidas.

Nesta versão, o fluxo entre os agentes é **conceitual e não automatizado por software**.
 
