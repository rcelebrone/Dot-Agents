# DotAgents — Multi-Agent Orchestration Boilerplate

Template agnóstico para instalar uma squad multi-agente (PO, Architect, Tech Lead, Developer, QA, Security, Ops) em qualquer projeto que use ferramentas de orquestração de agentes.

A squad é regida por um **orquestrador central**, tem **personas** com responsabilidades claras, **skills** reutilizáveis e uma **memória viva** específica do projeto.

---

## 🚀 Instalação

Dentro do projeto onde você quer instalar a squad, clone este repositório como `DotAgents/`:

```bash
git clone https://github.com/rodrigo-celebrone/DotAgents.git DotAgents
```

Em seguida, execute o script de instalação correspondente à sua ferramenta:

### Gemini-CLI
```bash
./DotAgents/instalador-gemini-cli.sh
```

### Antigravity
```bash
./DotAgents/instalador-antigravity.sh
```

### Claude Code
```bash
./DotAgents/instalador-claude.sh
```

### Cursor AI
```bash
./DotAgents/instalador-cursor.sh
```

Cada script copiará os agentes, skills e comandos para as pastas esperadas por cada ferramenta (`.gemini/`, `{{AGENTS_ROOT}}/`, `.claude/` ou `.cursor/`), tornando-os disponíveis no seu fluxo de trabalho.

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
