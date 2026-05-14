# API 4 - AdaTech

<p align="center">
  <strong>4º Semestre de ADS</strong><br>
  Agente de Inteligência Artificial para automação da instrução de registro aduaneiro<br>
  Papel exercido: <strong>Dev Team, backend principal, regras de negócio, RAG e integração com Ollama</strong>
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

O quarto API teve como desafio a criação de um agente de inteligência artificial capaz de automatizar a elaboração da instrução de registro aduaneiro. O projeto recebeu o nome de **AdaTech** e tinha como objetivo reduzir erros humanos, retrabalho e riscos legais em um processo que exige precisão na descrição de produtos, classificação fiscal, fabricante, origem e demais informações relevantes.

Nesse projeto, atuei como integrante do **Dev Team**, mas com forte protagonismo técnico no backend e na camada de inteligência artificial. Fui responsável pela estrutura da aplicação, criação da lógica de negócio, desenvolvimento de regras fundamentais para o funcionamento do sistema e implementação de recursos envolvendo **RAG**, **Ollama** e integração entre IA, backend, banco de dados e frontend.

---

## Cliente e parceiro acadêmico

| Item | Descrição |
|---|---|
| Cliente | TecSys Brasil |
| Representante | Creonice Honório |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |
| Repositório | [equipeAdalove/API-SEMESTRE4](https://github.com/equipeAdalove/API-SEMESTRE4) |
| Equipe | AdaLove |
| Produto | AdaTech |

---

## Problema proposto

A elaboração da instrução de registro aduaneiro é um processo manual que exige atenção a dados como Part-Number, classificação fiscal, fabricante, origem e endereço do fabricante. Quando essas informações são tratadas manualmente, podem ocorrer erros de interpretação, descrições ambíguas, retrabalho e riscos de questionamentos, penalidades ou multas.

O desafio era criar uma solução que automatizasse esse processo de forma inteligente, gerando descrições claras, precisas e compatíveis com exigências legais. A ferramenta precisava apoiar a equipe responsável, reduzir esforço manual e aumentar a segurança das informações geradas para submissão à Receita Federal.

---

## Solução desenvolvida

A solução desenvolvida foi o **AdaTech**, uma plataforma que utiliza inteligência artificial para automatizar a criação da instrução de registro aduaneiro. O sistema integra dados essenciais, como Part-Number, classificação fiscal, fabricante e origem, para gerar uma descrição do produto mais clara, padronizada e alinhada às exigências do processo aduaneiro.

O MVP foi construído para permitir upload de PDFs de pedidos de compra, extração de Part-Numbers, sugestão de NCM e descrição dos itens, revisão manual das informações extraídas, geração de arquivo Excel com dados finais e consulta ao histórico de documentos processados.

A proposta foi substituir um fluxo manual, demorado e sujeito a falhas por uma solução mais rápida, rastreável e confiável, sem eliminar a necessidade de revisão humana em um processo de alta responsabilidade.

---

## Funcionalidades

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
| Jira | Gestão das tarefas e sprints em nível de uso básico/intermediário |
| Git e GitHub | Versionamento e colaboração |

---

## Minhas contribuições

Atuei como desenvolvedor do **Dev Team**, com responsabilidade central no backend, estrutura da aplicação, regras de negócio e recursos de inteligência artificial.

### Contribuições em estrutura e arquitetura

- Contribuí para a organização da estrutura técnica do projeto.
- Atuei na definição do fluxo de processamento entre upload, extração, sugestão, revisão e geração do arquivo final.
- Apoiei a divisão entre responsabilidades do backend, frontend, banco de dados e agente de IA.
- Trabalhei para que a aplicação mantivesse um fluxo claro e coerente para o usuário final.
- Ajudei a estruturar a comunicação entre as camadas do sistema para reduzir inconsistências entre dados processados, respostas da IA e informações exibidas no frontend.

### Contribuições em backend

- Atuei como desenvolvedor backend principal.
- Desenvolvi regras de negócio relacionadas ao processamento dos documentos.
- Implementei partes da lógica para lidar com dados como Part-Number, NCM, fabricante, origem e descrição dos produtos.
- Trabalhei na integração entre backend e banco de dados.
- Apoiei a criação de endpoints consumidos pelo frontend.
- Contribuí para a geração e organização dos dados finais exportáveis.
- Realizei ajustes para melhorar a confiabilidade do fluxo e reduzir inconsistências.

### Contribuições em RAG, Ollama e IA

- Implementei recursos envolvendo **RAG** para melhorar o uso de contexto na geração das respostas.
- Trabalhei na integração com **Ollama**, permitindo uso local de modelo de linguagem dentro do fluxo da aplicação.
- Apoiei a estruturação de prompts e respostas para que a IA retornasse informações mais úteis ao processo aduaneiro.
- Contribuí para transformar a saída da IA em dados mais estruturados e aproveitáveis pelo sistema.
- Considerei limitações da IA e a necessidade de revisão humana antes da geração final das instruções.
- Atuei na conexão entre dados extraídos, contexto recuperado, resposta gerada e revisão pelo usuário.

### Protagonismo no semestre

Embora meu papel formal tenha sido Dev Team, minha atuação foi uma das mais centrais do projeto. Assumi responsabilidade direta por partes críticas do backend e da inteligência artificial, incluindo a implementação do RAG, a integração com Ollama e a lógica necessária para transformar documentos e dados de apoio em informações úteis para a instrução de registro aduaneiro.

Esse protagonismo foi importante porque o AdaTech dependia de uma base técnica confiável. O valor da solução não estava apenas em usar IA, mas em integrar IA, regras de negócio, dados e revisão humana dentro de um fluxo seguro e aplicável a um problema real.

### Importância da minha atuação

Minha atuação foi importante porque o backend concentrava as regras essenciais do produto. Como o sistema lidava com um processo sensível de registro aduaneiro, era necessário garantir que os dados fossem tratados de forma organizada e que o fluxo permitisse revisão humana antes da geração final.

Esse projeto também me permitiu aprofundar o uso de inteligência artificial em um contexto aplicado, entendendo seus benefícios e limitações. A solução não dependia apenas de gerar texto com IA, mas de recuperar contexto, estruturar dados, validar informações e apoiar um processo real de negócio.

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
| Jira | Sei fazer com ajuda | Uso para acompanhamento de tarefas, sem domínio avançado da ferramenta |

---

## Soft skills

| Soft skill | Situação em que foi exercitada |
|---|---|
| Responsabilidade | O projeto envolvia informações com impacto em processo aduaneiro, exigindo cuidado com precisão e rastreabilidade |
| Pensamento crítico | Foi necessário entender limites da IA e estruturar o sistema para permitir revisão humana |
| Protagonismo técnico | Assumi partes centrais do backend, da implementação do RAG e da integração com Ollama |
| Colaboração | Trabalhei em conjunto com frontend, PO e demais integrantes para integrar o fluxo completo |
| Organização técnica | Como backend principal, precisei manter regras e estrutura coerentes para sustentar o produto |
| Resolução de problemas | O projeto exigiu lidar com documentos, extração de dados, sugestões de IA e exportação final |
| Comunicação | Precisei alinhar contratos de dados e regras com o time para evitar divergências entre interface e backend |
| Adaptabilidade | O uso de IA exigiu ajustes conforme testes, inconsistências e necessidades do cliente |

---

## Aprendizados

O quarto API me ensinou que projetos com inteligência artificial exigem mais do que apenas conectar um modelo ao sistema. É necessário pensar em fluxo, validação, revisão, armazenamento, confiabilidade e clareza das informações geradas.

Também aprendi que, em processos sensíveis, a automação deve apoiar o trabalho humano, não substituir completamente a responsabilidade de revisão. No caso do AdaTech, a IA ajudava a reduzir esforço manual e retrabalho, mas o sistema precisava permitir correções e validações antes da geração final.

Do ponto de vista técnico, aprofundei minha experiência em backend com Python e FastAPI, integração com banco de dados, criação de regras de negócio e comunicação entre diferentes partes da aplicação. A implementação de recursos envolvendo RAG e Ollama reforçou meu interesse por soluções que combinam backend, inteligência artificial e automação de processos reais.

---

## Links

- [Repositório do projeto](https://github.com/equipeAdalove/API-SEMESTRE4)


---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 3 • AdaTrade](./API_3.md) | — |

</div>
