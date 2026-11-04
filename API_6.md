# API 6 - Synapse

<p align="center">
  <strong>6º Semestre • 2026-2</strong><br>
  Plataforma inteligente para definição e simulação de regras de comissionamento por texto e voz<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Plataforma%20Web-informational?style=for-the-badge" alt="Plataforma Web">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
  <img src="https://img.shields.io/badge/Foco-IA%20e%20Simula%C3%A7%C3%A3o-success?style=for-the-badge" alt="Inteligência artificial e simulação">
</p>

---

<a id="atalhos"></a>

<br>

## 📌 Atalhos

- [Identificação do projeto](#identificacao-do-projeto)
- [🏢 Empresa parceira](#empresa-parceira)
- [❗ Problema](#problema)
- [✅ Solução](#solucao)
- [📅 Cronograma e entregas](#cronograma-e-entregas)
- [🔗 Link do repositório Git](#link-do-repositorio-git)
- [🖥️ Preview da aplicação](#preview-da-aplicacao)
- [🛠️ Tecnologias utilizadas](#tecnologias-utilizadas)
- [👨‍💻 Contribuições pessoais](#contribuicoes-pessoais)
- [🧠 Hard skills](#hard-skills)
- [🤝 Soft skills](#soft-skills)
- [📚 Aprendizados](#aprendizados)

---

<a id="identificacao-do-projeto"></a>

<br>

## Identificação do projeto

| Item | Descrição |
|---|---|
| Semestre do curso | 6º semestre |
| Ano e semestre | 2026-2 |
| Nome do projeto | Synapse |
| Tipo de sistema | Plataforma web com inteligência artificial e processamento assíncrono |
| Papel no Scrum | Desenvolvedor |
| Atuação técnica | Fullstack: frontend, backend, dados e integração entre serviços |
| Equipe | Titus Systems |
| Público-alvo | Profissionais de recursos humanos, gestores e auditores |
| Situação do projeto | Em desenvolvimento, com entregas incrementais e apresentação final prevista para 03/12/2026 |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | [Dom Rock](https://www.domrock.net/) |
| Pontos focais | Luiz Otavio e Andre Almeida |
| Contexto do desafio | Estruturação de regras de negócio, simulação financeira e rastreabilidade das decisões |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

As regras de negócio de uma empresa mudam com o lançamento de produtos, a revisão de preços, os acordos comerciais e as campanhas de comissionamento. Quando essas regras permanecem dispersas ou dependem do conhecimento de pessoas específicas, aumentam as dificuldades para preservar o histórico, evitar conflitos e compreender o efeito de uma alteração.

O desafio da Dom Rock foi estruturar esse conhecimento e permitir que novas regras fossem definidas de maneira acessível, inclusive por voz. Além de interpretar a solicitação, a solução precisava avaliar seu impacto financeiro antes da aplicação, comparar os resultados com o cenário atual da empresa e oferecer recursos de rastreabilidade e revisão.

No Synapse, trabalhamos com regras de **comissionamento associadas a metas de vendas**. Esse recorte exige atenção aos parâmetros da regra, ao período analisado, aos dados históricos e à diferença entre uma sugestão produzida por inteligência artificial e um resultado financeiro calculado sobre os dados.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **Synapse**, uma plataforma web que recebe propostas de regras de comissionamento por texto ou voz, estrutura seus parâmetros e simula seus efeitos financeiros. O usuário acompanha o processamento, revisa as informações da regra e consulta o resultado em comparação com o **baseline**, que representa o cenário de referência da empresa.

A solução utiliza inteligência artificial para interpretar a solicitação e gerar o código da regra. Esse código é executado em um ambiente isolado, sobre as bases utilizadas na simulação. Os cálculos financeiros são realizados de forma determinística pelo processamento da aplicação, enquanto o modelo de linguagem apoia a interpretação e a geração da lógica.

O fluxo também contempla identificação de conflitos, correção da proposta, avaliação de viabilidade e sugestão de adaptações. As versões das regras, os artefatos do processamento e os resultados são preservados para permitir acompanhamento e consulta posterior.

### Principais funcionalidades

- Autenticação e controle de acesso com Keycloak.
- Entrada de regras de negócio por texto ou gravação de voz.
- Transcrição do áudio em português e extração estruturada dos parâmetros.
- Validação da regra e apresentação de conflitos para correção pelo usuário.
- Geração assistida de código Python para a simulação.
- Execução do código em containers isolados, com controle de recursos e tempo.
- Comparação do comissionamento simulado com o baseline e o orçamento.
- Sugestão de adaptação da regra e de meta de vendas conforme o resultado.
- Acompanhamento do progresso do processamento na interface.
- Histórico de regras, versões e resultados das simulações.
- Relatório de resultados com filtros e detalhamento dos valores.
- Registro de transições, decisões e artefatos para rastreabilidade.

### Arquitetura e integração

Organizamos o projeto em um monorepositório com quatro componentes principais:

| Componente | Tecnologias principais | Responsabilidade |
|---|---|---|
| Frontend | Vue 3, TypeScript, Vite e Pinia | Entrada da regra, correção, acompanhamento do processamento, histórico e resultados |
| API | Java 21 e Spring Boot | Endpoints REST, autenticação, submissões, estado das simulações, eventos SSE e persistência |
| Codegen | Python, LangGraph e Gemini | Extração da regra, validação, geração de código e condução do fluxo de adaptação |
| Worker | Python, RabbitMQ e Docker | Execução isolada do código, cálculo dos resultados e verificação de viabilidade |

A API, o Codegen e o Worker trocam eventos por **RabbitMQ**. Os eventos transportam referências aos artefatos, e o **PostgreSQL** mantém os dados e o histórico necessários ao processamento. O frontend utiliza **REST** para operações e consultas e **Server-Sent Events (SSE)** para receber atualizações do andamento da simulação.

Essa separação permite acompanhar tarefas que demandam mais tempo sem manter uma requisição HTTP aberta durante todo o cálculo. Também delimita as responsabilidades: a API controla o ciclo da simulação, o Codegen produz a lógica assistida por IA e o Worker executa e avalia o resultado.

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Data | Foco da entrega | Situação |
|---|---|---|---|
| Kick-off | 26/08/2026 | Entendimento do desafio e alinhamento com a Dom Rock | Concluído |
| Sprint 1 | 27/09/2026 | Entrada por texto, simulação de viabilidade e histórico dos resultados | Concluída |
| Sprint 2 | 25/10/2026 | Entrada por voz e assistência para adaptação das regras | Concluída |
| Sprint 3 | 22/11/2026 | Auditoria, transparência e validação dos parâmetros | Em desenvolvimento |
| Feira de Soluções | 03/12/2026 | Apresentação final do projeto | Programada |

### Documentação das sprints

- [Sprint 1](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-1.md)
- [Sprint 2](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-2.md)
- [Sprint 3](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-3.md)

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório principal do Synapse](https://github.com/Titus-System/synapse)
- [Frontend](https://github.com/Titus-System/synapse/tree/main/frontend)
- [API](https://github.com/Titus-System/synapse/tree/main/api)
- [Codegen](https://github.com/Titus-System/synapse/tree/main/codegen)
- [Worker](https://github.com/Titus-System/synapse/tree/main/worker)
- [Contratos entre componentes](https://github.com/Titus-System/synapse/tree/main/contracts)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

### Sprint 1 — entrada por texto e simulação

https://github.com/user-attachments/assets/4031c0ad-1c23-4672-8da4-0ac0ffbc73ed

### Sprint 2 — entrada por voz e adaptação de regras

https://github.com/user-attachments/assets/5c50876b-64d8-44c6-9050-4d9dfb758745

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" width="48" height="48" alt="Vue.js" title="Vue.js">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="48" height="48" alt="TypeScript" title="TypeScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" width="48" height="48" alt="Java" title="Java">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/spring/spring-original.svg" width="48" height="48" alt="Spring Boot" title="Spring Boot">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="48" height="48" alt="Python" title="Python">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" width="48" height="48" alt="PostgreSQL" title="PostgreSQL">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/rabbitmq/rabbitmq-original.svg" width="48" height="48" alt="RabbitMQ" title="RabbitMQ">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" width="48" height="48" alt="Docker" title="Docker">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Frontend | Vue 3, TypeScript, Vite e Vue Router | Componentes, telas, navegação e integração com os serviços |
| Estado e apresentação | Pinia e Tailwind CSS | Estado compartilhado, acompanhamento da simulação e estilização |
| API principal | Java 21, Spring Boot, Spring Security e JDBC | Endpoints, autenticação, regras de negócio e acesso aos dados |
| Banco de dados | PostgreSQL e Liquibase | Persistência, histórico, artefatos e evolução do esquema |
| Serviços Python | Python 3.12, SQLAlchemy, asyncpg e Pydantic | Processamento assíncrono, acesso aos dados e validação de estruturas |
| Inteligência artificial | LangGraph, LangChain e Google Gemini | Orquestração do processamento, extração de parâmetros e geração de código |
| Entrada por voz | MediaRecorder e Deepgram | Captura do áudio no navegador e transcrição em português |
| Mensageria | RabbitMQ, Spring AMQP e aio-pika | Troca de eventos e coordenação do processamento entre serviços |
| Atualizações da interface | REST e SSE | Operações do usuário e acompanhamento do andamento da simulação |
| Autenticação | Keycloak, OAuth 2.0, OpenID Connect e JWT | Login, sessão e acesso autenticado à API |
| Execução isolada | Docker e containers efêmeros | Execução controlada do código Python gerado pela IA |
| Contratos | OpenAPI e JSON Schema | Definição e validação das interfaces HTTP, eventos e dados compartilhados |
| Observabilidade | FastAPI, Prometheus, OpenTelemetry e Grafana Alloy | Endpoints operacionais, métricas, logs e coleta de telemetria |
| Testes | Vitest, Vue Test Utils, Pytest, Spring Boot Test e Testcontainers | Verificação de componentes, serviços, integrações e contratos |
| Qualidade e colaboração | ESLint, Oxlint, Ruff, mypy, Bandit, Git e GitHub | Análise de código, tipagem, versionamento e integração do trabalho da equipe |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuo como **desenvolvedor fullstack**, participando da implementação e integração das funcionalidades do Synapse. Minha atuação conecta a experiência do usuário no frontend às regras de negócio, à persistência dos dados e ao processamento realizado pelos serviços do backend.

No frontend, trabalho com **Vue 3 e TypeScript** na construção e integração das telas de entrada de regras, acompanhamento da simulação e consulta aos resultados. Também contribuo com o tratamento de estados de carregamento, erros e atualizações do processamento, buscando apresentar ao usuário informações coerentes com a etapa em que sua solicitação se encontra.

No backend, participo do desenvolvimento e dos ajustes dos fluxos em **Java e Spring Boot**, incluindo endpoints, validações, consultas e integração com o **PostgreSQL**. Essa atuação envolve manter consistência entre os dados enviados pela interface, as regras armazenadas e as respostas disponibilizadas para acompanhamento e histórico.

Na integração com os serviços em **Python**, contribuo para conectar a entrada da regra ao processamento assistido por inteligência artificial e à execução da simulação. O trabalho com **RabbitMQ** e os contratos compartilhados exige atenção aos formatos das mensagens, aos identificadores e às mudanças de estado, para que as etapas sejam acompanhadas corretamente pela aplicação.

Também participo da integração dos recursos de voz e da apresentação dos parâmetros extraídos, considerando a necessidade de revisão e correção pelo usuário. Nos resultados, trabalho com a disponibilização das informações calculadas pelos serviços, preservando a distinção entre a interpretação realizada pela IA e os valores produzidos pela simulação.

Ao longo das sprints, colaboro na validação dos fluxos completos, na investigação de problemas de integração e nos ajustes necessários às entregas. Os principais artefatos da minha atuação incluem componentes de interface, endpoints, regras de validação, consultas, integração de eventos e correções no fluxo entre submissão, processamento, histórico e resultado.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Vue 3 e TypeScript | Sei fazer com autonomia | Desenvolvimento e integração de telas e componentes da aplicação |
| HTML, CSS e Tailwind CSS | Sei fazer com autonomia | Organização visual dos formulários, estados e resultados |
| Pinia e gerenciamento de estado | Sei fazer com autonomia | Acompanhamento das informações da sessão e das simulações |
| Java e Spring Boot | Sei fazer com autonomia | Endpoints, validações e integração das regras de negócio |
| Python | Sei fazer com autonomia | Integração com os serviços de processamento e simulação |
| SQL e PostgreSQL | Sei fazer com autonomia | Consultas, persistência e recuperação do histórico |
| Integração REST e SSE | Sei fazer com autonomia | Envio das operações e atualização do progresso na interface |
| RabbitMQ e processamento assíncrono | Sei fazer com autonomia | Integração do fluxo de eventos e acompanhamento das etapas |
| JSON Schema e contratos de dados | Sei fazer com autonomia | Alinhamento de estruturas entre frontend, API e serviços Python |
| Autenticação e controle de acesso | Sei fazer com autonomia | Integração da sessão com os fluxos protegidos da aplicação |
| Integração com inteligência artificial | Sei fazer com autonomia | Conexão entre entrada da regra, processamento e apresentação dos resultados |
| LangGraph | Faço com ajuda | Acompanhamento e integração das etapas do fluxo assistido por IA |
| Docker | Sei fazer com autonomia | Uso do ambiente em containers e apoio à validação das integrações |
| Testes e depuração | Sei fazer com autonomia | Verificação de fluxos e investigação de falhas entre componentes |
| Observabilidade | Faço com ajuda | Uso de logs e informações de execução para acompanhar o processamento |
| Git e GitHub | Sei fazer com autonomia | Versionamento e colaboração durante as sprints |

</details>

---

<a id="soft-skills"></a>

<br>

## 🤝 Soft skills

<details>
  <summary><strong>Clique para visualizar as soft skills desenvolvidas no projeto</strong></summary>

<br>

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Pensamento analítico | Relacionei os parâmetros informados pelo usuário às etapas necessárias para simular e apresentar o resultado |
| Comunicação técnica | Alinhei estruturas de dados e comportamentos esperados com os integrantes responsáveis pelos diferentes componentes |
| Colaboração | Participei dos ajustes de integração entre frontend, API e serviços de processamento |
| Resolução de problemas | Investiguei falhas considerando o fluxo completo da solicitação, desde a interface até o retorno dos eventos |
| Pensamento crítico | Considerei a necessidade de validar os parâmetros e conferir os resultados antes de apresentá-los como uma regra viável |
| Adaptabilidade | Trabalhei com Vue, Java e Python conforme as necessidades das funcionalidades e integrações |
| Organização | Acompanhei tarefas e dependências para integrar as entregas dentro do planejamento das sprints |
| Responsabilidade | Dei atenção à consistência das informações e à rastreabilidade das operações em uma aplicação que trabalha com simulações financeiras |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O Synapse aprofundou minha compreensão sobre a integração de inteligência artificial em uma aplicação de negócio. Aprendi que interpretar a solicitação do usuário é apenas uma parte do problema: também é necessário validar os parâmetros, controlar o processamento, executar a lógica com segurança e apresentar resultados que possam ser compreendidos e conferidos.

A arquitetura com serviços separados ampliou minha visão sobre processamento assíncrono. O uso de eventos exige atenção ao estado da solicitação, à consistência dos contratos e à recuperação de falhas. Para o usuário, isso precisa se traduzir em uma interface que explique o progresso e permita acompanhar o resultado sem expor a complexidade interna do sistema.

Outro aprendizado importante foi distinguir geração de código e cálculo financeiro. A IA apoia a interpretação e a construção da lógica, enquanto os valores da simulação dependem da execução controlada sobre os dados. Essa separação reforçou meu cuidado com validação, rastreabilidade e revisão humana.

Minha atuação fullstack também fortaleceu a capacidade de transitar entre diferentes tecnologias e entender como uma decisão em uma camada afeta as demais. O projeto conecta conhecimentos desenvolvidos ao longo do curso em interfaces, backend, dados, integração e inteligência artificial, ampliando minha visão sobre a construção de soluções completas para problemas reais.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 5 • SyncDesk](./API_5.md) | — |

</div>
