# Formatação com o Markdown
 
 

Nesta aula, descobriremos a estrutura e a sintaxe do Markdown. Também veremos recursos do GitHub-Flavored Markdown (GFM), que são extensões de sintaxe que permitem integrar recursos do GitHub.

## Markdown

- linguagem de marcação que oferece uma abordagem simplificada para edição de conteúdo, protegendo os criadores de conteúdo das complexidades do HTML. 
- Enquanto o HTML é excelente para renderizar o conteúdo exatamente como foi pretendido, ele ocupa muito espaço e pode ser difícil de trabalhar, mesmo em pequenas doses. 
- A invenção do Markdown ofereceu um ótimo equilíbrio entre o poder do HTML para descrição de conteúdo e a facilidade do texto simples para edição.

## Estrutura e Sintaxe do Markdown

Nesta unidade, discutiremos a estrutura e a sintaxe do Markdown. Também abordaremos recursos do GitHub-Flavored Markdown (GFM), que são extensões de sintaxe que permitem integrar recursos do GitHub ao conteúdo.

## Sintaxe

### Enfatizar Texto

Usar itálico no texto é tão fácil quanto cercar o texto-alvo com um único asterisco (\*) ou um único sublinhado (\_). Certifique-se apenas de fechar uma ênfase com o mesmo caractere com o qual a abriu. Esteja atento à combinação de asteriscos e sublinhados. Aqui estão alguns exemplos:

```markdown
Isso é texto *itálico*.
Isso também é texto _itálico_.
```

Crie texto em negrito usando dois asteriscos (\*\*) ou dois sublinhados (\_\_).

```markdown
Isso é texto **negrito**.
Isso também é texto __negrito__.
```

Você também pode misturar diferentes ênfases.

```markdown
_Isso é texto **itálico e negrito**_ usando um único sublinhado para itálico e dois asteriscos para negrito.
__Isso é texto negrito e *itálico*__ usando dois sublinhados para negrito e um único asterisco para itálico.
```

Para usar um asterisco literal, anteceda-o com um caractere de escape; no GFM, isso é uma barra invertida (). Este exemplo resulta em sublinhados e asteriscos sendo mostrados na saída.

```markdown
\_Isso é todo \*\*texto\*\* simples\_.
```

### Declarar Cabeçalhos

HTML fornece cabeçalhos de conteúdo, como a tag `<h1>`. No Markdown, isso é suportado via símbolo #. Basta usar um # para cada nível de cabeçalho de 1 a 6.

```markdown
###### Isso é texto H6
```

### Link para Imagens e Sites

Links de imagem e site usam uma sintaxe semelhante.

```markdown
![Link de uma imagem.](/learn/azure-devops/shared/media/mara.png)
```

```markdown
[Link para o Treinamento da Microsoft](/training)
```


### Criar Listas

Você pode definir listas ordenadas ou não ordenadas. Também é possível definir itens aninhados por meio de indentação.

Listas ordenadas começam com números. Listas não ordenadas podem usar asteriscos ou traços (-).

Aqui está o Markdown para uma lista ordenada:

```markdown
1. Primeiro
1. Segundo
1. Terceiro
```

Resultado:

```markdown
    Primeiro
    Segundo
    Terceiro
```

```markdown
- Primeiro
  - Aninhado
- Segundo
- Terceiro
```

Aqui está o Markdown para uma lista não ordenada:

```markdown
    Primeiro
        Aninhado
    Segundo
    Terceiro
```

### Construir Tabelas

Você pode construir tabelas usando uma combinação de barras verticais (|) para quebras de coluna e traços (-) para designar a linha anterior como cabeçalho.

```markdown
Primeiro | Segundo
-|-
1 | 2
3 | 4
```

Resultado:

```markdown
    Primeiro 	Segundo
    1 	2
    3 	4
```


### Citar Texto

Você pode criar blocos de citação usando o caractere maior que (>).

```markdown
> Este é um texto citado.
```


### Preencher as lacunas com HTML inline

Se você se deparar com um cenário HTML não suportado pelo Markdown, pode usar HTML inline.

```markdown
Aqui está uma<br/>quebra de linha

    Aqui está uma
    quebra de linha
```

### Trabalhar com Código

