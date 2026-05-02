---
description: Setup inicial da squad — varre o repositório e popula `.agents/memory/` com o contexto real do projeto.
---

Leia `.agents/workflows/orchestrator.md` para entender o protocolo da squad antes de prosseguir.

Aloque os modelos por tier:
- **Reasoning Tier** (modelos mais capazes): Product Owner, Architect, Tech Lead, **Security Specialist**.
- **Speed Tier** (modelos mais rápidos): Developer, QA Specialist, Ops.

Execute a skill `.agents/skills/core/bootstrap/SKILL.md`: varra o repositório completo (manifestos, código-fonte, configurações, infra) e popule:
- `.agents/memory/business.md` — regras de negócio, terminologia de domínio, fluxos de permissão.
- `.agents/memory/architecture.md` — stack, NFRs, arquitetura macro, modelo de ameaças, controles de segurança ativos.
- `.agents/memory/guidelines.md` — padrões de código, lint, antipadrões, vulnerabilidades remediadas, **tom da squad**.

> Nota: a configuração da ferramenta de orquestração (Claude Code, Cursor, Antigravity, Gemini-CLI, etc.) é responsabilidade do instalador raiz `agent.md`, não deste workflow. Se este workflow foi acionado isoladamente em um projeto onde os symlinks ainda não existem, oriente o usuário a digitar `configure DotAgents` primeiro.

Ao finalizar, confirme ao usuário:
1. Stacks detectadas (linguagem, framework, banco, CI/CD).
2. Personalidade escolhida pela squad.
3. Setup concluído — pronto para receber a primeira demanda.
