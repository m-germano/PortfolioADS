# API 5 - SyncDesk

<p align="center">
  <strong>5º Semestre • 2026-1</strong><br>
  Sistema estruturado para atendimento, triagem e escalonamento de demandas<br>
  Papel exercido no Scrum: <strong>Desenvolvedor (Dev Team)</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Mobile%20e%20Web-informational?style=for-the-badge" alt="Aplicações mobile e web">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
  <img src="https://img.shields.io/badge/Foco-Atendimento%20e%20Integra%C3%A7%C3%A3o-success?style=for-the-badge" alt="Atendimento e integração">
</p>

> **Documentação para o TG II:** o contexto, as funcionalidades e as tecnologias abaixo se baseiam no README do SyncDesk fornecido para esta atualização. O papel de desenvolvedor está registrado na composição da equipe. As entregas individuais, a autoavaliação e os aprendizados pessoais estão sinalizados para preenchimento pelo aluno.

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
| Tipo de sistema | Aplicação mobile para solicitantes, aplicação web para atendentes e administradores e backend compartilhado |
| Papel no Scrum | Desenvolvedor (Dev Team), conforme a lista de integrantes do projeto |
| Equipe | Titus System |
| Método de trabalho | Scrum, com sprints de 21 dias, reuniões diárias, revisões e retrospectivas |
| Situação documentada | Três sprints e todos os itens do backlog registrados como concluídos; o cabeçalho do README ainda informa “Em Desenvolvimento” |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | [Pro4Tech](https://www.linkedin.com/company/pro4tech/) |
| Representantes | Larissa Souza e Rafael Monteiro |
| Contexto do desafio | Centralização e acompanhamento do atendimento ao cliente |
| Professor P2 | Gerson Penha |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

O desafio proposto pela Pro4Tech foi organizar o atendimento ao cliente em um fluxo que permitisse registrar as interações e acompanhar cada solicitação desde a triagem inicial até o encerramento. A solução precisava reunir conversas, histórico e gestão dos chamados, permitindo o escalonamento das demandas e maior controle sobre a operação de suporte.

A jornada deveria começar por uma **triagem automatizada**, capaz de coletar informações iniciais e orientar o atendimento. Além de facilitar a comunicação entre solicitantes e atendentes, o projeto deveria oferecer recursos gerenciais para acompanhar o desempenho da operação e a satisfação dos clientes.

---

<a id="solucao"></a>

<br>

## ✅ Solução

O **SyncDesk** reúne uma aplicação mobile para solicitantes, uma interface web para atendentes e administradores, uma API central e uma biblioteca compartilhada de integração. Essa organização permite que os diferentes perfis utilizem interfaces adequadas às suas atividades e compartilhem o mesmo fluxo de atendimento.

O backend concentra as regras de negócio, o controle de acesso, a triagem e a persistência dos dados. As interfaces utilizam comunicação em tempo real para as conversas e chamadas REST para operações como consulta de histórico e gerenciamento de chamados. A biblioteca compartilhada padroniza a comunicação dos clientes com o backend.

### Principais funcionalidades documentadas

- Troca de mensagens entre solicitantes e atendentes em uma tela de chat.
- Triagem automatizada com perguntas iniciais e respostas estruturadas.
- Abertura, atribuição, encaminhamento, atualização de status e encerramento de chamados.
- Cadastro, autenticação e controle de permissões por perfil.
- Administração de usuários e monitoramento dos atendimentos.
- Consulta e pesquisa no histórico das conversas.
- Alertas na interface para identificar novas mensagens.
- Dashboards e gráficos de auditoria para acompanhamento da operação.
- Avaliação do atendimento após o encerramento do chamado.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| SyncDesk API | Regras de negócio, autenticação, usuários, chamados, triagem, métricas e persistência |
| SyncDesk Mobile | Interface do solicitante, abertura de atendimentos, chat e histórico |
| SyncDesk Web | Interface de atendentes e administradores, gestão de chamados, usuários e dashboards |
| SyncDesk Library | Contratos e chamadas compartilhadas para integração das interfaces com o backend |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Data registrada | Situação no README fornecido |
|---|---|---|
| Kick-off | 03/03/2026 | Concluído |
| Sprint 1 | 05/04/2026 | Concluída; demonstração em vídeo disponível |
| Sprint 2 | 03/05/2026 | Concluída |
| Sprint 3 | 31/05/2026 | Concluída |
| Feira de Soluções | 25/06/2026 | Registrada como “Não iniciado”; realização não confirmada no material |

O backlog registra como concluídas as funcionalidades das três sprints. Como o mesmo README mantém o projeto “Em Desenvolvimento” e a Feira de Soluções como “Não iniciado”, esses registros não permitem confirmar o encerramento formal do projeto.

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório principal e documentação do SyncDesk](https://github.com/Titus-System/SyncDesk)
- [SyncDesk API — backend](https://github.com/Titus-System/syncdesk-api)
- [SyncDesk Mobile — aplicativo](https://github.com/Titus-System/syncdesk-mobile)
- [SyncDesk Web — interface de atendimento e administração](https://github.com/Titus-System/syncdesk-web)
- [SyncDesk Library — biblioteca compartilhada](https://github.com/Titus-System/syncdesk-library)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir à demonstração da Sprint 1](https://youtu.be/ucNTISGGgis)

O vídeo está indicado na documentação do projeto como entrega da primeira sprint. Ele não representa, necessariamente, todas as funcionalidades das sprints posteriores.

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

| Área | Tecnologias | Aplicação documentada no projeto |
|---|---|---|
| Backend | Python e FastAPI | API central, regras de negócio, usuários, chamados e triagem automatizada |
| Persistência relacional | PostgreSQL e SQLAlchemy | Dados estruturados e acesso aos dados no backend |
| Persistência de mensagens | MongoDB | Armazenamento de mensagens e interações |
| Autenticação | JWT | Autenticação no backend e suporte ao controle de acesso |
| Aplicação mobile | React Native, Expo, TypeScript e TailwindCSS | Interface dos solicitantes e integração com o atendimento |
| Aplicação web | React, JavaScript, Vite e TailwindCSS | Interface de atendentes e administradores |
| Estado assíncrono | React Query | Consulta e sincronização de dados na aplicação web |
| Comunicação | WebSocket e APIs REST | Mensagens em tempo real, histórico e operações do sistema |
| Biblioteca compartilhada | TypeScript, Axios e npm | Padronização e distribuição da integração com o backend |
| Testes e qualidade | Pytest e ESLint | Ferramentas de testes e análise de código citadas na documentação |
| Ambiente e versionamento | Docker, Node.js, Git e GitHub | Ferramentas indicadas para o ambiente de desenvolvimento e colaboração |

As tecnologias desta seção pertencem à solução da equipe. A experiência individual com cada uma deve ser registrada separadamente na autoavaliação abaixo.

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor (Dev Team)** na equipe do SyncDesk, conforme a composição de integrantes registrada no README do projeto.

**Pendente de preenchimento pelo aluno:** detalhar as atividades realizadas individualmente. O material fornecido descreve as responsabilidades dos componentes, mas não associa funcionalidades, decisões técnicas ou artefatos específicos a cada desenvolvedor.

| Aspecto do relato | Informação a completar |
|---|---|
| Escopo de atuação | [PREENCHER: componentes em que atuei e responsabilidades assumidas] |
| Entregas individuais | [PREENCHER: funcionalidades, correções, testes ou documentação que produzi] |
| Decisão ou desafio técnico | [PREENCHER: problema enfrentado, solução adotada e justificativa] |
| Integração com a equipe | [PREENCHER: como alinhei minha entrega com os demais componentes] |
| Resultado e evidências | [PREENCHER: resultado observado e links de commits, pull requests, issues ou demonstrações] |

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar a autoavaliação técnica a completar</strong></summary>

<br>

Registrar apenas tecnologias utilizadas pessoalmente. Utilizar o mesmo padrão dos relatórios anteriores para o nível de proficiência, como “Sei fazer com autonomia” ou “Faço com ajuda”.

| Hard skill | Nível de proficiência | Evidência individual no projeto |
|---|---|---|
| [PREENCHER: tecnologia ou competência utilizada] | [PREENCHER: autoavaliação] | [PREENCHER: entrega concreta e referência] |

</details>

---

<a id="soft-skills"></a>

<br>

## 🤝 Soft skills

<details>
  <summary><strong>Clique para visualizar o registro de competências comportamentais a completar</strong></summary>

<br>

Descrever situações vivenciadas pessoalmente, indicando a ação realizada e o resultado. A participação em uma equipe Scrum, por si só, não identifica quais competências foram exercitadas por cada integrante.

| Soft skill | Exemplo pontual no projeto |
|---|---|
| [PREENCHER: competência exercitada] | [PREENCHER: situação, ação pessoal e resultado] |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

**[PREENCHER — reflexão pessoal sobre o 5º API.]** Relatar o principal aprendizado, um desafio superado e a evolução em relação aos semestres anteriores, relacionando a reflexão às entregas individuais descritas acima.

O contexto técnico do SyncDesk envolve a integração entre aplicações mobile e web, atendimento em tempo real, persistência em bancos diferentes e organização do ciclo de vida dos chamados. Esses temas podem orientar a reflexão quando corresponderem à experiência efetivamente vivenciada pelo aluno.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 4 • AdaTech](./API_4.md) | [➡️ API 6 • Synapse](./API_6.md) |

</div>
