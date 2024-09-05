# Introdução ao Codespace
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

Vamos entender um pouco sobre o ciclo de vida do Codespace

GitHub Codespaces é um ambiente de desenvolvimento totalmente configurado e hospedado na nuvem. Ao usar GitHub Codespaces, seu espaço de trabalho, juntamente com todos os seus ambientes de desenvolvimento configurados, ficam disponíveis em qualquer computador com acesso à Internet. Objetivos de aprendizado

## O Ciclo de vida do Codespace

GitHub Codespaces é configurável, permitindo criar um ambiente de desenvolvimento personalizado para o seu projeto. Ao configurar um ambiente de desenvolvimento customizado para o seu projeto, você pode ter uma configuração de Codespace repetível para todos os usuários do seu projeto.

O ciclo de vida de um Codespace começa quando você cria um Codespace e termina quando você o exclui. É possível desconectar e reconectar-se a um Codespace ativo sem afetar seus processos em execução. Você pode parar e reiniciar um Codespace sem perder as alterações feitas em seu projeto.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252F0mOv1u7GJq9nSZ8jMhoA%252Fcodespace-circular-lifecycle.png%3Falt=media%26token=13237f86-3a8e-491c-a338-a9523f5b907f&width=768&dpr=4&quality=100&sign=165bef82832d58fd72c8ecadd9953e783a858f0e8ed8dbe9f2818a1d728b350b)

## Crie um codespace

Você pode criar um Codespace em GitHub.com, no Visual Studio Code ou pelo GitHub CLI. Existem quatro maneiras de criar um Codespace:
- A partir de um modelo GitHub ou de qualquer repositório de modelos em GitHub.com para iniciar um novo projeto.
- De uma ramificação em seu repositório para novos recursos funcionarem.
- De uma solicitação pull aberta para explorar o trabalho em andamento.
- De um commit no histórico de um repositório para investigar um bug em um momento específico.

Você pode usar temporariamente um Codespace para testar o código ou pode retornar ao mesmo Codespace para trabalhar em recursos de longa duração.

Você pode criar mais de um Codespace por repositório ou até mesmo por branch. No entanto, há limites para o número de Codespaces que você pode criar e executar ao mesmo tempo. Se você atingir o número máximo de Codespaces e tentar criar outro, será exibida uma mensagem informando que um Codespace existente precisa ser removido/excluído antes que um novo Codespace possa ser criado.

Você pode criar um novo Codespace sempre que desenvolver em GitHub Codespaces ou manter um Codespace de longa duração para um recurso. Se estiver iniciando um novo projeto, crie um Codespace a partir de um modelo e publique-o posteriormente em um repositório no GitHub.

Ao criar um novo Codespace sempre que trabalhar em um projeto, você deve enviar regularmente suas alterações para garantir que quaisquer novos commits estejam no GitHub. Ao usar um Codespace de longa execução para um novo projeto, extraia da ramificação padrão do repositório sempre que começar a trabalhar no Codespace. Isso permite que o ambiente obtenha os commits mais recentes. O fluxo de trabalho é semelhante a trabalhar com um projeto em uma máquina local.

Os administradores de repositório podem habilitar pré-compilações do GitHub Codespaces para um repositório para acelerar a criação do Codespace.

Para obter instruções detalhadas e orientações passo a passo, consulte os recursos intitulados Um guia para iniciantes para aprender a codificar com GitHub Codespaces e Desenvolvendo em um Codespace localizados na unidade Resumo no final deste módulo.

## Processo de criação de um Codespace:

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FFZbHEPBwpStLrQ2d4LLb%252Fcodespace-connection-editor.png%3Falt=media%26token=65b14bf2-8e61-41eb-b6ec-6076e9bcaa44&width=768&dpr=4&quality=100&sign=7343fa72498f644fe7a663a80d2c37712c084c9f2989f163af08d7addefacf90)

When creating a GitHub Codespace, four processes occur:
1. VM and storage are assigned to your Codespace. 
2. A container is created.
3. A connection to the Codespace is made.
4. A post-creation setup is made.

## Salvar alterações em um Codespace

Quando você se conecta a um Codespace pela web, o AutoSave é ativado automaticamente para salvar as alterações após um período de tempo específico. Ao se conectar a um Codespace por meio do Visual Studio Code em execução em sua área de trabalho, você deve habilitar o AutoSave.

