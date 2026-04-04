Skill: Dependency Guard & Security

1. Descrição

Monitora a saúde das dependências do projeto e sugere atualizações.

2. Comandos de Auditoria

JS: npm audit ou yarn audit

C#: dotnet list package --vulnerable

Dart: dart pub outdated

3. Workflow

Se encontrar vulnerabilidades críticas, criar automaticamente uma task de fix/security-patch.

Sugerir atualizações de minor versions para manter o projeto atualizado.
