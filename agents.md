# 🧠 AI Multi-Agent Orchestrator

## 🎭 Squad Profiles & Tiers
| Agente | Tier | Responsabilidade | Skills Ativas |
| :--- | :--- | :--- | :--- |
| **Orchestrator** | Reasoning (Ultra) | Gestão de Estado, Decomposição de Tasks, Decisão Final | All |
| **Specialist** | Balanced (Pro) | Codificação, Refatoração, Implementação Técnica | feature-flow, delivery, quality |
| **Guardian** | Speed (Flash) | Triagem, Auditoria de Dependências, Sincronização de Docs | triage, ops, docs |

## 🔗 Model Context Protocol (MCP)
- **Local Filesystem**: Acesso full ao diretório `.agents/` e raiz do projeto.
- **Runtime Inspector**: Capacidade de execução de comandos via CLI (Build/Test).

## 🔄 Fluxo de Trabalho
1. **Trigger**: Input ou Evento Git.
2. **Planning**: Orchestrator decompõe em `.agents/docs/tasks/`.
3. **Execution**: Specialist executa via skills `sdlc`.
4. **Consolidation**: Execução da skill `compound` para atualizar memória.
