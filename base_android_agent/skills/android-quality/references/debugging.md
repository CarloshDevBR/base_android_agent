# Debugging Android

1. Reproduza o problema quando possível e preserve a mensagem completa.
2. Identifique a primeira causa relevante, arquivo e linha.
3. Formule uma hipótese apoiada por evidência.
4. Se houver autorização para corrigir, faça a menor alteração relacionada.
5. Execute novamente o comando ou cenário que falhou.
6. Amplie a investigação somente se a falha persistir.

Não faça várias alterações especulativas ao mesmo tempo. Se o pedido for apenas diagnosticar,
apresente causa, evidências e correção sugerida sem modificar arquivos.

## Inspeção do projeto

Execute `sh scripts/inspect-project.sh <diretório>` quando módulos, plugins ou comandos de validação
não estiverem claros. O script apenas lê arquivos do projeto e não executa Gradle.
