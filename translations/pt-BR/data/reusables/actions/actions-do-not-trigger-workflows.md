When you use the repository's `GITHUB_TOKEN` to perform tasks, events triggered by the `GITHUB_TOKEN` will not create a new workflow run. Isso impede que você crie execuções de fluxo de trabalho recursivo. Por exemplo, se um fluxo de trabalho executar código pushes usando o `GITHUB_TOKEN`, um novo fluxo de trabalho não será executado mesmo quando o repositório contém um fluxo de trabalho configurado para ser executado quando ocorrerem eventos `push`.