# Tokens de Acesso Pessoal
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

O token de acesso pessoal do GitHub é uma forma de autenticação usada para acessar recursos e realizar ações na plataforma GitHub em nome de um usuário.


## Passo a Passo - Prático:

**Passo 1: Crie um Token de Acesso Pessoal**

1. Acesse o GitHub e vá para "Settings" (Configurações) do seu perfil.
2. No menu lateral, selecione "Developer settings" (Configurações do desenvolvedor).
3. Clique em "Personal access tokens" (Tokens de acesso pessoal) e depois em "Generate token" (Gerar token).
4. Siga as instruções para configurar as permissões necessárias e clique em "Generate token" no final.
5. Copie o token gerado.

**Passo 2: Clone um Repositório Usando o Token**

1. Abra o Git Bash no seu computador.
2. No terminal, use o seguinte comando para clonar um repositório usando o token:

```
git clone https://SEU_TOKEN_AQUI@github.com/seu-usuario/seu-repositorio.git
```

Substitua `SEU_TOKEN_AQUI` pelo token que você copiou e `seu-usuario/seu-repositorio.git` pelo caminho do repositório que você deseja clonar.

Por exemplo:

```
git clone https://seu-token-aqui@github.com/seu-usuario/meu-projeto.git
```