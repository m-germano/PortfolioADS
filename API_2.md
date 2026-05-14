# API 2 - MindDoc Analyzer

<p align="center">
  <strong>2º Semestre de ADS</strong><br>
  Software para automatizar a extração de informações de documentos<br>
  Papel exercido: <strong>Dev Team, estrutura do sistema, lógica de negócio e telas</strong>
</p>

---

## Atalhos

- [Visão geral](#visão-geral)
- [Parceiro acadêmico](#parceiro-acadêmico)
- [Problema proposto](#problema-proposto)
- [Solução desenvolvida](#solução-desenvolvida)
- [Funcionalidades](#funcionalidades)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Minhas contribuições](#minhas-contribuições)
- [Hard skills](#hard-skills)
- [Soft skills](#soft-skills)
- [Aprendizados](#aprendizados)
- [Links](#links)

---

## Visão geral

O segundo API teve como objetivo o desenvolvimento de um software capaz de automatizar a extração de informações de documentos utilizando modelos de linguagem e visão. O projeto recebeu o nome de **MindDoc Analyzer** e foi direcionado ao contexto de relatórios clínicos, com foco em facilitar o acesso, a organização e a análise de dados relevantes para profissionais da área de psicologia.

Esse projeto representou uma evolução importante em relação ao primeiro semestre, pois envolveu mais regras de negócio, persistência de dados, telas de cadastro e consulta, além da necessidade de lidar com informações extraídas automaticamente de documentos. Minha atuação ocorreu como integrante do **Dev Team**, contribuindo diretamente para a estrutura do sistema, lógica de negócio, funcionalidades e telas.

---

## Parceiro acadêmico

| Item | Descrição |
|---|---|
| Parceiro | Fatec São José dos Campos - Prof. Jessen Vidal |
| Contexto | Projeto acadêmico desenvolvido no 2º semestre do curso de ADS |
| Repositório | [equipeAdalove/API-SEMESTRE2](https://github.com/equipeAdalove/API-SEMESTRE2) |
| Equipe | AdaLove |
| Produto | MindDoc Analyzer |

---

## Problema proposto

Muitas organizações lidam diariamente com grande volume de documentos. Mesmo quando esses documentos são digitalizados, a extração de informações relevantes pode continuar sendo uma atividade lenta, manual e sujeita a erros. Em documentos com layouts variados, apenas extrair texto não é suficiente, pois o significado das informações depende também do contexto visual e da estrutura do documento.

No contexto do projeto, o problema foi aplicado a relatórios clínicos. A necessidade era automatizar a extração de informações essenciais, como diagnósticos, tratamentos e evolução do paciente, organizando esses dados em uma estrutura acessível para consulta, edição e manutenção.

---

## Solução desenvolvida

A solução criada foi o **MindDoc Analyzer**, uma aplicação voltada ao cadastro, extração, consulta, edição e exclusão de informações provenientes de relatórios clínicos. O sistema foi pensado para facilitar o trabalho de profissionais que precisam analisar documentos com informações sensíveis e estruturá-las de forma mais eficiente.

A proposta do MVP foi permitir que o usuário cadastrasse relatórios, submetesse documentos para análise por modelos de linguagem e visão, visualizasse as informações extraídas de maneira organizada e pudesse ajustar manualmente os dados quando necessário. Também foram considerados requisitos de privacidade, funcionamento local e controle de acesso, uma vez que o sistema trabalha com dados clínicos.

---

## Funcionalidades

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

## Tecnologias utilizadas

| Tecnologia | Aplicação no projeto |
|---|---|
| Java | Desenvolvimento da aplicação e implementação de regras de negócio |
| Programação orientada a objetos | Organização da lógica, entidades e responsabilidades do sistema |
| CSS | Estilização da interface |
| MySQL | Banco de dados relacional para armazenamento dos relatórios |
| Maven | Gerenciamento de dependências do projeto |
| JUnit | Apoio a testes |
| Ollama | Uso local de modelos de linguagem |
| Figma | Prototipação e apoio ao desenho das telas |
| Trello | Organização visual das tarefas |
| Jira | Acompanhamento de tarefas e sprints em nível de uso básico/intermediário |
| Git e GitHub | Versionamento e colaboração |

---

## Minhas contribuições

Atuei como integrante do **Dev Team**, participando do desenvolvimento da estrutura da aplicação, criação de telas, implementação da lógica de negócio e construção de funcionalidades.

### Contribuições técnicas

- Ajudei na estruturação inicial do sistema, organizando partes importantes para o funcionamento da aplicação.
- Desenvolvi telas voltadas ao cadastro, consulta, edição e visualização das informações dos relatórios.
- Contribuí com a implementação da lógica de negócio necessária para manipular os relatórios clínicos.
- Apoiei o fluxo de cadastro e manutenção dos dados no banco.
- Participei da construção de funcionalidades relacionadas ao CRUD dos relatórios.
- Trabalhei na conexão entre interface, regras de negócio e persistência de dados.
- Realizei ajustes e correções ao longo das sprints para melhorar a experiência de uso e a estabilidade do sistema.

### Protagonismo no semestre

Mesmo atuando formalmente como Dev Team, tive uma participação ativa na construção técnica do produto. Minha contribuição não ficou restrita a tarefas isoladas. Participei da estruturação do sistema, da criação das telas e da lógica de negócio, conectando diferentes partes da aplicação para que o fluxo fizesse sentido para o usuário.

Como já tinha experiência prévia com programação, consegui atuar com autonomia na implementação e também apoiar decisões técnicas do time. Esse protagonismo foi importante porque o projeto exigia mais do que telas funcionando: era necessário garantir que cadastro, consulta, edição, banco de dados e extração automatizada estivessem alinhados em um fluxo coerente.

### Importância da minha atuação

Minha participação neste API foi importante para consolidar conhecimentos de desenvolvimento de software em uma aplicação mais próxima de um sistema real. Diferente do primeiro semestre, em que o foco era um site informativo, este projeto exigiu pensar em dados, regras, telas, fluxos de uso e consistência das informações.

Também pude entender melhor a responsabilidade de desenvolver soluções que lidam com informações sensíveis. O contexto clínico exigiu atenção à privacidade, organização e confiabilidade dos dados, fatores que influenciaram diretamente a forma como o sistema foi pensado e implementado.

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
| Jira | Sei fazer com ajuda | Uso para acompanhamento de tarefas, sem domínio avançado da ferramenta |
| Git e GitHub | Sei fazer com autonomia | Versionamento e colaboração no repositório |

---

## Soft skills

| Soft skill | Situação em que foi exercitada |
|---|---|
| Trabalho em equipe | Atuei como Dev Team, precisando alinhar minhas entregas com as demais partes do sistema |
| Comunicação | Foi necessário comunicar dúvidas, impedimentos e avanços para evitar retrabalho entre telas, lógica e banco de dados |
| Responsabilidade | O projeto lidava com dados clínicos, exigindo atenção à organização, privacidade e confiabilidade das informações |
| Protagonismo técnico | Assumi participação ativa na estrutura, nas telas e na lógica de negócio, ajudando a sustentar o fluxo principal da aplicação |
| Resolução de problemas | Durante as sprints, precisei ajustar funcionalidades, corrigir fluxos e adaptar a lógica conforme a evolução do projeto |
| Aprendizado contínuo | O projeto envolveu tecnologias e conceitos novos, como extração automatizada de dados e uso de modelos locais |

---

## Aprendizados

O segundo API ampliou minha compreensão sobre sistemas com regras de negócio e persistência de dados. Aprendi que uma aplicação precisa ser pensada de forma integrada: tela, regra, banco de dados, validação e experiência do usuário devem funcionar em conjunto.

Também compreendi melhor os desafios de automatizar processos que antes eram manuais. A extração de informações de documentos exige cuidado, pois a tecnologia precisa apoiar o usuário sem eliminar a necessidade de revisão, principalmente em contextos sensíveis como relatórios clínicos.

Esse projeto foi importante para minha evolução como desenvolvedor, pois me aproximou de uma aplicação com características reais: cadastro, consulta, edição, exclusão, autenticação, organização de dados e preocupação com segurança.

---

## Links

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE2)


---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 1 • Horus](./API_1.md) | [➡️ API 3 • AdaTrade](./API_3.md) |

</div>
