# API 4 - AdaTech

<p align="center">
  <strong>4º Semestre - 2025-2</strong><br>
  Agente de Inteligência Artificial para automação da instrução de registro aduaneiro<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
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
| Semestre do curso | 4º semestre |
| Ano e semestre | 2025-2 |
| Nome do projeto | AdaTech |
| Tipo de sistema | Plataforma web |
| Papel no Scrum | Desenvolvedor |
| Equipe | AdaLove |

---

## Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | TecSys Brasil |
| Representante | Creonice Honório |
| Área de atuação | Soluções tecnológicas aplicadas a processos aduaneiros e comércio exterior |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

## Problema

A elaboração da instrução de registro aduaneiro é um processo manual que exige atenção a dados como Part-Number, classificação fiscal, fabricante, origem e endereço do fabricante. Quando essas informações são tratadas manualmente, podem ocorrer erros de interpretação, descrições ambíguas, retrabalho e riscos de questionamentos, penalidades ou multas.

O desafio era apoiar a geração de descrições claras, precisas e compatíveis com exigências legais. A empresa precisava reduzir esforço manual e aumentar a segurança das informações geradas para submissão à Receita Federal, sem eliminar a necessidade de revisão humana em um processo de alta responsabilidade.

---

## Solução

A equipe desenvolveu o **AdaTech**, uma **plataforma web** que utiliza inteligência artificial para apoiar a criação da instrução de registro aduaneiro. O sistema permite upload de PDFs de pedidos de compra, extração de Part-Numbers, sugestão de NCM e descrição dos itens, revisão manual das informações extraídas, geração de arquivo Excel com dados finais e consulta ao histórico de documentos processados.

### Principais funcionalidades

- Upload de PDF de pedido de compra.
- Extração de Part-Numbers presentes no documento.
- Sugestão de NCM e descrição de cada item.
- Uso de RAG para apoiar a geração de respostas com contexto mais relevante.
- Integração com Ollama para execução local de modelo de linguagem.
- Formulário para revisão e correção das informações extraídas.
- Geração de arquivo Excel com os dados finais.
- Tela de login para controle de acesso.
- Histórico de PDFs processados.
- Documentação de instalação e uso.
- Integração entre backend, banco de dados, frontend e agente de IA.

---

## Link do repositório Git

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE4)

---

## Tecnologias utilizadas

| Tecnologia | Aplicação no projeto |
|---|---|
| Python | Desenvolvimento backend, regras de negócio e integração com IA |
| FastAPI | Construção da API e endpoints do sistema |
| PostgreSQL | Armazenamento de dados processados e histórico |
| RAG | Recuperação de contexto para apoiar respostas mais relevantes da IA |
| Ollama | Execução local de modelo de linguagem |
| DuckDuckGo | Apoio a buscas e enriquecimento de informações |
| TypeScript | Desenvolvimento frontend e integração |
| React | Interface web da aplicação |
| Vite | Ambiente de desenvolvimento frontend |
| HTML e CSS | Estrutura e estilização das telas |
| Node.js | Apoio ao ambiente frontend |
| Figma | Prototipação e apoio visual |
| Slack | Comunicação da equipe |
| Jira | Gestão das tarefas e sprints em nível básico/intermediário |
| Git e GitHub | Versionamento e colaboração |

---

## Contribuições pessoais

Atuei como **desenvolvedor** no time, com foco em backend, estrutura da aplicação, regras de negócio e recursos de inteligência artificial. Contribuí para a organização do fluxo de processamento entre upload, extração, sugestão, revisão e geração do arquivo final, além de apoiar a divisão entre responsabilidades do backend, frontend, banco de dados e agente de IA.

No backend, trabalhei com **Python**, **FastAPI** e **PostgreSQL** para desenvolver regras de negócio relacionadas ao processamento dos documentos, lidar com dados como Part-Number, NCM, fabricante, origem e descrição dos produtos, integrar backend e banco de dados, apoiar a criação de endpoints consumidos pelo frontend e organizar os dados finais exportáveis.

