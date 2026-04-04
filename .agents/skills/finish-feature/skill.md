Skill: Feature Completion & Deployment Preparation
1. Descrição Geral
Esta skill é acionada quando o desenvolvimento de uma funcionalidade ou correção de bug é finalizado. Ela garante a integridade do código através de testes, prepara o artefato de execução, atualiza a documentação de histórico e sincroniza o trabalho com o repositório remoto.
2. Gatilhos de Ativação (Triggers)
O agente deve invocar esta skill ao identificar frases como:
 * "Concluí a funcionalidade X"
 * "A feature Y está pronta"
 * "Finalizei as tarefas da branch"
 * "Pode subir as alterações"
3. Workflow de Fechamento (Passo a Passo)
Passo 1: Execução de Testes
O agente deve identificar a tecnologia do projeto e executar o comando de teste correspondente:
 * C# / .NET: dotnet test
 * JavaScript / Node: npm test ou yarn test
 * Dart / Flutter: flutter test
 * Rust: cargo test
Se os testes falharem, o agente deve interromper o processo e reportar os erros.
Passo 2: Geração de Executável ou Comando de Execução
Dependendo do tipo de projeto, o agente deve:
 * Gerar o build (ex: dotnet publish, npm run build, flutter build apk/ios, cargo build --release).
 * Caso seja um script ou biblioteca, apresentar explicitamente o comando para o usuário validar a execução manual.
Passo 3: Atualização do Changelog
O agente deve localizar o arquivo CHANGELOG.md na raiz do projeto e adicionar uma nova entrada sob a seção [Unreleased] ou criar uma nova versão, listando as alterações feitas baseadas nas tasks concluídas.
Passo 4: Incremento de Versão
O agente deve atualizar o arquivo de versão de acordo com o ecossistema:
 * C#: Atualizar <Version> ou <AssemblyVersion> no .csproj.
 * JavaScript: npm version patch (ou atualizar o package.json).
 * Dart: Atualizar o version no pubspec.yaml.
 * Rust: Atualizar o version no Cargo.toml.
Passo 5: Sincronização Remota
O agente deve realizar o commit final (caso haja mudanças no changelog/versão) e subir a branch:
git add .
git commit -m "chore: finalize feature and update version/changelog"
git push origin <nome-da-branch-atual>

4. Confirmação Final
Após o sucesso de todas as etapas, o agente deve emitir um relatório curto:
 * Status dos testes.
 * Localização do executável ou comando de execução.
 * Versão atualizada.
 * Link ou confirmação do push para o repositório.
 * 
