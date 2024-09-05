# Adentrando Detalhadamente o InnerSouce no Github
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

Vamos compreender o que é o InnerSouce e suas boas práticas.

## Introdução:

O desenvolvimento de software tradicionalmente se dividia entre dois modelos: código aberto e proprietário. O código aberto permite contribuições abertas, enquanto o software proprietário mantém-se fechado para proteger a propriedade intelectual.

Se você lidera uma empresa que investiu em software proprietário, pode querer combinar as vantagens do código aberto sem abrir completamente seu software. É aí que entra o InnerSource.

## Como gerenciar um programa InnerSource bem-sucedido


### >> O que é InnerSource?

O software de código aberto pode ser livremente usado, modificado e compartilhado por qualquer pessoa. Usando software de código aberto, qualquer pessoa pode visualizar, modificar e distribuir um projeto para qualquer finalidade, com a ideia de que compartilhar código leva a software melhor e mais confiável.

InnerSource é a prática de aplicar padrões de código aberto a projetos com um público limitado. Por exemplo, uma empresa pode estabelecer um programa InnerSource que espelha a estrutura de um projeto de código aberto típico, exceto que ele só é acessível aos funcionários dessa empresa. Na prática, é um programa de código aberto atrás do firewall da sua empresa.

### >> Benefícios do InnerSource

Um programa InnerSource pode oferecer inúmeros benefícios além dos modelos tradicionais de código fechado.

Primeiramente, eles incentivam a transparência. O acesso ao código-fonte de outros projetos da empresa pode ajudar os desenvolvedores a serem mais produtivos ao trabalharem em seus próprios projetos. Eles podem ver como diferentes equipes resolveram problemas semelhantes aos que estão enfrentando e muitas vezes encontrar código e outros recursos que podem reutilizar. O acesso a problemas da equipe, solicitações de pull e planos do projeto também fornece melhores dados para entender a velocidade e direção do projeto.

Em seguida, eles reduzem o atrito. Se uma equipe consumidora depende de uma correção de bug ou novo recurso para um projeto de propriedade de outra equipe, eles têm um canal por meio do qual podem propor as mudanças necessárias. E se essas mudanças não puderem ser mescladas por qualquer motivo, a equipe consumidora tem a opção de bifurcar o projeto para atender às suas necessidades.

Finalmente, eles padronizam práticas. Um desafio comum que as organizações de desenvolvimento enfrentam é que diferentes equipes frequentemente divergem nas formas como operam. Criar um programa InnerSource é uma ótima oportunidade para adotar convenções padrão que podem ser usadas em todas as equipes de desenvolvimento, mesmo que não sigam práticas idênticas. Por exemplo, duas equipes podem preferir processos diferentes para aceitar contribuições. Padronizá-las na forma como comunicam esses processos diferentes torna muito mais fácil para qualquer pessoa contribuir para ambas.


### >> Configurar visibilidade e permissões de repositório

Você pode configurar repositórios do GitHub com três níveis de visibilidade. Usuários que não atendem ao requisito de visibilidade veem páginas "não encontradas" ao tentar acessar seu repositório. Os níveis são:
- Repositórios públicos são visíveis para todos. Use esta visibilidade para projetos que são realmente de código aberto e oferecem acesso a pessoas dentro e fora de sua organização. 
- Repositórios internos são visíveis apenas para membros da organização que os possui. Use esta visibilidade para projetos InnerSource.
- Repositórios privados são visíveis apenas para o proprietário e quaisquer equipes ou indivíduos que eles adicionarem. Use esta visibilidade para projetos aos quais apenas usuários e grupos específicos devem ter acesso.

Depois de estabelecer a visibilidade do repositório, você pode configurar permissões individualmente ou por equipe. Existem cinco níveis de permissão:
- Nível de leitura é recomendado para contribuidores não programadores que desejam visualizar ou discutir o projeto.
- Nível de triagem é recomendado para contribuidores que precisam gerenciar proativamente problemas e solicitações de pull sem acesso de gravação.
- Nível de gravação é recomendado para contribuidores que empurram ativamente para o projeto.
- Nível de manutenção é recomendado para gerentes de projeto que precisam gerenciar o repositório sem acesso a ações sensíveis ou destrutivas.
- Nível de administrador é recomendado para pessoas que precisam de acesso total ao projeto, incluindo ações sensíveis e destrutivas, como gerenciar segurança ou excluir um repositório.

À medida que um programa InnerSource cresce, o número de repositórios provavelmente aumenta significativamente. Embora seja ótimo ter todos esses ativos disponíveis para a organização, pode se tornar um desafio encontrar e trabalhar eficientemente com o conteúdo. Para abordar proativamente esse problema, é uma prática recomendada para as equipes considerar o que podem fazer para facilitar a descoberta e o trabalho com seus repositórios por parte de outras pessoas.

Algumas melhores práticas incluem:
- Usar um nome descritivo para o repositório, como warehouse-api ou supply-chain-web.
- Incluir uma descrição concisa. Uma ou duas frases devem ser suficientes para que os usuários em potencial saibam se o projeto pode atender às suas necessidades.
- Licenciar seu repositório para que os usuários saibam como podem usar, modificar e distribuir o software.
- Incluir um arquivo README.md no repositório. O GitHub usa este arquivo como a página inicial quando as pessoas visitam o repositório.

## Boas Práticas

### Adicionar um arquivo README

