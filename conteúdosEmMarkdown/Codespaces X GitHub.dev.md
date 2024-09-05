# Codespaces X GitHub.dev
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

Você provavelmente está se perguntando: quando devo usar GitHub Codespaces e quando devo usar GitHub.dev?

Você pode usar GitHub.dev para navegar em arquivos e repositórios de código-fonte do GitHub e fazer e confirmar alterações de código. Você pode abrir qualquer repositório, bifurcação ou pull request no editor GitHub.dev.

Se você quiser fazer um trabalho mais pesado, como testar seu código, use GitHub Codespaces. Ele possui computação associada para que você possa construir seu código, executá-lo e ter acesso ao terminal. GitHub.dev não contém computação. Com GitHub Codespaces, você obtém o poder de uma máquina virtual (VM) pessoal com acesso ao terminal, da mesma forma que usaria seu ambiente local, apenas na nuvem. Comparação de Codespaces e GitHub.dev

A tabela a seguir lista as principais diferenças entre Codespaces e GitHub.dev:

| | GitHub.dev | GitHub Codespaces |
|---|---|---|
| **Custos** | Free | Cota mensal gratuita de uso para contas pessoais |
| **Disponibilidade** | Disponível para todos em GitHub.com | Disponível para todos em GitHub.com |
| **Comece** | GitHub.dev abre instantaneamente com o pressionar de uma tecla e você pode começar a usá-lo imediatamente, sem ter que esperar pela configuração ou instalação | Quando você cria ou retoma um Codespace, uma VM é atribuída ao Codespace e o contêiner é configurado com base no conteúdo de um arquivo devcontainer.json. Esta configuração leva alguns minutos para criar o ambiente de desenvolvimento. |
| **Computação** | Não há computação associada, portanto você não pode criar e executar seu código ou usar o terminal integrado. | Com GitHub Codespaces, você obtém o poder de uma VM dedicada para executar e depurar seu aplicativo. |
| **Acesso ao terminal** | Nenhum | GitHub Codespaces fornece um conjunto comum de ferramentas por padrão, o que significa que você pode usar o Terminal exatamente como faria em seu ambiente local. |
| **Extensões** | Apenas um subconjunto de extensões que podem ser executadas na Web aparece na visualização de extensões e pode ser instalado | Com GitHub Codespaces, você pode usar a maioria das extensões do Visual Studio Code Marketplace. |

## Continue trabalhando com o Codespaces

Você pode iniciar seu fluxo de trabalho em GitHub.dev e continuar trabalhando em um Codespace. Se você tentar acessar a visualização Run, Debug ou o Terminal, você será notificado de que eles não estão disponíveis em GitHub.dev.

Para continuar seu trabalho em um Codespace, selecione Continuar trabalhando em…. Selecione Criar novo codespace para criar um codespace em sua ramificação atual. Antes de escolher esta opção, você deve confirmar quaisquer alterações.