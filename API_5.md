# API 5 - SyncDesk

<p align="center">
  <strong>5º Semestre • 2026-1</strong><br>
  Sistema estruturado para atendimento, triagem e escalonamento de demandas<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Mobile%20e%20Web-informational?style=for-the-badge" alt="Aplicações mobile e web">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge" alt="Projeto concluído">
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
| Semestre do curso | 5º semestre |
| Ano e semestre | 2026-1 |
| Nome do projeto | SyncDesk |
| Tipo de sistema | Plataforma de atendimento com aplicações mobile e web |
| Papel no Scrum | Desenvolvedor |
| Atuação técnica | Fullstack: backend, frontend web, aplicativo mobile e integração entre os componentes |
| Equipe | Titus System |
| Metodologia | Scrum, com sprints, reuniões diárias, revisões e retrospectivas |
| Situação do projeto | Concluído, incluindo as três sprints e a apresentação na Feira de Soluções |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | [Pro4Tech](https://www.linkedin.com/company/pro4tech/) |
| Representantes | Larissa Souza e Rafael Monteiro |
| Contexto do desafio | Atendimento ao cliente, triagem e gestão de demandas |
| Professor P2 | Gerson Penha |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

O atendimento ao cliente precisa conectar a comunicação com o solicitante ao acompanhamento de sua demanda. Sem um fluxo estruturado, torna-se mais difícil recuperar o histórico das interações, identificar o responsável por cada chamado, encaminhar solicitações e acompanhar sua resolução.

O desafio proposto pela Pro4Tech foi desenvolver uma aplicação mobile que centralizasse o atendimento em um sistema de chat, com registro completo das conversas e controle da abertura, do escalonamento e do encerramento dos chamados. A jornada deveria começar por uma triagem automatizada, permitindo identificar a necessidade do cliente antes do atendimento humano.

Além da experiência do solicitante, o projeto precisava atender às necessidades dos atendentes e gestores, oferecendo organização operacional, controle de acesso, acompanhamento de indicadores e avaliação da qualidade do suporte.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **SyncDesk**, uma plataforma que integra um aplicativo mobile para solicitantes, uma aplicação web para atendentes e administradores e uma API central para as regras de negócio e a persistência dos dados.

O cliente inicia o atendimento pelo aplicativo, responde à triagem automatizada e acompanha a conversa e o chamado. Na interface web, os atendentes dão continuidade ao suporte, organizam as solicitações e atualizam sua situação. Os administradores gerenciam usuários, acompanham a operação e consultam os indicadores do sistema.

A comunicação combina **APIs REST** para consultas e operações de negócio com **WebSocket** para o chat em tempo real. O **PostgreSQL** armazena os dados relacionais, enquanto o **MongoDB** mantém as mensagens e as interações das conversas.

### Principais funcionalidades

- Autenticação, recuperação de senha e controle de acesso por perfil.
- Cadastro e gerenciamento de usuários, empresas e produtos.
- Triagem automatizada para identificar a demanda do solicitante.
- Abertura, atribuição, encaminhamento, escalonamento e encerramento de chamados.
- Chat em tempo real entre solicitantes e atendentes.
- Consulta ao histórico e pesquisa de conversas.
- Alertas de novas mensagens e atualizações de chamados.
- Dashboards e indicadores para acompanhamento do atendimento.
- Avaliação da satisfação do cliente após o encerramento.
- Gerenciamento de perfil e configurações de conta.
- Armazenamento de arquivos e integração com envio de e-mails.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| SyncDesk API | Autenticação, regras de negócio, chamados, triagem, conversas, arquivos e persistência |
| SyncDesk Mobile | Acesso do solicitante ao atendimento, aos chamados, ao histórico e ao perfil |
| SyncDesk Web | Operação dos atendentes e administração de usuários, chamados e indicadores |
| SyncDesk Library | SDK compartilhado de integração, desenvolvido por outro integrante da equipe |

As aplicações também possuem tratamento de sessão, estados de carregamento, retorno de erros e atualização das informações. Na interface web, o WebSocket atende à conversa aberta, enquanto a consulta periódica de dados mantém os avisos globais de novas mensagens e alterações nos chamados.

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Data | Principais entregas | Situação |
|---|---|---|---|
| Kick-off | 03/03/2026 | Apresentação do desafio e alinhamento inicial com a empresa parceira | Concluído |
| Sprint 1 | 05/04/2026 | Chat, triagem inicial e gerenciamento do ciclo de vida dos chamados | Concluída |
| Sprint 2 | 03/05/2026 | Recursos administrativos e pesquisa no histórico de conversas | Concluída |
| Sprint 3 | 31/05/2026 | Alertas, dashboards, auditoria e avaliação do atendimento | Concluída |
| Feira de Soluções | 25/06/2026 | Apresentação do projeto e demonstração da solução desenvolvida | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório principal do SyncDesk](https://github.com/Titus-System/SyncDesk)
- [SyncDesk API — backend](https://github.com/Titus-System/syncdesk-api)
- [SyncDesk Mobile — aplicativo](https://github.com/Titus-System/syncdesk-mobile)
- [SyncDesk Web — interface de atendimento e administração](https://github.com/Titus-System/syncdesk-web)
- [SyncDesk Library — biblioteca compartilhada da equipe](https://github.com/Titus-System/syncdesk-library)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir à demonstração da Sprint 1](https://youtu.be/ucNTISGGgis)

A demonstração apresenta a primeira etapa do SyncDesk, com o fluxo inicial de atendimento. Nas sprints seguintes, ampliamos a solução com recursos administrativos, pesquisa de histórico, alertas, indicadores e avaliação do suporte.

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="48" height="48" alt="Python" title="Python">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastapi/fastapi-original.svg" width="48" height="48" alt="FastAPI" title="FastAPI">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" width="48" height="48" alt="PostgreSQL" title="PostgreSQL">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" width="48" height="48" alt="MongoDB" title="MongoDB">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" width="48" height="48" alt="React e React Native" title="React e React Native">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="48" height="48" alt="TypeScript" title="TypeScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" width="48" height="48" alt="Docker" title="Docker">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Backend | Python, FastAPI e Uvicorn | Endpoints, regras de negócio e execução da API |
| Dados relacionais | PostgreSQL, SQLAlchemy Async e Alembic | Persistência, consultas assíncronas e controle das alterações do banco |
| Dados de conversas | MongoDB, Motor e Beanie | Armazenamento e acesso às mensagens e interações |
| Autenticação | JWT, Passlib e Argon2 | Sessões, controle de acesso e proteção das senhas |
| Frontend web | React, JavaScript/JSX, Vite, React Router e Tailwind CSS | Telas administrativas e operacionais, navegação e estilização |
| Estado e consultas web | TanStack React Query, Zustand e Axios | Requisições, cache, estado de autenticação e notificações |
| Aplicação mobile | React Native, Expo, Expo Router, TypeScript e NativeWind | Telas, navegação e experiência de atendimento no aplicativo |
| Sessão e consultas mobile | Expo Secure Store e TanStack React Query | Armazenamento de tokens, consultas e atualização dos dados |
| Comunicação | REST e WebSocket | Integração com o backend e chat em tempo real |
| Arquivos e e-mail | MinIO/S3 e Resend | Armazenamento de arquivos e envio de mensagens por e-mail |
| Observabilidade | Prometheus, Grafana, Loki e Promtail | Métricas, painéis e centralização de logs |
| Testes e qualidade | Pytest, Jest, Ruff, mypy, Bandit, ESLint e Prettier | Testes automatizados, tipagem, análise e padronização do código |
| Ambiente e colaboração | Docker, Docker Compose, Poetry, Node.js, npm, Git e GitHub | Organização do ambiente, dependências e desenvolvimento em equipe |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor fullstack**, contribuindo com o backend, o frontend web e a aplicação mobile. Minha participação envolveu a implementação de funcionalidades e a integração entre as camadas, acompanhando o caminho das informações desde a interação do usuário até seu processamento e armazenamento.

No backend, trabalhei com **Python e FastAPI** na construção e no ajuste de endpoints, validações e regras de negócio relacionadas aos usuários, chamados e atendimentos. Também participei da integração com **PostgreSQL e MongoDB**, considerando a diferença entre os dados relacionais da operação e o histórico das conversas.

Na aplicação web, contribuí com telas e componentes em **React**, consumo de serviços com **Axios**, gerenciamento de consultas e atualização das informações apresentadas ao usuário. Trabalhei na integração dos fluxos de autenticação, gerenciamento de chamados e atendimento, considerando as permissões de cada perfil, os estados de carregamento e o tratamento de erros.

No aplicativo mobile, atuei com **React Native, Expo e TypeScript**, participando da construção e integração das interfaces de acesso, acompanhamento de chamados e comunicação com o suporte. Essa atuação exigiu atenção à navegação, à manutenção da sessão e às diferenças entre o funcionamento no navegador, no emulador e no dispositivo móvel.

Também participei dos ajustes de comunicação em tempo real e da validação dos fluxos entre as interfaces e a API. A integração do chat exigiu alinhar o histórico recuperado por requisições HTTP às novas mensagens recebidas pelo WebSocket, mantendo a experiência de atendimento coerente entre os participantes.

Ao longo das sprints, colaborei na identificação de problemas, nos testes das funcionalidades e na organização das entregas. Os principais artefatos da minha atuação foram endpoints, regras de negócio, componentes de interface, integrações com a API, ajustes de persistência e correções nos fluxos de atendimento. A **SyncDesk Library foi desenvolvida por outro integrante da equipe**; minha contribuição se concentrou nos componentes da aplicação e em sua integração.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Python e FastAPI | Sei fazer com autonomia | Desenvolvimento de endpoints, validações e regras de negócio |
| SQL e PostgreSQL | Sei fazer com autonomia | Consultas e persistência dos dados de usuários e chamados |
| MongoDB | Sei fazer com autonomia | Integração com dados de conversas e histórico de mensagens |
| React e JavaScript | Sei fazer com autonomia | Desenvolvimento e integração das interfaces web |
| React Native, Expo e TypeScript | Sei fazer com autonomia | Construção de telas e consumo de serviços no aplicativo mobile |
| HTML, CSS, Tailwind CSS e NativeWind | Sei fazer com autonomia | Organização visual e adaptação das interfaces web e mobile |
| APIs REST e Axios | Sei fazer com autonomia | Comunicação entre as interfaces e os serviços do backend |
| WebSocket | Sei fazer com autonomia | Integração do envio e recebimento de mensagens em tempo real |
| React Query e gerenciamento de estado | Sei fazer com autonomia | Controle de consultas, carregamento e atualização das telas |
| Autenticação e autorização | Sei fazer com autonomia | Integração de sessão e tratamento das permissões por perfil |
| Testes e depuração | Sei fazer com autonomia | Validação de fluxos e correção de problemas entre frontend e backend |
| Docker e Docker Compose | Sei fazer com autonomia | Execução do ambiente e dos serviços utilizados no desenvolvimento |
| Observabilidade | Faço com ajuda | Consulta a logs e indicadores para apoiar a investigação de problemas |
| Git e GitHub | Sei fazer com autonomia | Versionamento e integração das entregas com a equipe |

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
| Comunicação | Alinhei com a equipe os dados enviados e recebidos pelas interfaces para manter os fluxos de atendimento consistentes |
| Colaboração | Trabalhei em conjunto com outros desenvolvedores na integração entre backend, aplicação web e aplicativo mobile |
| Organização | Dividi as atividades em entregas menores e acompanhei suas dependências durante as sprints |
| Resolução de problemas | Investiguei falhas de integração considerando requisições, sessão, persistência e comportamento das telas |
| Adaptabilidade | Alternei entre tecnologias de backend, web e mobile conforme as necessidades do projeto |
| Atenção à experiência do usuário | Considerei mensagens de erro, carregamento e atualização do chat para tornar o atendimento mais claro |
| Responsabilidade | Validei os fluxos em que atuei antes de integrá-los às entregas da equipe |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O SyncDesk ampliou minha visão sobre desenvolvimento fullstack ao reunir backend, aplicação web e aplicativo mobile em uma mesma solução. Aprendi que uma funcionalidade de atendimento precisa manter consistência em todas essas camadas: a ação realizada em uma interface deve produzir o resultado esperado na API e ser refletida corretamente para os demais usuários.

O trabalho com comunicação em tempo real reforçou a importância de diferenciar o histórico persistido das novas mensagens recebidas durante uma conversa. Também aprofundei meu entendimento sobre estados de conexão, autenticação, atualização de dados e tratamento de falhas, aspectos que influenciam diretamente a experiência de uso.

A utilização de PostgreSQL e MongoDB ajudou a consolidar minha compreensão sobre a escolha de estruturas de armazenamento conforme a necessidade de cada domínio. Ao mesmo tempo, a atuação com React e React Native exigiu adaptar componentes e fluxos às particularidades de cada plataforma.

Concluir as sprints e apresentar o projeto na Feira de Soluções reforçou a importância de integrar o trabalho técnico à organização da equipe e à comunicação do valor da solução. Essa experiência consolidou minha capacidade de contribuir em diferentes partes de um produto, mantendo atenção à funcionalidade completa e ao problema do cliente.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 4 • AdaTech](./API_4.md) | [➡️ API 6 • Synapse](./API_6.md) |

</div>
