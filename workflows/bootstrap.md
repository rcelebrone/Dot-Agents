---
description: Setup inicial da squad — varre o repositório e popula a memória do projeto
---

Leia `.agents/rules/orchestrator.md` para entender o protocolo da squad.

Atue como o **Tech Lead** (`.agents/rules/techlead.md`).

Analise os modelos de linguagem disponíveis neste ambiente e aloque:
- **Reasoning Tier** (modelos mais capazes): Product Owner, Architect e Tech Lead
- **Speed Tier** (modelos mais rápidos): Dev Team, QA Specialist e Ops

Em seguida, acione o **Product Owner** para executar `skills/core/bootstrap/SKILL.md`: varra o repositório completo (manifestos, código-fonte, configurações) e popule os arquivos de memória em `.agents/memory/` com o contexto real do projeto — arquitetura, regras de negócio e guidelines de código.

Ao finalizar, confirme para o usuário quais stacks foram detectadas, qual personalidade foi escolhida para a squad e declare o setup concluído.
