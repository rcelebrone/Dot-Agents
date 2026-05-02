---
description: Setup inicial da squad — varre o repositório e popula a memória do projeto
---

Leia `.agents/rules/orchestrator.md` para entender o protocolo da squad.

Analise os modelos de linguagem disponíveis neste ambiente e aloque:
- **Reasoning Tier** (modelos mais capazes): Product Owner, Architect e Tech Lead
- **Speed Tier** (modelos mais rápidos): Dev Team, QA Specialist e Ops

Em seguida, execute a skill `skills/core/bootstrap/SKILL.md`: varra o repositório completo (manifestos, código-fonte, configurações) e popule os arquivos de memória em `.agents/memory/` com o contexto real do projeto — arquitetura, regras de negócio e guidelines de código.

Configure a squad de acordo com a ferramenta do usuário (cursor, claude, antigravity, gemini-cli, ou outra). Você precisará entender os padrões da ferramenta pra configurar de acordo.

Ao finalizar, confirme para o usuário quais stacks foram detectadas, qual personalidade foi escolhida para a squad e declare o setup concluído.