Markdown fornece um comportamento padrão para trabalhar com blocos de código inline delimitados pelo caractere de crase (\`). Ao decorar o texto com este caractere, ele é renderizado como código.

```markdown
Isso é `código`.
```

Se você tiver um segmento de código abrangendo várias linhas, pode usar três crases (\`\`\`) antes e depois para criar um bloco de código cercado.

```markdown
var primeiro = 1;
var segundo = 2;
var soma = primeiro + segundo;
```

```csharp
var primeiro = 1;
var segundo = 2;
var soma = primeiro + segundo;
```

O GFM estende esse suporte com destaque de sintaxe para linguagens populares. Basta especificar a linguagem como parte da primeira sequência de crases.

```javascript
var primeiro = 1;
var segundo = 2;
var soma = primeiro + segundo;
```

### Vincular problemas e solicitações de pull

O GFM oferece suporte a vários formatos de shortcode para facilitar a vinculação a problemas e solicitações de pull. A maneira mais fácil de fazer isso é usar o formato #ID, como #3602. O GitHub ajusta automaticamente links mais longos para esse formato se você os colar. Existem também convenções adicionais que você pode seguir, se estiver trabalhando com outras ferramentas ou deseja especificar outros projetos/branches.

|Tipo de referência|Referência bruta|Link curto|
|---|---|---|
|URL do problema ou solicitação de pull|[https://github.com/desktop/desktop/pull/3602](https://github.com/desktop/desktop/pull/3602)|#3602|

## e número do problema ou solicitação de pull | #3602 | #3602

GH- e número do problema ou solicitação de pull | GH-3602 | GH-3602 Nome de usuário/Repositório# e número do problema ou solicitação de pull | desktop/desktop#3602 | desktop/desktop#3602

Para obter mais informações, consulte o artigo "Referências e URLs autolinked" na unidade de Resumo no final deste módulo.

## Vincular commits específicos

Você pode vincular a um commit colando seu ID ou simplesmente usando seu algoritmo hash seguro (SHA).

|Tipo de referência|Referência bruta|Link curto|
|---|---|---|
|URL do commit|https://github.com/desktop/desktop/commit/8304e9c271a5e5ab4fda797304cd7bcca7158c87|8304e9c|
|SHA|8304e9c271a5e5ab4fda797304cd7bcca7158c87|8304e9c|
|Usuário@SHA|desktop@8304e9c271a5e5ab4fda797304cd7bcca7158c87|desktop@8304e9c|
|Nome de usuário/Repositório@SHA|desktop/desktop@8304e9c271a5e5ab4fda797304cd7bcca7158c87|desktop/desktop@8304e9c|


## Mencionar usuários e equipes

Digitar um símbolo @ seguido de um nome de usuário do GitHub envia uma notificação para essa pessoa sobre o comentário. Isso é chamado de "@mention", porque você está mencionando o indivíduo. Você também pode @mencionar equipes dentro de uma organização.

```markdown
@githubteacher
```

## Rastrear listas de tarefas

Você pode criar listas de tarefas dentro de problemas ou solicitações de pull usando a seguinte sintaxe. Isso pode ser útil para acompanhar o progresso quando usado no corpo de um problema ou solicitação de pull.

```markdown
- [x] Primeira tarefa
- [x] Segunda tarefa
- [ ] Terceira tarefa
```

## Comandos de barra

Comandos de barra podem economizar tempo, reduzindo a digitação necessária para criar Markdown complexo.

Você pode usar comandos de barra em qualquer campo de descrição ou comentário em problemas, solicitações de pull ou discussões onde esse comando de barra é suportado.

| Comando        | Descrição                                                                                                                                                                                      |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| /code          | Insere um bloco de código Markdown. Você escolhe o idioma.                                                                                                                                     |
| /details       | Insere uma área de detalhes expansível. Você escolhe o título e o conteúdo.                                                                                                                    |
| /saved-replies | Insere uma resposta salva. Você escolhe entre as respostas salvas para sua conta de usuário. Se adicionar %cursor% à sua resposta salva, o comando de barra coloca o cursor nessa localização. |
| /table         | Insere uma tabela Markdown. Você escolhe o número de colunas e linhas.                                                                                                                         |
| /tasklist      | Insere uma lista de tarefas. Este comando de barra só funciona em uma descrição de problema.                                                                                                   |
| /template      | Mostra todos os modelos no repositório. Você escolhe o modelo a ser inserido. Este comando de barra funciona para modelos de problema e um modelo de solicitação de pull.                      |
