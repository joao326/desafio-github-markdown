# Permissões do Github
 
 

Nesta aula, abordaremos sobre as permissões de nível hierárquico dentro do github.

## O níveis que abordaremos, será:
- Permissões de repositório
- Permissões de equipe
- Permissões da organização
- Permissões da empresa

### Permissões de Repositório

Nas permissões de repositório há cinco tipos diferentes, sendo eles:
1. **Leitura:** Para quem só precisa visualizar ou discutir o projeto, sem fazer modificações.
2. **Triagem:** Para gerenciar problemas e solicitações sem poder fazer alterações. Ideal para alguns gerentes de projeto.    
3. **Gravação:** Para colaboradores que ativamente contribuem ao fazer "push" no projeto. A permissão padrão para desenvolvedores.
4. **Manutenção:** Para gerentes de projeto que precisam gerenciar o repositório, mas sem acesso a ações críticas.
5. **Administrador:** Acesso total ao projeto, incluindo ações críticas. Indicado para administradores e proprietários de repositórios.

Você pode atribuir diferentes níveis de acesso a membros, colaboradores externos e equipes em sua organização, escolhendo o nível apropriado para cada pessoa ou função sem conceder mais acesso do que necessário. Depois de configurar permissões corretas em um repositório, você pode usá-lo como modelo para criar novos repositórios com a mesma estrutura e arquivos.

#### Para criarmos um modelo:
1. No GitHub.com, acesse a página principal do repositório.
2. Abaixo no nome do repositório, selecione **Configurações**. Se você não conseguir ver a guia **Configurações**, abra o menu suspenso e escolha **Configurações**.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FWvU8mQZZegLHNkuxixHw%252Fmodelopermis%25C3%25B5es.png%3Falt=media%26token=7f01b2cd-b5a1-4bbb-b676-11adbb2be799&width=768&dpr=4&quality=100&sign=19a825bef675f7e0edb42fe4902d86e3083844e76f106032e1ff20da7419c594)

##### **Repositório de modelos**
1. Selecione **Repositório de modelos**.

### Permissões de Equipe

As equipes facilitam a atribuição de permissões em vários usuários de uma vez. Membros herdam permissões da equipe pai, simplificando a propagação de autorizações com base na estrutura da empresa.

Dois níveis de permissão em equipes:
1. **Membro:** Mesmas habilidades dos membros da organização.
2. **Mantenedor:** Pode fazer tudo que membros fazem e mais, como alterar nome, adicionar membros e gerenciar revisões de código.

O dono da organização pode promover qualquer membro a mantenedor de uma equipe. Para auditar o acesso a um repositório, é possível ver uma lista de equipes e usuários com acesso nas configurações.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252Fw4YMeoXZFj1zdpNXheUo%252FN%25C3%25ADveis%2520de%2520permiss%25C3%25A3o%2520da%2520equipe.png%3Falt=media%26token=fd915cb3-435c-4680-8238-d4c52deb3c45&width=768&dpr=4&quality=100&sign=2c295a2f54d454104f9ca7b986bc73c88599ba3ac4df231b777592e50ad8c029)

### Permissões da Organização

1. **Proprietário:** Faz tudo que membros fazem e pode adicionar/remover usuários. Geralmente, são duas pessoas no máximo.
2. **Membro:** Cria e gerencia repositórios e equipes da organização.
3. **Moderador:** Bloqueia/desbloqueia colaboradores, estabelece limites de interação e esconde comentários em repositórios públicos.
4. **Gerente de Cobrança:** Visualiza e edita informações de cobrança.
5. **Gerente de Segurança:** Gerencia alertas de segurança e configurações em toda a organização, lê permissões de todos os repositórios.
6. **Colaborador Externo:** Pode acessar um ou mais repositórios, não sendo membro explícito da organização.

Além disso, também é possível definir permissões padrão para todos os membros da organização.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FwDc8yPmp8wwT7id602vC%252Forg-base-permissions.png%3Falt=media%26token=10094c5d-78fd-4944-a8a6-b9040b365cee&width=768&dpr=4&quality=100&sign=b327013edb58df28eeafc362f2d7a2ab67dd6ae52bdcac1d45857de6845084ee)

Por fim, para melhorar o gerenciamento e a segurança, também é possível conceder permissões de leitura padrão a todos os membros da sua organização e ajustar o acesso aos repositórios de acordo com cada caso.

### Permissões da Empresa

Por extensão, cada conta de usuário individual que é membro de uma organização também é membro da empresa, e você pode controlar várias configurações relacionadas à autenticação por meio desse nível mais alto.

Há três níveis de permissão no âmbito da empresa:
1. **Proprietário Corporativo:** Controle total, pode gerenciar administração, adicionar/remover organizações, configurar políticas, cobrança e mais.
2. **Membro Corporativo:** Mesmas habilidades dos membros da organização.
3. **Gerente de Cobrança Corporativo:** Vê/edita informações de cobrança e adiciona/remove outros gerentes de cobrança.

Além desses níveis, é possível definir uma política padrão para permissões de repositório em todas as organizações.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FEqT1KxeBys7dCbwD0GnO%252Fpermissoes-padrao.png%3Falt=media%26token=12c3ab2f-ce15-46be-afdc-a910685a6c45&width=768&dpr=4&quality=100&sign=3f8c644ed209be404fa61a15314cff9c08c00a8acd37c617235a497c05b42c56)

Buscando melhorar o gerenciamento e a segurança, você pode conceder permissões de leitura padrão a todos os membros da sua empresa e ajustar o acesso aos repositórios caso a caso.

## Segurança e Gerenciamento de Repositórios

### **Regras de Proteção de Branch:**
- Controle as alterações no repositório.
- Exija aprovações, pull requests, commits assinados e mais.
- Defina regras para todos, incluindo administradores.
- Restrinja quem pode fazer push para branches.

### **Arquivo CODEOWNERS:**
- Atribua membros ou equipes como proprietários de código.
- Eles são automaticamente solicitados como revisores em pull requests que afetam seu código.

### **Visualizar Tráfego com Insights:**
- Qualquer um com acesso de push pode ver:
    - Clones completos.
    - Visitantes recentes.
    - Referências de sites.
    - Conteúdo popular.

#### Para acessar o grafo de tráfego:
1. No GitHub.com, acesse a página principal do repositório.
2. No nome do repositório, selecione **Insights**.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252F290g3wHZKNtbqKe9OfHK%252Finsigts.png%3Falt=media%26token=9fce23ce-663e-4d3f-9d70-5abd7aa093d8&width=768&dpr=4&quality=100&sign=872a75047a77f98ef248c3d3ff050147ea1de180119cfbd6270dc19a72d7d3e8)

1. À esquerda, selecione **Tráfego:**

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252Fwh3P9kGbEMGdFGvfrCf7%252Ftraffic-tab.png%3Falt=media%26token=06262f6f-b51f-444d-bd46-7e42c95b9fd2&width=768&dpr=4&quality=100&sign=aee25ba1d5b2816ede7dfe13ade75f093865bd272630c328ed6c677fd526fe22)

Opcionalmente, selecione **Clones** ou **Exibições** para ver o grafo de tráfego de clones ou exibições.