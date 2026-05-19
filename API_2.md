# API 2 - MindDoc Analyzer

<p align="center">
  <strong>2º Semestre • 2024-2</strong><br>
  Aplicação para automatizar a extração de informações de documentos<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Aplica%C3%A7%C3%A3o%20Desktop-informational?style=for-the-badge" alt="Aplicação Desktop">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
</p>

---

## Atalhos

- [Identificação do projeto](#identificação-do-projeto)
- [Empresa parceira](#empresa-parceira)
- [Problema](#problema)
- [Solução](#solução)
- [Link do repositório Git](#link-do-repositório-git)
- [Preview da aplicação](#preview-da-aplicação)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Contribuições pessoais](#contribuições-pessoais)
- [Hard skills](#hard-skills)
- [Soft skills](#soft-skills)
- [Aprendizados](#aprendizados)

---

## Identificação do projeto

| Item | Descrição |
|---|---|
| Semestre do curso | 2º semestre |
| Ano e semestre | 2024-2 |
| Nome do projeto | MindDoc Analyzer |
| Tipo de sistema | Aplicação desktop |
| Papel no Scrum | Desenvolvedor |
| Equipe | AdaLove |

---

## Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | Fatec São José dos Campos - Prof. Jessen Vidal |
| Professor responsável pelos requisitos | Prof. Giuliano Bertoti |
| Contexto | Projeto acadêmico desenvolvido no 2º semestre do curso de Análise e Desenvolvimento de Sistemas |

---

## Problema

Muitas organizações lidam diariamente com grande volume de documentos. Mesmo quando esses documentos são digitalizados, a extração de informações relevantes pode continuar sendo uma atividade lenta, manual e sujeita a erros. Em documentos com layouts variados, apenas extrair texto não é suficiente, pois o significado das informações depende também do contexto visual e da estrutura do documento.

No contexto do projeto, o problema foi aplicado a relatórios clínicos. A necessidade era organizar informações essenciais, como diagnósticos, tratamentos e evolução do paciente, em uma estrutura acessível para consulta, edição e manutenção. Por envolver dados sensíveis, o processo também exigia cuidado com privacidade, confiabilidade e revisão das informações extraídas.

---

## Solução

A equipe desenvolveu o **MindDoc Analyzer**, uma **aplicação desktop** voltada ao cadastro, extração, consulta, edição e exclusão de informações provenientes de relatórios clínicos. O sistema permitia registrar relatórios, submeter documentos para análise por modelos de linguagem e visão, visualizar informações extraídas de forma organizada e realizar ajustes manuais quando necessário.

### Principais funcionalidades

- Cadastro de relatórios clínicos no banco de dados.
- Consulta de relatórios cadastrados.
- Atualização e exclusão de registros.
- Extração automatizada de informações essenciais dos documentos.
- Exibição estruturada das informações extraídas.
- Edição manual dos dados extraídos.
- Filtros por informações relevantes, como paciente, patologia e outros dados-chave.
- Controle de acesso e autenticação.
- Funcionamento local para preservar privacidade e reduzir dependência de APIs externas.

---

## Link do repositório Git

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE2)

---

## Preview da aplicação

https://github.com/user-attachments/assets/5ef23336-f4fe-4a3f-99b2-5dea512436ad

---

## Tecnologias utilizadas

<br>

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" width="48" height="48" alt="Java" title="Java"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" width="48" height="48" alt="CSS3" title="CSS3"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" width="48" height="48" alt="MySQL" title="MySQL"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/maven/maven-original.svg" width="48" height="48" alt="Maven" title="Maven"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/junit/junit-original.svg" width="48" height="48" alt="JUnit" title="JUnit"/>
  &nbsp;
  <img src="https://cdn.simpleicons.org/ollama/000000" width="48" height="48" alt="Ollama" title="Ollama"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" width="48" height="48" alt="Figma" title="Figma"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/trello/trello-original.svg" width="48" height="48" alt="Trello" title="Trello"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jira/jira-original.svg" width="48" height="48" alt="Jira" title="Jira"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" width="48" height="48" alt="Git" title="Git"/>
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/github/github-original.svg" width="48" height="48" alt="GitHub" title="GitHub"/>
</p>

<br>

<div align="center">

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Desenvolvimento da aplicação | Java e programação orientada a objetos | Implementação da aplicação desktop, regras de negócio, entidades e organização das responsabilidades do sistema |
| Interface | CSS | Estilização das telas e ajustes visuais para melhorar a experiência de uso |
| Banco de dados | MySQL | Armazenamento, consulta e manutenção dos relatórios clínicos cadastrados |
| Dependências e estrutura | Maven | Gerenciamento de dependências e padronização da estrutura do projeto Java |
| Testes | JUnit | Apoio à validação de funcionalidades e regras implementadas |
| Inteligência artificial local | Ollama | Uso local de modelos de linguagem e visão para apoiar a extração automatizada de informações |
| Design e prototipação | Figma | Apoio ao desenho das telas, organização visual e validação da experiência da interface |
| Gestão do projeto | Trello e Jira | Organização das tarefas, acompanhamento das sprints e visualização do andamento das entregas |
| Versionamento | Git e GitHub | Controle de versões, colaboração entre integrantes e organização do repositório |

</div>

---

## Contribuições pessoais

Atuei como **desenvolvedor** no time, participando da estruturação da aplicação, criação de telas, implementação da lógica de negócio e construção de funcionalidades. Contribuí para o fluxo de cadastro, consulta, edição e visualização das informações dos relatórios, conectando interface, regras de negócio e persistência de dados.

Minhas principais contribuições técnicas envolveram o uso de **Java**, **programação orientada a objetos**, **CSS**, **MySQL**, **Maven**, **Git** e **GitHub**. Também participei de ajustes relacionados ao uso de **Ollama** no contexto de extração automatizada de informações. Os principais artefatos gerados foram telas de cadastro e consulta, regras de manipulação dos relatórios, ajustes de interface, apoio ao CRUD dos registros e correções realizadas ao longo das sprints para melhorar a estabilidade do sistema.

---

## Hard skills

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Java | Sei fazer com autonomia | Implementação de funcionalidades e regras de negócio |
| Programação orientada a objetos | Sei fazer com autonomia | Organização da lógica do sistema e manipulação de entidades |
| MySQL | Sei fazer com autonomia | Persistência e consulta de relatórios |
| Modelagem de dados | Sei fazer com autonomia | Organização das informações extraídas e armazenadas |
| CSS | Sei fazer com autonomia | Ajustes visuais nas telas |
| Maven | Sei fazer com autonomia | Estruturação de dependências do projeto |
| JUnit | Sei fazer com autonomia | Contato e aplicação de testes no ambiente Java |
| Ollama e modelos locais | Sei fazer com autonomia | Uso de modelos de linguagem e visão no contexto do projeto |
| Figma | Sei fazer com autonomia | Apoio à prototipação e validação visual |
| Trello | Sei fazer com autonomia | Organização visual das tarefas do projeto |
| Jira | Faço com ajuda | Uso para acompanhamento de tarefas, sem domínio avançado da ferramenta |
| Git e GitHub | Sei fazer com autonomia | Versionamento e colaboração no repositório |

---

## Soft skills

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Trabalho em equipe | Durante a construção das telas de cadastro e consulta, alinhei minhas entregas com as partes de banco de dados e regras de negócio para que o fluxo dos relatórios funcionasse de forma integrada |
| Comunicação | Ao identificar divergências entre campos exibidos na tela e dados necessários para o registro dos relatórios, comuniquei o time para ajustar o fluxo antes que o problema gerasse retrabalho nas sprints seguintes |
| Responsabilidade | Como o sistema lidava com relatórios clínicos, tive cuidado ao estruturar funcionalidades de consulta, edição e manutenção dos dados, preservando clareza e organização das informações |
| Resolução de problemas | Durante as sprints, atuei em ajustes de telas e lógica de negócio quando o fluxo de cadastro e edição não refletia corretamente as informações dos relatórios |
| Aprendizado contínuo | O projeto exigiu contato com extração automatizada de informações e modelos locais, o que me levou a estudar como integrar esse tipo de recurso ao fluxo da aplicação |

---

## Aprendizados

O segundo API ampliou minha compreensão sobre sistemas com regras de negócio e persistência de dados. Aprendi que uma aplicação precisa ser pensada de forma integrada: tela, regra, banco de dados, validação e experiência do usuário devem funcionar em conjunto.

Também compreendi melhor os desafios de automatizar processos que antes eram manuais. A extração de informações de documentos exige cuidado, pois a tecnologia precisa apoiar o usuário sem eliminar a necessidade de revisão, principalmente em contextos sensíveis como relatórios clínicos.

Esse projeto foi importante para minha evolução como desenvolvedor, pois me aproximou de uma aplicação com características reais: cadastro, consulta, edição, exclusão, autenticação, organização de dados e preocupação com segurança.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 1 • Horus](./API_1.md) | [➡️ API 3 • AdaTrade](./API_3.md) |

</div>
