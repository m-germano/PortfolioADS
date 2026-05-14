# API 3 - AdaTrade

<p align="center">
  <strong>3º Semestre de ADS</strong><br>
  Plataforma web de acompanhamento dos resultados de importação e exportação dos estados brasileiros<br>
  Papel exercido: <strong>Product Owner, ETL, backend principal e integração frontend-backend</strong>
</p>

---

## Atalhos

- [Visão geral](#visão-geral)
- [Cliente e parceiro acadêmico](#cliente-e-parceiro-acadêmico)
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

O terceiro API foi o projeto mais importante da minha trajetória até este momento no curso. O desafio consistia em desenvolver uma plataforma web para acompanhamento dos resultados de importação e exportação dos estados brasileiros, com base em dados abertos oficiais do Ministério do Desenvolvimento, Indústria, Comércio e Serviços.

O projeto recebeu o nome de **AdaTrade** e foi pensado para apoiar economistas, gestores públicos, empresas e demais tomadores de decisão na análise do comércio exterior brasileiro. A proposta era transformar grandes volumes de dados históricos em informações claras, acessíveis e úteis para interpretação do desempenho dos estados e municípios no mercado internacional.

Nesse semestre, atuei com forte protagonismo como **Product Owner**, responsável pelo relacionamento com o cliente e definição do produto, além de atuar como responsável pelo processo de **ETL dos dados**, desenvolvedor backend principal e ponto central de integração entre frontend e backend.

---

## Cliente e parceiro acadêmico

| Item | Descrição |
|---|---|
| Cliente | Dom Rock |
| Representante | Felipe Santos |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |
| Repositório | [equipeAdalove/API-SEMESTRE3](https://github.com/equipeAdalove/API-SEMESTRE3) |
| Equipe | AdaLove |
| Produto | AdaTrade |

---

## Problema proposto

O comércio exterior brasileiro gera grande volume de dados públicos, mas a análise desses dados pode ser complexa para usuários que não têm domínio técnico em manipulação de bases, consultas e tratamento de informações. A empresa parceira propôs o desafio de criar uma plataforma web capaz de disponibilizar informações sobre importações e exportações dos estados brasileiros de forma acessível, organizada e visual.

O problema central era permitir que os usuários identificassem estados e municípios em ascensão, estagnação ou declínio no mercado internacional. Para isso, a solução precisava tratar bases extensas, organizar os dados por recortes relevantes e apresentar indicadores de forma compreensível para apoiar tomada de decisão.

---

## Solução desenvolvida

A solução desenvolvida foi o **AdaTrade**, uma plataforma web voltada à análise do desempenho dos estados brasileiros no comércio exterior. O sistema organiza e estrutura dados de importação e exportação, permitindo consultas por estado, município, ano, tipo de operação, produto e outros recortes relevantes.

O projeto foi construído com foco em transformar dados brutos em informação. Para isso, foi necessário criar um processo de ETL para extrair, limpar, padronizar e otimizar grandes volumes de dados históricos. Em seguida, esses dados foram disponibilizados por meio de uma API REST, consumida pelo frontend para apresentar visualizações e consultas de forma mais intuitiva.

---

## Funcionalidades

- Consulta de dados de importação e exportação por estado brasileiro.
- Análise de desempenho de municípios no comércio exterior.
- Visualização de indicadores por período.
- Filtros por produto, operação, localidade e recortes temporais.
- Comparação de resultados entre estados.
- Consulta de dados por NCM.
- API REST para disponibilização dos dados tratados.
- Processo de ETL para limpeza, padronização e otimização dos dados.
- Estruturas otimizadas para melhorar desempenho das consultas.
- Integração entre backend e frontend para consumo dos indicadores.

---

## Tecnologias utilizadas

| Tecnologia | Aplicação no projeto |
|---|---|
| Python | ETL, limpeza, tratamento e otimização dos dados |
| Pandas | Manipulação de grandes bases históricas |
| TypeScript | Desenvolvimento da API e estrutura do backend |
| NestJS | Construção da API REST |
| SQL | Consulta, organização e análise dos dados |
| PostgreSQL | Banco de dados relacional do projeto |
| React | Desenvolvimento da interface web |
| Vite | Ambiente de desenvolvimento frontend |
| HTML e CSS | Estrutura e estilização da interface |
| Cache em memória | Otimização de desempenho de consultas recorrentes |
| Tabelas pré-calculadas | Redução do custo de processamento em consultas pesadas |
| Git e GitHub | Versionamento e colaboração |
| Figma | Apoio à prototipação e alinhamento visual |
| Jira | Acompanhamento das atividades e sprints em nível de uso básico/intermediário |
| Scrum | Organização do ciclo de desenvolvimento |

---

## Minhas contribuições

Este foi o API em que tive maior responsabilidade até então. Minha atuação combinou produto, dados, backend, integração e comunicação com o cliente.

### Contribuições como Product Owner

- Atuei como ponte entre equipe e cliente para entendimento do problema, definição de escopo e validação das entregas.
- Conduzi conversas com o cliente para compreender expectativas, prioridades e restrições do projeto.
- Apoiei a construção e priorização do backlog do produto.
- Traduzi necessidades de negócio em funcionalidades técnicas para o time de desenvolvimento.
- Ajudei a organizar entregas por sprint, mantendo o MVP conectado ao problema real proposto.
- Participei da validação das funcionalidades e da preparação das apresentações do projeto.

### Contribuições em ETL e dados

- Fui responsável pelo processo de ETL dos dados de comércio exterior.
- Realizei limpeza, padronização e organização de grandes volumes de dados históricos.
- Trabalhei com bases oficiais, tratando inconsistências e preparando os dados para uso na aplicação.
- Estruturei dados de forma mais eficiente para permitir consultas por estado, município, NCM, período e tipo de operação.
- Implementei estratégias de otimização, como tabelas pré-calculadas e cache em memória, para melhorar desempenho e escalabilidade.

### Contribuições em backend

- Atuei como desenvolvedor backend principal.
- Desenvolvi a API REST responsável por disponibilizar os dados tratados para o frontend.
- Criei regras de negócio para consultas, filtros e recortes de dados.
- Estruturei endpoints para atender às necessidades de visualização e comparação da plataforma.
- Trabalhei na integração entre backend e banco de dados.
- Realizei ajustes de desempenho para evitar lentidão em consultas com grande volume de informação.

### Contribuições na integração frontend-backend

- Fui responsável por garantir a integração entre frontend e backend.
- Alinhei contratos de dados com a equipe de frontend para que os componentes consumissem corretamente a API.
- Apoiei a correção de inconsistências entre dados retornados e dados exibidos na interface.
- Atuei na validação dos fluxos de consulta para garantir que a experiência final estivesse coerente com a proposta do produto.

### Importância da minha atuação

Minha atuação foi central para o sucesso do AdaTrade porque o projeto dependia diretamente da qualidade dos dados e da confiabilidade da API. Sem um processo sólido de ETL, os dados oficiais não poderiam ser usados de forma eficiente na plataforma. Sem uma API bem estruturada, o frontend não conseguiria apresentar as informações de maneira clara e performática.

Além disso, o papel de Product Owner exigiu que eu conectasse a visão do cliente às decisões técnicas da equipe. Esse equilíbrio entre negócio, dados e desenvolvimento tornou o projeto uma experiência muito relevante para minha formação e foi um dos motivos pelos quais ele se tornou o API mais marcante da minha trajetória até o momento.

---

## Hard skills

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Python | Sei fazer com autonomia | Processo de ETL, limpeza e tratamento de grandes volumes de dados |
| Pandas | Sei fazer com autonomia | Manipulação e padronização das bases históricas |
| TypeScript | Sei fazer com autonomia | Desenvolvimento backend e estruturação da API |
| NestJS | Sei fazer com autonomia | Construção da API REST do projeto |
| SQL | Sei fazer com autonomia | Consultas, análise e organização de dados |
| PostgreSQL | Sei fazer com autonomia | Armazenamento e consulta dos dados tratados |
| Modelagem de dados | Sei fazer com autonomia | Estruturação das bases para uso pela aplicação |
| Cache em memória | Sei fazer com autonomia | Otimização de desempenho das consultas |
| Tabelas pré-calculadas | Sei fazer com autonomia | Redução de processamento em consultas pesadas |
| React | Sei fazer com autonomia | Integração com frontend e consumo da API |
| Git e GitHub | Sei fazer com autonomia | Versionamento e colaboração no repositório |
| Scrum e Product Owner | Sei fazer com autonomia | Gestão do backlog, comunicação com cliente e validação das entregas |
| Figma | Sei fazer com autonomia | Apoio à prototipação e alinhamento visual |
| Jira | Sei fazer com ajuda | Uso para acompanhamento das atividades, sem domínio avançado da ferramenta |

---

## Soft skills

| Soft skill | Situação em que foi exercitada |
|---|---|
| Comunicação com cliente | Como Product Owner, conversei diretamente com o cliente para entender expectativas, prioridades e validações |
| Visão de negócio | Precisei transformar dados públicos de comércio exterior em funcionalidades úteis para tomada de decisão |
| Protagonismo | Assumi responsabilidades centrais em produto, ETL, backend e integração, sendo um dos principais pontos técnicos do projeto |
| Organização | Foi necessário organizar backlog, dados, endpoints e entregas por sprint sem perder o foco no MVP |
| Pensamento analítico | Trabalhei com grandes volumes de dados, identificando formas de limpeza, padronização e otimização |
| Resolução de problemas | Enfrentei desafios de desempenho, inconsistência de dados e integração entre frontend e backend |
| Liderança prática | Mesmo atuando também como desenvolvedor, precisei orientar decisões e manter alinhamento entre time e cliente |

---

## Aprendizados

O AdaTrade foi o projeto que mais consolidou minha identidade profissional dentro do curso. Nele, percebi com clareza como dados, backend, produto e comunicação com cliente se conectam em uma solução real.

Aprendi que trabalhar com dados públicos exige muito cuidado. Antes de criar dashboards ou consultas, é necessário garantir que a base esteja limpa, padronizada, compreensível e preparada para uso. Também aprendi que desempenho precisa ser pensado desde o início, principalmente quando o sistema lida com grandes volumes de dados históricos.

Como Product Owner, desenvolvi minha capacidade de ouvir o cliente, traduzir necessidades em requisitos e equilibrar expectativas com viabilidade técnica. Como desenvolvedor backend e responsável pelo ETL, aprofundei meu conhecimento técnico e minha autonomia em decisões de arquitetura, dados e integração.

Esse API também foi importante fora da sala de aula, pois o projeto AdaTrade foi apresentado no **PyDay SJC**, reforçando sua relevância técnica e meu envolvimento com a comunidade de tecnologia.

---

## Links

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE3)


---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 2 • MindDoc Analyzer](./API_2.md) | [➡️ API 4 • AdaTech](./API_4.md) |

</div>
