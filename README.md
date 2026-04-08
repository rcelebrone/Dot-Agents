# Multi-Agent Orchestration Boilerplate

Este repositório é um template de referência para instalar uma squad completa e autônoma de Agentes de IA dentro de qualquer projeto de software.

## 🏗️ A Squad

O framework abandona o conceito de um único assistente e instaura uma equipe (`agents/`):
* **Tech Lead**: Orquestra e fatia demandas.
* **Architect**: Cuida da integridade (`architecture.md`).
* **Dev Team**: Focado em código.
* **QA Specialist**: Testes e Triagem.
* **Ops**: CI/CD, dependências e entrega.

## 🚀 Instalação e Análise de Capacidade (Model Routing)

Para instalar este framework no seu projeto e garantir a orquestração:

1. **Injeção**: Copie os arquivos e pastas (`agents/`, `skills/`, `agents.md`, etc) para a raiz do seu repositório.
2. **Avaliação do LLM (Setup Inicial)**: Na sua IDE ou CLI de Agente, envie o comando:
   > "Por favor, atue como o **Tech Lead** (`agents/techlead.md`). Analise os modelos de linguagem disponíveis no nosso ambiente (ex: Claude 3.5 Sonnet, GPT-4o, Opus). Aloque os modelos com maior capacidade de *Reasoning* para você e para o **Architect**, e modelos mais rápidos para o **QA** e **Ops**. Em seguida, execute o `skills/core/bootstrap.md` para ajustar as skills à linguagem de programação deste repositório."

## 🛠️ O Ciclo de Delegação Autônoma

Os agentes são instruídos a **não fazerem o trabalho uns dos outros**. Se o usuário pedir uma feature, o fluxo será:
1. O **Tech Lead** cria as tarefas em `docs/tasks/`.
2. O **Tech Lead** delega a escrita ao **Dev Team**.
3. O **Dev Team** finaliza e aciona o **QA Specialist** para rodar os testes.
4. Passando nos testes, o **Ops** executa o fechamento (`delivery.md`).
5. O **Tech Lead** invoca o `compound.md` para consolidar o aprendizado em `guidelines.md` e avisa o usuário que o épico foi concluído.
