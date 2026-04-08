# Multi-Agent Orchestration Boilerplate

Este repositório é um template de referência para instalar uma squad completa e autônoma de Agentes de IA dentro de qualquer projeto de software.

## 🏗️ A Squad

O framework abandona o conceito de um único assistente genérico e instaura uma equipe especializada (`agents/`):
* 🎯 **Product Owner**: Interface com o usuário. Refina regras de negócio e define os Critérios de Aceite (DoD).
* 👑 **Tech Lead**: Orquestrador Técnico. Transforma os requisitos do PO em tarefas arquiteturais e gerencia o time.
* 📐 **Architect**: Cuida da integridade do sistema e mantém a memória viva (`architecture.md`).
* 💻 **Dev Team**: Focado exclusivamente na escrita de código, testes unitários e refatoração.
* 🐛 **QA Specialist**: Focado em testes, auditoria de logs e isolamento de bugs (RCA).
* ⚙️ **Ops**: Responsável por CI/CD, dependências, build final e versionamento de entrega.

## 🚀 Instalação e Análise de Capacidade (Model Routing)

Para instalar este framework no seu projeto e garantir a orquestração perfeita:

1. **Injeção**: Copie todos os arquivos e pastas deste repositório (`agents/`, `skills/`, `agents.md`, etc.) para a raiz do seu projeto destino.
2. **Avaliação do LLM (Setup Inicial)**: Na sua IDE ou CLI de Agente, envie o seguinte comando inicial:
   > "Por favor, atue como o **Tech Lead** (`agents/techlead.md`). Analise os modelos de linguagem disponíveis no nosso ambiente (ex: Claude 3.5 Sonnet, GPT-4o, Opus). Aloque os modelos com maior capacidade de *Reasoning* para o **Product Owner**, para você e para o **Architect**. Aloque modelos mais rápidos (*Speed/Balanced*) para o **Dev Team**, **QA** e **Ops**. Em seguida, execute a skill `skills/core/bootstrap.md` para ajustar todo o framework à linguagem de programação deste repositório."

## 🛠️ O Ciclo de Delegação Autônoma

Os agentes possuem restrições rígidas e **não fazem o trabalho uns dos outros**. Se o usuário humano pedir uma nova funcionalidade, o fluxo será:

1. O **Product Owner** refina a ideia e cria a documentação de requisitos em `docs/features/`.
2. O **Tech Lead** lê os requisitos, aciona o **Architect** se necessário, e quebra a demanda técnica em `docs/tasks/`.
3. O **Tech Lead** delega a execução sequencial ao **Dev Team**.
4. O **Dev Team** codifica e aciona o **QA Specialist** para rodar a auditoria e os testes.
5. Passando nos testes, a bola vai para o **Ops**, que gera o build de release e atualiza o versionamento (`delivery.md`).
6. O **Tech Lead** invoca o `compound.md` para consolidar aprendizados em `guidelines.md`.
7. O **Product Owner** faz a validação final da entrega contra os critérios de aceite e notifica o usuário humano do sucesso.

---
*Este framework é agnóstico a linguagens e focado em orquestração multi-agente de alto desempenho.*
