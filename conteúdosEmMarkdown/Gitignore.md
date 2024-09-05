# Gitignore
 
 

O arquivo .gitignore é usado no Git para especificar quais arquivos e diretórios devem ser ignorados pelo controle de versão. Assim evitamos que arquivos desnecessários sejam incluídos no repositório.

## Estrutura do `.gitignore`:

O arquivo `.gitignore` é um simples arquivo de texto que lista padrões de nomes de arquivos e diretórios que o Git deve ignorar. Cada linha no arquivo representa um padrão a ser ignorado. Os padrões podem incluir curingas para coincidir com vários arquivos ou diretórios.

Exemplo de um arquivo `.gitignore` básico:

```
# Comentários começam com #
# Ignorar arquivos temporários
*.tmp

# Ignorar arquivos de log
*.log

# Ignorar diretório de compilação
/build/

# Ignorar arquivos de configuração local
config.local
```

## Como criar um arquivo `.gitignore`:
1. **Crie o arquivo:** Você pode criar o arquivo manualmente usando um editor de texto simples ou através do terminal usando comandos como `touch .gitignore` (no Linux/Unix) ou `New-Item .gitignore -type file` (no PowerShell do Windows).
2. **Edite o arquivo:** Adicione os padrões de arquivos e diretórios que você deseja ignorar, como no exemplo acima.

## Padrões de Ignoração:
- `*`: Corresponde a qualquer sequência de caracteres.
- `?`: Corresponde a qualquer caractere individual.
- `/`: Indica uma barra como separador de diretório (use para ignorar diretórios específicos).
- `#`: Indica um comentário.

### Exemplos Práticos:
1. Ignorar todos os arquivos `.class`:

```
*.class
```

2. Ignorar um diretório chamado `dist`:

```
dist/
```

3. Ignorar arquivos de configuração específicos:

```
config.local
config.dev
```


## Integração com Repositórios Existente:
Se você já iniciou um repositório Git e deseja adicionar um `.gitignore` posteriormente, faça o seguinte:
1. Crie o arquivo `.gitignore`.
2. Abra o terminal na raiz do seu repositório e execute
```
    git add .gitignore
    git commit -m "Adicionar arquivo .gitignore"
```
3. O arquivo `.gitignore` agora está no controle de versão e será aplicado aos arquivos e diretórios correspondentes.

Pessoal, o uso do `.gitignore` é uma prática importante para manter nosso repositório limpo e evitar a inclusão de arquivos desnecessários ou até mesmo dados sensíveis.

Por fim... Certifique-se de adaptar o conteúdo do `.gitignore` de acordo com os requisitos específicos do seu projeto.