Seu trabalho é salvo em uma máquina virtual na nuvem. Você pode fechar e parar um Codespace e retornar ao trabalho salvo posteriormente. Se você tiver alterações não salvas, receberá uma solicitação para salvá-las antes de sair. No entanto, se o seu Codespace for excluído, seu trabalho será perdido. Para salvar seu trabalho, você deve confirmar suas alterações e enviá-las para seu repositório remoto ou publicar seu trabalho em um novo se você criou seu Codespace a partir de um modelo. Abra um Codespace existente

Você pode reabrir qualquer um dos seus Codespaces ativos ou interrompidos em GitHub.com, em um IDE JetBrains, no Visual Studio Code ou usando GitHub CLI.

Para retomar um Codespace existente, você pode ir ao repositório onde o Codespace existe e pressionar a tecla "," no teclado e selecionar Retomar este codespace ou abrir https://github.com/codespaces no navegador, selecionar o repositório e em seguida, selecione o Codespace existente.

## Tempos limite para um codespace

Se um Codespace estiver inativo ou se você sair do Codespace sem parar explicitamente, o aplicativo expirará após um período de inatividade e interromperá a execução. O tempo limite padrão é após 30 minutos de inatividade. Não é possível personalizar a duração do período de tempo limite para novos Codespaces. Quando um Codespace expira, seus dados são mantidos desde a última vez que suas alterações foram salvas.

## Conexão com a Internet ao usar GitHub Codespaces

Um Codespace requer uma conexão com a Internet. Se a conexão com a Internet for perdida enquanto você trabalha em um Codespace, você não conseguirá acessar seu Codespace. No entanto, quaisquer alterações não confirmadas serão salvas. Ao restabelecer a conexão com a Internet, você poderá acessar o Codespace no mesmo estado em que estava quando a conexão foi perdida.

Se você tiver uma conexão de Internet instável, você deve confirmar e enviar suas alterações com frequência.

## Fechar ou parar um Codespace

Se você sair do Codespace sem executar o comando stop (por exemplo, fechando a guia do navegador) ou deixar o Codespace em execução sem interação, o Codespace e seus processos em execução continuarão durante o período de tempo limite de inatividade. O período de tempo limite de inatividade padrão é de 30 minutos. Você pode definir sua configuração de tempo limite pessoal para Codespaces criados, mas isso pode ser anulado pela política de tempo limite de uma organização.

Apenas a execução de Codespaces incorre em cobranças de CPU. Um Codespace parado incorre apenas em custos de armazenamento.

Você pode parar e reiniciar um Codespace para aplicar alterações. Por exemplo, se você alterar o tipo de máquina usado para seu Codespace, será necessário interrompê-lo e reiniciá-lo para que a alteração entre em vigor. Quando você fecha ou interrompe seu Codespace, todas as alterações não confirmadas são preservadas até que você se conecte ao Codespace novamente.

Você também pode interromper o Codespace e optar por reiniciá-lo ou excluí-lo se encontrar um erro ou algo inesperado.

## Reconstruir um codespace

Você pode reconstruir seu Codespace para implementar alterações na configuração do contêiner de desenvolvimento. Para a maioria dos usos, é possível criar um novo Codespace como alternativa à reconstrução de um Codespace. Ao reconstruir seu Codespace, as imagens do cache aceleram o processo de reconstrução. Você também pode executar uma reconstrução completa para limpar o cache e reconstruir o contêiner com imagens novas.

Ao reconstruir o contêiner em um Codespace, as alterações feitas fora do diretório /workspaces são limpas. As alterações feitas dentro do diretório /workspaces, incluindo o clone do repositório ou modelo a partir do qual você criou o Codespace, são preservadas durante uma reconstrução.

## Excluir um codespace

Você pode criar um Codespace para uma tarefa específica. Depois de enviar suas alterações para uma ramificação remota, você poderá excluir esse Codespace com segurança.

Se você tentar excluir um Codespace com commits git não enviados, o editor notificará que há alterações que não foram enviadas para uma ramificação remota. Você pode enviar quaisquer alterações desejadas e excluir seu Codespace. Você também pode continuar excluindo seu Codespace e quaisquer alterações não confirmadas ou exportar o código para uma nova ramificação sem criar um novo Codespace.

Codespaces interrompidos que permanecem inativos por um período de tempo especificado são excluídos automaticamente. Codespaces inativos são excluídos após 30 dias, mas você pode personalizar os intervalos de retenção do Codespace.