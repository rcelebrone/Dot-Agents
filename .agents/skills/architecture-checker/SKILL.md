Skill: Architecture Consistency Checker

1. Descrição

Valida se o novo código respeita as camadas definidas no projeto (Clean Architecture / Onion Architecture).

2. Regras por Stack

C# / .NET: Domínio não deve referenciar Infra; Camada de Application não deve conhecer UI.

Dart / Flutter: Camada de Data não deve vazar para a UI; Respeitar uso de BLoC/Cubit ou Riverpod.

JS / TS: Evitar dependências circulares; Garantir separação de controllers e services.

3. Workflow

Executar análise estática de dependências antes de marcar uma task como concluída.

Reportar se houver "vazamento" de lógica de banco de dados para a camada de visualização.
