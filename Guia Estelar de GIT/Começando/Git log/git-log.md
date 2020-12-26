# Git Log

Mostra a história dos commits (autores, datas, branch que usamos etc)

Exemplos de git log:

```
git log 

git log --oneline

git log --n 5

git log --since=2020-10-01

git log --until=2020-10-01

git log --author=Mayk

git log --grep="init"
```

- ``git log``, traz todos as informações mais necessárias
- ``git log --oneline``, traz menos informações
- ``git log -n 5``, traz apenas 5 logs, o números de logs exibidos pode mudar
- ``git log --since=2020-10-01``, traz todos os commits feitos depois da data colocada
- ``git log --until=2020-10-01``, traz todos os commits antes da data colocada
- ``git log --author=Mayk``, traz todos os commits dos usuários que se chamam "Mayk"
- ``git log --grep="init"``, traz todos os commits com a mensagem que você quiser, nesta caso ele irá pegar todos os commits que tem "init" na mensagem