Na camada de inteligência artificial, implementei recursos envolvendo **RAG** para melhorar o uso de contexto na geração das respostas e trabalhei na integração com **Ollama**, permitindo o uso local de modelo de linguagem dentro do fluxo da aplicação. Também apoiei a estruturação de prompts e respostas para que a IA retornasse informações mais úteis ao processo aduaneiro, considerando limitações da tecnologia e a necessidade de revisão humana antes da geração final das instruções.

Os principais artefatos gerados foram endpoints da API, regras de processamento, integrações com banco de dados, fluxo de RAG, integração com Ollama, estruturação de prompts, organização dos dados exportáveis em Excel e ajustes de comunicação entre backend, IA e frontend.

---

## Hard skills

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Python | Sei fazer com autonomia | Implementação de regras de negócio, backend e integração com IA |
| FastAPI | Sei fazer com autonomia | Criação de endpoints e estrutura da API |
| PostgreSQL | Sei fazer com autonomia | Persistência de dados processados e histórico |
| RAG | Sei fazer com autonomia | Implementação de recuperação de contexto para apoiar respostas da IA |
| Ollama | Sei fazer com autonomia | Integração com modelo de linguagem local |
| Integração com IA | Sei fazer com autonomia | Conexão entre IA, backend, dados e revisão do usuário |
| Manipulação de PDFs | Sei fazer com autonomia | Apoio ao fluxo de extração de dados dos documentos |
| Geração de Excel | Sei fazer com autonomia | Organização dos dados finais para exportação |
| React e TypeScript | Sei fazer com autonomia | Integração com frontend e apoio ao consumo da API |
| Git e GitHub | Sei fazer com autonomia | Versionamento e colaboração no repositório |
| Figma | Sei fazer com autonomia | Apoio visual e entendimento de fluxos de interface |
| Jira | Faço com ajuda | Uso para acompanhamento de tarefas, sem domínio avançado da ferramenta |

---

## Soft skills

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Responsabilidade | Como o sistema apoiava um processo aduaneiro sensível, tratei regras de processamento e dados exportáveis com cuidado para permitir revisão humana antes da geração final |
| Pensamento crítico | Ao trabalhar com IA, considerei que as respostas do modelo poderiam conter inconsistências e ajudei a estruturar o fluxo para que o usuário pudesse revisar e corrigir as informações |
| Organização técnica | Durante a definição do fluxo entre upload, extração, sugestão, revisão e exportação, organizei responsabilidades entre backend, banco de dados e agente de IA para reduzir inconsistências |
| Colaboração | Alinhei contratos de dados com integrantes do frontend para que as informações extraídas e sugeridas pela IA fossem exibidas corretamente na interface |
| Resolução de problemas | Ao lidar com documentos, sugestões de IA e geração de Excel, ajustei partes do fluxo para transformar respostas textuais em dados mais estruturados e aproveitáveis pelo sistema |
| Comunicação | Durante a integração entre backend e frontend, expliquei regras e formatos de retorno para evitar divergências entre o processamento dos dados e a visualização na tela |
| Adaptabilidade | O uso de RAG e Ollama exigiu ajustes conforme testes, inconsistências e necessidades do cliente, o que exigiu adaptação contínua durante as sprints |

---

## Aprendizados

O quarto API me ensinou que projetos com inteligência artificial exigem mais do que apenas conectar um modelo ao sistema. É necessário pensar em fluxo, validação, revisão, armazenamento, confiabilidade e clareza das informações geradas.

Também aprendi que, em processos sensíveis, a automação deve apoiar o trabalho humano, não substituir completamente a responsabilidade de revisão. No caso do AdaTech, a IA ajudava a reduzir esforço manual e retrabalho, mas o sistema precisava permitir correções e validações antes da geração final.

Do ponto de vista técnico, aprofundei minha experiência em backend com Python e FastAPI, integração com banco de dados, criação de regras de negócio e comunicação entre diferentes partes da aplicação. A implementação de recursos envolvendo RAG e Ollama reforçou meu interesse por soluções que combinam backend, inteligência artificial e automação de processos reais.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 3 • AdaTrade](./API_3.md) | — |

</div>