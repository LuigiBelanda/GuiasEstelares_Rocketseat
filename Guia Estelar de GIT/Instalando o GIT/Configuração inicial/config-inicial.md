# Configuração Inicial

Essa configuração você fará apenas uma vez por computador e o efeito se manterá após atualizações.

Você também pode mudá-las em qualquer momento rodando esses comandos novamente

## Sua identidade 

Assim que instalar o git, abra o terminal e digite:

```
git config --global user.name "Seu nome completo aqui entre aspas"

git config --global user.email seuemailaqui@dominio.com.br
```

**Isto é importante porque cada commit usa essa informação, e ela é carimbada de forma imutável nos commits que você começa a criar**

Se você quiser substituir essa informação com nome diferente para um projeto específico, você pode rodar o comando sem a opção `--global` dentro daquele projeto

# Editor

Você poderá trocar o editor padrão, que é o **vim**, por outro

```
git config --global core.editor "code -w"
```

# Ver configurações

Você poderá verificar suas configurações com o comando abaixo

```
git config --list
```

## Git config 

- Permite ver e atribuir variáveis de configuração como nome e email
- Estas variáveis podem ser armazenadas em três lugares diferentes:
    - ``/etc/gitconfig``: válido para todos os usuários no sistema e todos os seus repositórios. Se você passar a opção ``--system`` para ``git config``, ele lê e escreve nesse arquivo
    -  ``~/.gitconfig`` ou ``~/.config/git/config``: Somente para seu usuário. Você pode fazer o git ler e escrever neste arquivo passando a opção ``--global``
    - ``config`` no diretório Git (ou seja, ``.git/config``) de qualquer repositório que você esteja usando: específico para este repositório

```
Cada nível sobrescreve os valores no nível anterior, ou seja, valores em .git/config prevalecem sobre /etc/gitconfig
```
