# git-mistakes

Исправить ошибку в последнем коммите

```sh
➜ git commit --amend -m "Adding readme.md to git-mistakes"
```



Откатить файлы из `commit-a` в `Untracked` состояние

```sh
➜ git reset HEAD~1 // На одно изменение назад
```

```sh
➜ git reset xxx // На конкретный коммит
```



## Уровни отката изменений

1) Мягкий (не изменяется стратегия в git add .): --soft
```sh
➜ git reset --soft HEAD~1
```

2) Жесткий (все файлы в состояние `Untracked`): --mixed
```sh
➜ git reset --mixed HEAD~1
```

3) Опасный (удалит все файлы): --hard
