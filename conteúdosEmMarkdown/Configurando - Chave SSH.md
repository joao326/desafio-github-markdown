# Configurando - Chave SSH
status:: #zettel/fleeting 
tags:: #DIO/git #Programação/Git 

Chaves SSH são como chaves especiais que ajudam as pessoas a se conectarem a computadores remotos de forma segura, sem precisar sempre digitar senha ou token.

## Passo a Passo - Prático:

### 1. Verificar se você já possui uma chave SSH

Antes de gerar uma nova chave SSH, verifique se você já possui uma. No terminal, execute o seguinte comando:

```
ls -al ~/.ssh
```

Se você já tiver uma chave SSH, normalmente os arquivos terão nomes como `id_rsa` (chave privada) e `id_rsa.pub` (chave pública).

### 2. Gerar uma nova chave SSH (se necessário)

Se você não tiver uma chave SSH ou desejar gerar uma nova, use o seguinte comando:

```
ssh-keygen -t rsa -b 4096 -C "seu_email@example.com"
```

- `-t rsa`: Especifica o tipo de chave (RSA).
    
- `-b 4096`: Define o número de bits na chave (4096 bits é uma boa prática para maior segurança).
    
- `-C "seu_email@example.com"`: Adiciona um comentário para ajudar a identificar a chave (substitua pelo seu e-mail do GitHub).
    

Pressione Enter para aceitar o caminho padrão do arquivo (`~/.ssh/id_rsa`) e, se desejar, configure uma senha para a chave.

### 3. Adicionar a chave SSH ao agente SSH (opcional)

Para facilitar a gestão das chaves, você pode adicionar a chave ao agente SSH:

```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

### 4. Observações adicionais
- É possível adicionar uma senha a chave privada para adicionar mais uma camada de segurança, para isso:
#### Gerar nova chave com senha:
```
ssh-keygen -t rsa -b 4096 -C "seu_email@example.com"
```
#### Adicionar uma senha a uma chave existente
```
ssh-keygen -p -f ~/.ssh/sua_chave_privada
```
Substitua `sua_chave_privada` pelo caminho e nome do arquivo da sua chave privada atual.