# DotAgents — Multi-Agent Orchestration Boilerplate

Template agnóstico para instalar uma squad multi-agente (PO, Architect, Tech Lead, Developer, QA, Security, Ops) em qualquer projeto que use ferramentas de orquestração de agentes.

A squad é regida por um **orquestrador central**, tem **personas** com responsabilidades claras, **skills** reutilizáveis e uma **memória viva** específica do projeto.

---

## 🚀 Instalação

Primeiro, clone este repositório como `DotAgents/` dentro do seu projeto:

```bash
git clone https://github.com/rodrigo-celebrone/DotAgents.git DotAgents
```

Agora, siga as instruções de acordo com a ferramenta que você utiliza:

### ♊ Gemini-CLI
#### 1. Execute o instalador
```bash
./DotAgents/instalador-gemini-cli.sh
```
#### 2. 🤖 Prompt para o LLM
> "Você agora está equipado com a squad **DotAgents**. Localize os arquivos de configuração em `.gemini/` e execute o workflow de inicialização descrito em `commands/bootstrap.md`. Assuma as personas de **Tech Lead**, **Architect** e **Product Owner** para analisar o projeto e preencher os arquivos em `memorys/` com a stack técnica, regras de negócio e guidelines detectados. 
> 
> **Validação de Formatação:** Utilize as documentações oficiais: 
> - [Skills](https://geminicli.com/docs/cli/skills/)
> - [Subagents](https://geminicli.com/docs/core/subagents/)
> - [Custom Commands](https://geminicli.com/docs/cli/custom-commands/)
> Para garantir que todos os agents, skills e commands da squad em `.gemini/` estejam com a formatação e metadados corretos para esta ferramenta."

---

### 🚀 Antigravity
#### 1. Execute o instalador
```bash
./DotAgents/instalador-antigravity.sh
```
#### 2. 🤖 Prompt para o LLM
> "Você agora está equipado com a squad **DotAgents**. Localize os arquivos de configuração em `.gemini/` e execute o workflow de inicialização descrito em `commands/bootstrap.md`. Assuma as personas de **Tech Lead**, **Architect** e **Product Owner** para analisar o projeto e preencher os arquivos em `memorys/` com a stack técnica, regras de negócio e guidelines detectados.
> 
> **Validação de Formatação:** Utilize as bases da Antigravity (D-O-E Framework) para garantir que as Directives e a Orchestration da squad em `.gemini/antigravity/` estejam alinhadas com os padrões de artefatos e execução da ferramenta. Consulte se necessário: https://antigravity.google/docs (ou documentação interna disponível)."

---

### ❄️ Claude Code
#### 1. Execute o instalador
```bash
./DotAgents/instalador-claude.sh
```
#### 2. 🤖 Prompt para o LLM
> "Você agora está equipado com a squad **DotAgents**. Localize os arquivos de configuração em `.claude/` e execute o workflow de inicialização descrito em `commands/bootstrap.md`. Assuma as personas de **Tech Lead**, **Architect** e **Product Owner** para analisar o projeto e preencher os arquivos em `memorys/` com a stack técnica, regras de negócio e guidelines detectados.
> 
> **Validação de Formatação:** Utilize a documentação oficial da Anthropic para [Claude Code](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code) para validar se os **Subagents** em `.claude/agents/` e as **Skills** em `.claude/skills/` (seguindo o padrão `SKILL.md`) estão corretamente estruturados com o frontmatter e metadados exigidos."

---

### 🖱️ Cursor AI
#### 1. Execute o instalador
```bash
./DotAgents/instalador-cursor.sh
```
#### 2. 🤖 Prompt para o LLM
> "Você agora está equipado com a squad **DotAgents**. Localize os arquivos de configuração em `.cursor/` e execute o workflow de inicialização descrito em `commands/bootstrap.md`. Assuma as personas de **Tech Lead**, **Architect** e **Product Owner** para analisar o projeto e preencher os arquivos em `memorys/` com a stack técnica, regras de negócio e guidelines detectados.
> 
> **Validação de Formatação:** Utilize as diretrizes oficiais do Cursor para [Custom Rules](https://docs.cursor.com/context/rules-for-ai) e `.cursorrules` para garantir que as definições dos agentes e instruções da squad estejam otimizadas para o indexador do Cursor e para a integração com o Chat/Composer."

---

## 🏗️ A Squad

| Persona | Responsabilidade |
|---|---|
| 🎯 **Product Owner** | Refina regras de negócio, define DoD. |
| 🏛️ **Architect** | Integridade sistêmica, ADRs. |
| 👑 **Tech Lead** | Triagem técnica, criação de tasks, coordenação ágil. |
| 💻 **Developer** | Implementação Clean Code + TDD. |
| 🧪 **QA Specialist** | Validação funcional, RCA de bugs. |
| 🔒 **Security Specialist** | Threat modeling, AppSec audit. |
| 🚀 **Ops** | Ciclo de entrega local, deploy. |

---

## 📁 Estrutura

- `agents/`: Definições das personas.
- `skills/`: Habilidades especializadas.
- `commands/`: Workflows e orquestração.
- `memorys/`: Memória viva (Business, Architecture, Guidelines).

---

## 📄 Licença

Consulte o arquivo [`license.md`](license.md) para detalhes sobre os termos de uso.
