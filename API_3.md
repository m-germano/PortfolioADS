# API 3 - AdaTrade

<p align="center">
  <strong>3º Semestre - 2025-1</strong><br>
  Plataforma web de acompanhamento dos resultados de importação e exportação dos estados brasileiros<br>
  Papel exercido no Scrum: <strong>Product Owner</strong>
</p>

---

## Atalhos

- [Identificação do projeto](#identificação-do-projeto)
- [Empresa parceira](#empresa-parceira)
- [Problema](#problema)
- [Solução](#solução)
- [Link do repositório Git](#link-do-repositório-git)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Contribuições pessoais](#contribuições-pessoais)
- [Hard skills](#hard-skills)
- [Soft skills](#soft-skills)
- [Aprendizados](#aprendizados)

---

## Identificação do projeto

| Item | Descrição |
|---|---|
| Semestre do curso | 3º semestre |
| Ano e semestre | 2025-1 |
| Nome do projeto | AdaTrade |
| Tipo de sistema | Plataforma web |
| Papel no Scrum | Product Owner |
| Equipe | AdaLove |

---

## Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | Dom Rock |
| Representante | Felipe Santos |
| Área de atuação | Tecnologia, dados e inteligência artificial aplicada a negócios |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

## Problema

O comércio exterior brasileiro gera grande volume de dados públicos, mas a análise desses dados pode ser complexa para usuários que não têm domínio técnico em manipulação de bases, consultas e tratamento de informações. Mesmo com dados oficiais disponíveis, a leitura desses arquivos exige conhecimento técnico e tempo para limpeza, padronização e interpretação.

A empresa parceira propôs o desafio de facilitar a análise de importações e exportações dos estados brasileiros. O problema central era permitir que usuários identificassem estados e municípios em ascensão, estagnação ou declínio no mercado internacional, sem depender de processos manuais de tratamento de dados ou consultas complexas em bases extensas.

---

## Solução

A equipe desenvolveu o **AdaTrade**, uma **plataforma web** voltada à análise do desempenho dos estados brasileiros no comércio exterior. O sistema organizou dados de importação e exportação por estado, município, ano, tipo de operação, produto e outros recortes relevantes. Para isso, foi criado um processo de **ETL** para extrair, limpar, padronizar e otimizar grandes volumes de dados históricos, disponibilizando as informações por meio de uma **API REST** consumida pelo frontend.

### Principais funcionalidades

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

## Link do repositório Git

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE3)

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
| Jira | Acompanhamento das atividades e sprints em nível básico/intermediário |
| Scrum | Organização do ciclo de desenvolvimento |

---

## Contribuições pessoais

Atuei como **Product Owner** e também contribuí tecnicamente com **ETL**, backend e integração entre frontend e backend. Como Product Owner, fui ponte entre equipe e cliente para entendimento do problema, definição de escopo, construção e priorização do backlog, validação das funcionalidades e preparação das apresentações do projeto. Também traduzi necessidades de negócio em funcionalidades técnicas para o time de desenvolvimento.

Na parte de dados, fui responsável pelo processo de **ETL** dos dados de comércio exterior, utilizando **Python** e **Pandas** para limpeza, padronização e organização de grandes volumes de dados históricos. Estruturei dados para permitir consultas por estado, município, NCM, período e tipo de operação, além de implementar estratégias de otimização, como **tabelas pré-calculadas** e **cache em memória**.

No backend, atuei com **TypeScript**, **NestJS**, **SQL** e **PostgreSQL** para desenvolver a **API REST** responsável por disponibilizar os dados tratados ao frontend. Criei regras de negócio para consultas, filtros e recortes de dados, estruturei endpoints para visualização e comparação dos indicadores e realizei ajustes de desempenho para reduzir lentidão em consultas com grande volume de informação. Também alinhei contratos de dados com o frontend em **React**, garantindo que os componentes consumissem corretamente a API.

Os principais artefatos gerados foram scripts de ETL, bases tratadas, estrutura de banco de dados, endpoints da API REST, regras de consulta, filtros, tabelas pré-calculadas, ajustes de cache, documentação de apoio ao time e backlog priorizado para as sprints.

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
| Jira | Faço com ajuda | Uso para acompanhamento das atividades, sem domínio avançado da ferramenta |

---

## Soft skills

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Comunicação com cliente | Nas conversas com o representante da Dom Rock, alinhei expectativas sobre os recortes de análise de comércio exterior e transformei essas necessidades em itens de backlog para o time |
| Visão de negócio | Ao estruturar consultas por estado, município, NCM e período, conectei os dados públicos disponíveis a funcionalidades úteis para apoiar análise de desempenho no comércio exterior |
| Organização | Durante o desenvolvimento do ETL e da API, organizei bases, endpoints, filtros e prioridades de sprint para manter o MVP viável dentro do prazo do semestre |
| Pensamento analítico | Ao lidar com grandes volumes de dados oficiais, precisei identificar inconsistências, definir padrões de limpeza e preparar estruturas mais eficientes para consulta |
| Resolução de problemas | Quando consultas com grande volume de informação apresentaram risco de lentidão, implementei tabelas pré-calculadas e cache em memória para melhorar o desempenho da plataforma |
| Colaboração | Durante a integração frontend-backend, alinhei contratos de dados com a equipe de frontend para corrigir divergências entre os dados retornados pela API e os dados exibidos na interface |

---

## Aprendizados

O AdaTrade foi o projeto que mais consolidou minha identidade profissional dentro do curso. Nele, percebi com clareza como dados, backend, produto e comunicação com cliente se conectam em uma solução real.

Aprendi que trabalhar com dados públicos exige muito cuidado. Antes de criar dashboards ou consultas, é necessário garantir que a base esteja limpa, padronizada, compreensível e preparada para uso. Também aprendi que desempenho precisa ser pensado desde o início, principalmente quando o sistema lida com grandes volumes de dados históricos.

Como Product Owner, desenvolvi minha capacidade de ouvir o cliente, traduzir necessidades em requisitos e equilibrar expectativas com viabilidade técnica. Como desenvolvedor backend e responsável pelo ETL, aprofundei meu conhecimento técnico e minha autonomia em decisões de arquitetura, dados e integração.

Esse API também foi importante fora da sala de aula, pois o projeto AdaTrade foi apresentado no **PyDay SJC**, reforçando sua relevância técnica e meu envolvimento com a comunidade de tecnologia.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 2 • MindDoc Analyzer](./API_2.md) | [➡️ API 4 • AdaTech](./API_4.md) |

</div>