# Resumão sobre Github
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

Nesta aula, recordaremos as noções básicas do Github para que possamos compreender melhor seus recursos e produtos fundamentais.

## Atenção:

Lembrando que iremos apenas recapitular os conceitos já visto no curso de Introdução ao Git e ao Github.

## Github

Como já vimos anteriormente, o Github é uma plataforma em nuvem que utiliza o Git como núcleo. Ela possibilita que nosso processo de colaboração de projetos seja mais simples e nos fornece ferramentas de linha de comando, além de outras funcionalidade que permitem que devs e usuários colaborem juntos.

O Github também oferece uma plataforma de desenvolvimento com IA para a criação, escala e entregas de softwares seguros.
## Github e a IA

A IA generativa está se interligando a várias áreas e ferramentas, possibilitando uma melhor produtividade em vários ramos e claro, no desenvolvimento de software não seria diferente.

A plataforma do Github também utiliza a IA e está cada vez mais aprimorando a colaboração por meio de problemas e pull requests da plataforma AI, além da melhoria na produtividade com o Copilot e a segurança com automatização de verificações de segurança de forma mais rápida.
## Colaboração

Como percebemos o Github tem como principal característica a colaboração e com as ferramentas disponibilizadas essa colaboração torna-se mais simples e ocorrendo sem muito esforço. Como os repositórios e pull requests, possibilitam que diversas pessoas (sejam devs, gerenciadores de projeto, lideres, etc) possam trabalhar mais rapidamente, reduzindo assim, o tempo de aprovação. Resultando em entregas eficientes e de forma mais rápida.

## Produtividade

Com ferramentas internas de CI/CD que são integradas ao fluxo de trabalho, a produtividade passa a ser acelerada com essa automação. O Github oferece um cuidado com a administração das rotinas e acelera o trabalho diário.

## Segurança

A plataforma oferece recursos de segurança nativos e internos minimizando o risco de segurança com soluções criadas internamente. Ele permite que nossos códigos fiquem privados até mesmo dentro das nossas organizações

## Escala

O Github é a MAIOR comunidade de Devs, com isso a plataforma compreende bem as necessidades de melhorias/mudanças com isso é feito alterações essenciais no produto. A plataforma possui compreensão que alteram o setor, funcionalidades de colaboração, ferramentas para ampliar a produtividade, segurança e a IA para ampliar toda essa gama de funcionalidades oferecidas.

_______________________________________________________________________

## O que é um repositório?

Um repositório é o local onde contém todos os arquivos do nosso projeto. Seria como uma pastinha que guarda todos esses arquivos de nossos projeto, como os nossos projetos de software. É com eles que podemos colaborar, gerenciar nosso trabalho, acompanhar as alterações, armazenar o histórico de alterações, etc...

## O que são Branches?

Branches são pontos seguros em nosso código, onde podemos criar várias branches(pontos/ramos) com copias ou partes do nosso código, nessas branches podemos fazer alterações de bugs e features de forma segura, sem alterar a branche principal. Dessa forma, podemos fazer as alterações/correções de bugs e outras implementações sem alterar nosso código padrão. Podemos então depois, mesclar as alterações estáveis na nossa branche principal.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FMKOsSofoEKPWplGD3Qxr%252FGitHub-Flow-1.png%3Falt=media%26token=9d5c4d98-5f17-40f2-b5c7-d7ff91ba4d95&width=768&dpr=4&quality=100&sign=1cab03890199a30a0caf4d068e2364a392b25d750e1cea73cbc1f6b435ab5452)

## O que são os Commits?

Quando adicionamos um arquivo em nosso repositório é precisamos adicionar um commit via push, com um texto breve informando do que se trata aquele alteração. Sempre que um commit for criado, ele recebe um ID próprio e é acompanhado juntamente com o tempo e quem realizou o commit (o colaborador). Os commits nos possibilitam um melhor acompanhamento de forma clara para qualquer pessoa que esteja revisando o histórico de um arquivo ou até mesmo um item vinculado, como um problema ou uma solicitação de pull.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252F4DkgDWpPcANjsP7uIy6N%252Fcommits.png%3Falt=media%26token=cc58c580-705a-42e2-8f2f-5e16a59a7458&width=768&dpr=4&quality=100&sign=e547538eecc3298af340ca2559103faa9f5b83bacea4478d57815af6a0c99555)

Já dentro de um repositório Git, um arquivo pode existir com vários estados válidos. Os estados primários são:
1. Não rastreado: O arquivo é rastreado, mas não foi modificado desde a última confirmação;
2. Rastreado: O Rastreado é aquele que o Git está monitorando ativamente, a "imagem" então pode está em um dos subestados a seguir:
	- Não modificado: O arquivo é rastreado, mas não foi modificado desde a última confirmação;
	- Modificado em: O arquivo foi alterado desde o ultimo commit, no entanto, essas alterações não foram preparadas para o próximo commit;
	- Preparado: O arquivo foi modificado e as alterações foram adicionadas à área de preparo;
	- Confirmado: O arquivo está no [[banco de dados]] do repositório

## E as solicitações de Pull - Pull Request?

A solicitação de pull é basicamente um pedido para que outras pessoas vejam suas mudanças e decidam se elas devem ser adicionadas ao projeto principal ou não. Ao passar pelos revisores do projeto, eles podem comentar, fazer sugestões de correções e até mesmo discutir sobre as alterações. Quando todos concordam que as mudanças são validas é feito então a mesclagem no projeto principal. Em resumo, uma solicitação de pull é um pedido de permissão para que seja adicionados as alterações ao projeto, passando por revisão para garantir que tudo esteja correto antes da mesclagem.

![](https://aline-antunes.gitbook.io/~gitbook/image?url=https:%2F%2F74136188-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F2HZbEqnaq1Y4YcnxMtW1%252Fuploads%252FrKknhdsmdmZ4eOQsWFzM%252Fsolicitacao%2520de%2520pull.png%3Falt=media%26token=eaaf341d-1e44-468c-80c4-15e1ebe50f8c&width=768&dpr=4&quality=100&sign=8a6c483aeb86c975f69cf89bc8020ce5e21c724838e956a42a01d58900c16267)

## Gists

Os gists assemelham-se aos repositórios, sendo uma forma mais simples de compartilhar trechos de códigos com outras pessoas. Já que eles se assemelham aos repositórios podemos criar fork e clona-los, podendo ser publico ou privado. Onde os públicos ficam disponíveis para outras pessoas e os privados não podem ser pesquisados e outras pessoas não podem visualiza-los.

**Link do Gists:** [https://gist.github.com/](https://gist.github.com/)

## Wikis

As wikis fazem parte dos repositórios e há uma sessão onde podemos hospedar as documentações. Podemos usar o wiki do repositório para compartilhar conteúdos ao decorrer do nosso projeto. Com as wikis podemos fornecer documentação adicional.