Um arquivo README comunica as expectativas para o seu projeto e ajuda a gerenciar contribuições. Os arquivos README podem:
- Articular o propósito e a visão do projeto para que os consumidores em potencial entendam se atende às suas necessidades.
- Oferecer auxílios visuais, como capturas de tela ou trechos de código, para ilustrar o projeto em ação.
- Incluir links para uma versão de produção ou demo do aplicativo para revisão.
- Definir expectativas para pré-requisitos e procedimentos de implantação.
- Incluir referências aos projetos dos quais você depende. Essas referências são uma boa maneira de promover o trabalho de outros.
- Usar Markdown para orientar os leitores por meio de conteúdo formatado corretamente.

Se você colocar seu arquivo README no diretório oculto .github, docs ou no diretório raiz, o GitHub reconhece e exibe automaticamente seu README para visitantes do repositório. Se um repositório contiver mais de um arquivo README, o arquivo mostrado é escolhido em locais na seguinte ordem: o diretório .github, depois o diretório raiz do repositório e, finalmente, o diretório docs.

#### Confira alguns exemplos incríveis de README.

Depois que o projeto for lançado, use o e-mail e outros canais de networking para promovê-lo. Alcançar um público apropriado pode resultar em um impulso significativo na participação no projeto. Gerenciar projetos no GitHub

À medida que os projetos ganham tração, o influxo de usuários e contribuições pode exigir muito trabalho para gerenciar. Dependendo do projeto, pode ser necessário um esforço significativo apenas para gerenciar as expectativas dos participantes do projeto.

Para abordar proativamente esse problema, o GitHub procura um arquivo CONTRIBUTING.md na raiz (ou /docs ou /.github) de um repositório. Use este arquivo para explicar a política de contribuição para o projeto. Os detalhes exatos podem variar, mas é uma boa ideia informar aos potenciais contribuidores quais convenções o projeto segue, onde a equipe procura solicitações de pull, quais detalhes são solicitados para relatórios de bugs, etc.

Se um CONTRIBUTING.md existir, o GitHub apresenta um link para ele quando os usuários criam problemas ou solicitações de pull para incentivá-los a segui-lo.

#### >> Confira alguns exemplos incríveis de CONTRIBUTING.md.

Além disso, considere adicionar um arquivo CODEOWNERS ao repositório para definir indivíduos ou equipes responsáveis por revisar modificações de código. Criar modelos de problemas e solicitações de pull

O GitHub oferece modelos iniciais para novos problemas e solicitações de pull. Use-os para fornecer o texto de descrição inicial para um problema ou solicitação de pull recém-criado.

Por exemplo, se seu projeto tiver .github/ISSUE_TEMPLATE.md, sempre que um usuário iniciar o processo de criação de um problema, eles verão esse conteúdo. Em vez de ter que se referir constantemente aos detalhes necessários de um CONTRIBUTING.md, eles podem preencher o problema como um formulário usando o texto do modelo.

É o mesmo para solicitações de pull, exceto que o caminho é .github/PULL_REQUEST_TEMPLATE.md.

Confira alguns exemplos incríveis de modelos de problemas e solicitações de pull do GitHub.

### Definir fluxos de trabalho

Para projetos que incentivam contribuições externas, certifique-se de especificar qual fluxo de trabalho o projeto segue. O fluxo de trabalho deve incluir detalhes sobre onde e como os ramos devem ser usados para bugs e recursos, como as solicitações de pull devem ser abertas e quaisquer outros detalhes que as pessoas fora da equipe do repositório devem saber antes de enviar código. Se você ainda não tem um fluxo de trabalho em mente, deve considerar o fluxo de trabalho do GitHub.

Você deve comunicar uma estratégia para gerenciar lançamentos e implantações. Essas partes do fluxo de trabalho afetam o branching e merging diários, então é importante comunicá-las aos contribuidores. Saiba mais sobre como elas se relacionam com sua estratégia de branching do Git. Medir o sucesso do programa

Qualquer equipe que se aventura no InnerSource deve pensar nos tipos de métricas que deseja rastrear para avaliar o sucesso de seu programa. Embora métricas tradicionais como "tempo de lançamento no mercado" e "bugs relatados" ainda sejam aplicáveis, elas não necessariamente ilustram os benefícios obtidos por meio do InnerSource.

Em vez disso, considere adicionar métricas que mostrem como a participação externa melhorou a qualidade do projeto. O repositório está recebendo solicitações de pull de fontes externas que corrigem bugs e adicionam recursos? Existem participantes ativos nas discussões sobre o projeto e seu futuro? O programa está inspirando uma expansão do InnerSource que gera benefícios em outras partes da organização?

Em resumo, métricas são difíceis, especialmente quando se trata de medir o valor e o efeito das contribuições individuais e de equipe. Se mal utilizadas, as métricas podem prejudicar a cultura, os processos existentes e diminuir o sentimento coletivo em relação à organização ou à equipe de liderança. Ao pensar em medir a adoção do InnerSource, considere o seguinte:
- Meça o processo, não o resultado
    - Tempo de revisão de código
    - Tamanho da solicitação de pull
    - Trabalho em andamento
    - Tempo para abrir
- Meça em relação a metas e não absolutos
- Meça equipes e não indivíduos
    - Número de contribuidores únicos para um projeto
    - Número de projetos reutilizando código
    - Número de menções cruzadas entre equipes