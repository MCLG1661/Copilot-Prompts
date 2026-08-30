# 🧭 Mentor de Carreira em Tecnologia

*Protótipo de sistema multiagente baseado em Prompt Engineering para apoiar a exploração e o planejamento de carreiras em tecnologia.*

![Prompt Engineering](https://img.shields.io/badge/AI-Prompt%20Engineering-8A2BE2)
![AI Agents](https://img.shields.io/badge/AI-Agent%20Design-412991)
![Generative AI](https://img.shields.io/badge/Generative%20AI-Career%20Mentor-6C63FF)
![GitHub Copilot](https://img.shields.io/badge/GitHub-Copilot-000000?logo=githubcopilot&logoColor=white) 
![DIO](https://img.shields.io/badge/DIO-CI%26T%20Bootcamp-5A0FC8)
![Status](https://img.shields.io/badge/Status-Protótipo-blue)

---

## 🎯 Visão Geral

O **Mentor de Carreira em Tecnologia** é um projeto de Inteligência Artificial Generativa que explora a divisão de um problema complexo entre **dois agentes especializados**.

O sistema foi concebido para transformar uma conversa inicial sobre experiência, competências, interesses e objetivos profissionais em um **perfil estruturado** e, posteriormente, em recomendações e um roadmap de desenvolvimento.

O fluxo é dividido em duas responsabilidades:

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

> **Importante:** nesta versão, o workflow entre os agentes é conceitual. Não existe ainda uma aplicação que automatize a execução e o handoff entre os agentes.

---

## 💡 Problema

Escolher uma trajetória em tecnologia pode ser difícil quando diferentes fatores precisam ser considerados simultaneamente:

- experiência profissional anterior;
- conhecimentos técnicos;
- competências transferíveis;
- interesses;
- disponibilidade para estudo;
- objetivos profissionais;
- lacunas de conhecimento.

Em vez de utilizar um único prompt para executar todo o processo, o projeto separa o problema em **duas etapas especializadas**.

---

## 🤖 Arquitetura Multiagente

### Agente 1 — Entrevistador de Carreira

Responsável pela etapa de descoberta.

Seu objetivo é conduzir uma entrevista estruturada e transformar as respostas em um perfil profissional organizado.

```text
Perguntar → Explorar → Identificar → Estruturar
```

Principais dimensões analisadas:

- experiência profissional;
- conhecimentos técnicos;
- interesses;
- objetivos;
- disponibilidade;
- pontos fortes;
- lacunas de competências.

📄 [Ver prompt do Agente 1](prompts/AGENTE-1-Entrevistador-de-Carreira.md)

---

### Agente 2 — Planejador de Carreira

Recebe o perfil estruturado produzido na etapa anterior e utiliza esse contexto para analisar possíveis trajetórias.

```text
Analisar → Priorizar → Recomendar → Planejar
```

Entre suas responsabilidades estão:

- avaliar aderência a diferentes carreiras;
- priorizar alternativas;
- justificar recomendações;
- identificar competências a desenvolver;
- estruturar um roadmap;
- sugerir projetos de portfólio;
- apoiar preparação profissional.

📄 [Ver prompt do Agente 2](prompts/AGENTE-2-Planejador-de-Carreira.md)

---

## 🔄 Handoff de Contexto

Um dos conceitos centrais do projeto é a passagem de contexto entre agentes.

O primeiro agente não entrega apenas uma resposta textual genérica. Ele organiza as informações relevantes para que possam funcionar como entrada da próxima etapa.

```text
ENTREVISTA
    │
    ▼
PERFIL ESTRUTURADO
    │
    ▼
HANDOFF
    │
    ▼
PLANEJAMENTO
```

Essa abordagem demonstra como a **separação de responsabilidades** pode tornar workflows baseados em LLMs mais claros e controláveis.

---

## 🧪 Demonstração Completa

O repositório inclui uma simulação fictícia de ponta a ponta mostrando:

1. perfil inicial;
2. entrevista;
3. saída estruturada do Agente 1;
4. handoff;
5. análise do Agente 2;
6. alternativas de carreira;
7. recomendação principal;
8. roadmap de 120 dias;
9. projeto de portfólio;
10. preparação para entrevistas.

➡️ **[Ver demonstração completa do fluxo multiagente](examples/demo-fluxo-completo.md)**

A demonstração é fictícia e possui finalidade exclusivamente educacional.

---

## 🧠 Conceitos Aplicados

O projeto explora conceitos relacionados à construção de soluções com IA Generativa:

### Prompt Engineering

Definição estruturada de:

- papel do agente;
- objetivo;
- contexto;
- instruções;
- restrições;
- formato esperado de saída.

### Agent Design

Divisão do problema entre agentes com responsabilidades específicas.

### Context Engineering

Organização das informações relevantes para utilização pela etapa seguinte.

### Structured Outputs

Transformação de uma conversa em uma representação estruturada e reutilizável.

### Handoff

Transferência do resultado de um agente para outro dentro de um workflow.

### Decomposição de Tarefas

Separação de um problema amplo em etapas menores e especializadas.

---

## 📂 Estrutura do Repositório

```text
Mentor-de-Carreira/
│
├── prompts/
│   ├── AGENTE-1-Entrevistador-de-Carreira.md
│   └── AGENTE-2-Planejador-de-Carreira.md
│
├── examples/
│   └── demo-fluxo-completo.md
│
└── README.md
```

### `prompts/`

Contém as instruções dos dois agentes.

### `examples/`

Contém uma demonstração fictícia do funcionamento completo do workflow.

---

## ▶️ Como Explorar o Projeto

Como esta versão é baseada em Prompt Engineering e não possui uma aplicação automatizada, os prompts podem ser estudados ou testados individualmente em um modelo de linguagem compatível.

Fluxo conceitual:

```text
1. Executar o prompt do Agente 1
              ↓
2. Realizar a entrevista
              ↓
3. Obter o perfil estruturado
              ↓
4. Fornecer o perfil ao Agente 2
              ↓
5. Gerar análise e planejamento
```

Para compreender o comportamento esperado sem executar os prompts, consulte a **demonstração completa** disponível em `examples/`.

---

## 🚀 Possível Evolução

Uma próxima versão poderia transformar o protótipo em uma aplicação automatizada:

```text
Interface
    ↓
Agente Entrevistador
    ↓
Structured Output
    ↓
Orquestração
    ↓
Agente Planejador
    ↓
Roadmap
```

Possíveis evoluções incluem:

- interface web;
- integração com API de LLM;
- automação do handoff;
- persistência do perfil;
- histórico de sessões;
- geração estruturada de roadmap;
- exportação do plano;
- acompanhamento da evolução do usuário.

---

## ⚠️ Limitações

Este projeto possui finalidade **educacional e experimental**.

As recomendações produzidas por modelos de linguagem:

- não constituem avaliação profissional definitiva;
- não substituem orientação especializada;
- podem conter erros ou vieses;
- dependem da qualidade das informações fornecidas;
- não garantem contratação, transição profissional ou resultados específicos.

O projeto deve ser entendido como uma demonstração de **arquitetura de prompts e workflow com agentes**, e não como um serviço profissional automatizado de orientação de carreira.

---

## 🎓 Contexto

Projeto desenvolvido no contexto do **Bootcamp CI&T — Do Prompt ao Agente**, em parceria com a **DIO**, explorando a aplicação prática de Prompt Engineering e construção conceitual de agentes de IA.

O projeto foi posteriormente organizado e documentado como case de portfólio.

---

## 👨‍💻 Autor

**Marcus Guedes**

Projetos em **Data Analytics, Inteligência Artificial aplicada a Negócios, Gestão e Tecnologia**.

- [GitHub](https://github.com/MCLG1661)
- [LinkedIn](https://www.linkedin.com/in/marcusguedes/)

---

## 📌 Status

**Protótipo conceitual concluído.**

A arquitetura, os prompts e o fluxo demonstrativo estão documentados. A automação entre os agentes permanece como possibilidade de evolução futura.
