# API 6 - Synapse

<p align="center">
  <strong>6º Semestre • 2026-2</strong><br>
  Aplicação web inteligente para definição e simulação de regras de negócio por voz<br>
  Papel exercido no Scrum: <strong>A confirmar pelo aluno</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Plataforma%20Web-informational?style=for-the-badge" alt="Plataforma Web">
  <img src="https://img.shields.io/badge/Foco-IA%20e%20Regras%20de%20Neg%C3%B3cio-success?style=for-the-badge" alt="IA e regras de negócio">
  <img src="https://img.shields.io/badge/Entrega%20prevista-03%2F12%2F2026-orange?style=for-the-badge" alt="Entrega prevista para 03/12/2026">
</p>

> **Documentação para o TG II:** relatório baseado no README do Synapse fornecido para esta atualização, com entrega programada para 03/12/2026. As funcionalidades são apresentadas como escopo proposto, pois o material não informa seu estado de conclusão. Papel Scrum, stack de implementação, contribuições e autoavaliação individuais estão sinalizados para preenchimento.

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
| Tipo de sistema | Aplicação web inteligente |
| Papel no Scrum | [PREENCHER: papel exercido pelo aluno no 6º API] |
| Equipe | Titus Systems |
| Público previsto | Profissionais de recursos humanos, gestores e auditores |
| Situação documentada | Projeto com desenvolvimento previsto de 07/09/2026 a 22/11/2026 e entrega programada para 03/12/2026 |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | [Dom Rock](https://www.domrock.net/) |
| Pontos focais | Luiz Otavio e Andre Almeida |
| Contexto do desafio | Estruturação de regras de negócio, simulação de impacto financeiro e rastreabilidade das decisões |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

Empresas lidam com mudanças frequentes em produtos, preços, acordos comerciais e campanhas de comissionamento. Quando as regras dessas operações não são registradas de forma estruturada, parte do conhecimento permanece tácita, dificultando sua preservação, aplicação consistente e auditoria.

O desafio do Synapse é transformar a definição dessas regras em um processo mais acessível e rastreável. Além de capturar a intenção do usuário, a solução precisa permitir a avaliação de impactos financeiros e tornar compreensível o caminho entre a regra recebida, seu processamento e o resultado da simulação.

No recorte do backlog, **regra de negócio** corresponde ao conjunto de parâmetros que define o comissionamento após o alcance de uma meta de vendas.

---

<a id="solucao"></a>

<br>

## ✅ Solução

O **Synapse** é proposto como uma aplicação web na qual o usuário define regras de negócio por **comandos de voz**. A inteligência artificial deve interpretar a intenção e convertê-la em código processável, permitindo simular o impacto financeiro da regra e compará-lo com o cenário de referência da empresa, denominado *baseline*.

A proposta inclui a validação dos parâmetros recebidos, a sugestão de adaptações quando houver incompatibilidade ou inviabilidade orçamentária e o registro das informações utilizadas no processo. A explicação das decisões do modelo generativo e a geração de relatórios integram o escopo de transparência e auditoria.

### Funcionalidades previstas no backlog

| Funcionalidade | Finalidade | Sprint planejada |
|---|---|---|
| Simulação dos resultados da regra | Verificar a viabilidade dos parâmetros de comissionamento | 1 |
| Relatório após o processamento | Registrar a regra finalizada e sua simulação para consulta posterior | 1 |
| Captura de voz e transcrição | Facilitar a entrada da regra de negócio | 2 |
| Sugestão automática de adaptações | Propor ajustes diante de incompatibilidade dos parâmetros | 2 |
| Validação dos dados recebidos por voz | Confirmar os parâmetros antes da simulação | 2 |
| Registro dos dados processados | Permitir a verificação das fontes e do fluxo da simulação | 3 |
| Explicação das decisões tomadas | Oferecer transparência aos resultados e apoio à auditoria | 3 |

As sprints indicadas representam o planejamento presente no README; não equivalem à confirmação de implementação ou homologação de cada funcionalidade.

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Evento | Data ou período previsto |
|---|---|
| Kick-off | 26/08/2026 |
| Desenvolvimento | 07/09/2026 a 22/11/2026 |
| Feira de Soluções / entrega programada | 03/12/2026 |

### Documentação das sprints

- [Sprint 1](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-1.md)
- [Sprint 2](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-2.md)
- [Sprint 3](https://github.com/Titus-System/synapse/blob/main/sprints/sprint-3.md)

Esses endereços constam no README fornecido. O conteúdo dos relatórios de sprint não integra o material utilizado nesta atualização.

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório principal e documentação do Synapse](https://github.com/Titus-System/synapse)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

O README fornecido apresenta imagens de identificação e roadmap, mas não inclui uma demonstração da aplicação em funcionamento.

**[PREENCHER: inserir vídeo, GIF ou capturas de tela de uma entrega do Synapse, identificando a sprint e as funcionalidades demonstradas.]**

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

O README descreve os recursos técnicos da solução, mas não identifica linguagens, frameworks, banco de dados, provedor de transcrição ou modelo de inteligência artificial. Por isso, esses recursos são apresentados abaixo separadamente da stack de implementação a confirmar.

### Recursos técnicos descritos na proposta

| Recurso | Aplicação prevista |
|---|---|
| Interface web | Interação do usuário com a definição e a simulação de regras |
| Captura de voz e transcrição | Conversão da entrada falada em conteúdo utilizável no fluxo |
| Inteligência artificial generativa | Interpretação da intenção, conversão em código processável e sugestão de adaptações |
| Simulação de impacto financeiro | Comparação dos resultados da regra com o baseline da empresa |
| Validação de parâmetros | Conferência dos dados recebidos antes da simulação |
| Registro e explicação do processamento | Rastreabilidade dos dados e transparência das decisões |
| Geração de relatórios | Histórico das regras e dos resultados das simulações |

### Stack de implementação — a completar

| Camada | Informação a confirmar no código ou na documentação técnica |
|---|---|
| Frontend | [PREENCHER: linguagem, framework e principais bibliotecas] |
| Backend | [PREENCHER: linguagem, framework e organização dos serviços] |
| Dados | [PREENCHER: banco de dados e persistência do histórico] |
| Voz | [PREENCHER: ferramenta ou serviço de captura e transcrição] |
| Inteligência artificial | [PREENCHER: modelo, provedor e bibliotecas efetivamente utilizados] |
| Qualidade e execução | [PREENCHER: ferramentas de testes, ambiente e implantação] |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

**Pendente de preenchimento pelo aluno:** o README fornecido não informa o papel individual de Matheus Germano nem atribui entregas a integrantes específicos. O relato deve distinguir atividades concluídas de responsabilidades ou entregas ainda previstas.

| Aspecto do relato | Informação a completar |
|---|---|
| Papel no Scrum | [PREENCHER: papel exercido e eventuais mudanças durante o semestre] |
| Escopo de atuação | [PREENCHER: módulos, responsabilidades e participação nas sprints] |
| Entregas concluídas | [PREENCHER: funcionalidades, testes, correções ou documentação produzidos] |
| Desafio e decisão técnica | [PREENCHER: problema enfrentado, alternativas e solução adotada] |
| Resultado e evidências | [PREENCHER: resultado observado e links de commits, pull requests, issues ou demonstrações] |
| Atividades em andamento | [PREENCHER: pendências pessoais e situação na data da entrega do portfólio] |

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar a autoavaliação técnica a completar</strong></summary>

<br>

Relacionar competências efetivamente exercitadas às entregas individuais. Informar o nível de proficiência no padrão dos relatórios anteriores, como “Sei fazer com autonomia” ou “Faço com ajuda”.

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

Registrar exemplos pessoais com contexto, ação e resultado. Situações de comunicação com a equipe, entendimento das regras de negócio ou análise crítica dos resultados da IA podem ser utilizadas quando tiverem sido vivenciadas pelo aluno.

| Soft skill | Exemplo pontual no projeto |
|---|---|
| [PREENCHER: competência exercitada] | [PREENCHER: situação, ação pessoal e resultado] |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

**[PREENCHER — reflexão pessoal sobre o 6º API.]** Explicar o aprendizado obtido nas atividades já realizadas, um desafio técnico ou de colaboração e a relação dessa experiência com a evolução ao longo do curso.

O contexto do Synapse permite discutir a transformação de linguagem natural em regras processáveis, a validação de parâmetros, a comparação de cenários e a explicação de decisões de inteligência artificial. A reflexão final deve selecionar os temas ligados à atuação individual e considerar o estágio real do projeto na entrega do TG II.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 5 • SyncDesk](./API_5.md) | — |

</div>
