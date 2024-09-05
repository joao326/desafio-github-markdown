# Personalizando seu Codespace
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

GitHub Codespaces é um ambiente dedicado para você. Você pode configurar seus repositórios com um contêiner de desenvolvimento para definir seu ambiente GitHub Codespaces.

## Dicas para personalizar o seu codespace

Há muitas maneiras de personalizar seu Codespace. Vamos entender cada um deles:
- **Sincronização de configurações:** você pode sincronizar as configurações do Visual Studio Code (VS Code) entre o aplicativo de desktop e o cliente web do VS Code.
- **Dotfiles:** você pode usar um repositório
- para especificar scripts, preferências de shell e outras configurações.
- **Renomear um Codespace:** quando você cria um Codespace, ele recebe um nome de exibição gerado automaticamente. Se você tiver vários Codespaces, o nome de exibição ajudará a diferenciar entre Codespaces.
- **Alterar seu shell:** você pode alterar seu shell em um Codespace para manter a configuração com a qual está acostumado. Ao trabalhar em um Codespace, você pode abrir uma nova janela de terminal com um shell de sua escolha, alterar seu shell padrão para novas janelas de terminal ou instalar um novo shell. Você também pode usar dotfiles para configurar seu shell.
- **Alterar o tipo de máquina:** você pode alterar o tipo de máquina que está executando seu Codespace, para usar recursos apropriados para o trabalho que está realizando.
- **Definir o editor padrão:** você pode definir seu editor padrão para Codespaces em sua página de configurações pessoais. Defina sua preferência de editor para que, quando você criar um Codespace ou abrir um Codespace existente, ele seja aberto em seu editor padrão.
1. Código do Visual Studio (aplicativo de desktop)
2. Código do Visual Studio (aplicativo cliente da web)
3. JetBrains Gateway - para abrir Codespaces em um JetBrains IDE
4. JupyterLab - a interface web do Projeto Jupyter Definir a região padrão: você pode definir sua região padrão na página de configurações de perfil do GitHub Codespaces para personalizar onde seus dados são mantidos.
- **Defina o tempo limite:** um Codespace irá parar de funcionar após um período de inatividade. Por padrão, esse período é de 30 minutos, mas você pode especificar um período de tempo limite padrão maior ou menor em suas configurações pessoais no GitHub. A configuração atualizada se aplica a quaisquer novos Codespaces que você criar ou a Codespaces existentes na próxima vez que você iniciá-los.
- **Configurar exclusão automática:** Codespaces inativos são excluídos automaticamente. Você pode escolher por quanto tempo seus Codespaces interrompidos serão retidos, até um máximo de 30 dias.

## Adicione ao seu Codespace com extensões ou plugins

Você pode adicionar plug-ins e extensões em um Codespace para personalizar sua experiência no JetBrains e no VS Code.

## Extensões de código VS

Se você trabalhar em seus Codespaces no aplicativo de desktop VS Code ou no cliente Web, poderá adicionar quaisquer extensões necessárias do Visual Studio Code Marketplace. Consulte Suporte ao Desenvolvimento Remoto e Codespaces GitHub na documentação do VS Code para obter informações sobre como as extensões são executadas em Codespaces GitHub.

Se você já usa o VS Code, pode usar o Settings Sync para sincronizar automaticamente extensões, configurações, temas e atalhos de teclado entre sua instância local e quaisquer Codespaces que você criar.

## Plug-ins JetBrains

Se você trabalha em seus Codespaces em um IDE JetBrains, poderá adicionar plug-ins do JetBrains Marketplace.