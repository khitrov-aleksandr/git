# Откат законченного rebase
```bash
   git reset --hard ORIG_HEAD
```

# Пример отката изменений с удалением коммитов
1. Делаем hard reset до нужного коммита:
```bash
   git reset --hard 8c80dd7682fe894c2e972e52985dd28e299fae23
```
1. Делаем force push на удалённый репозиторий:
```bash
   git push -f origin master
```
# Игнорирование переноса строки
Актуально для phpStorm
Отключаем отслеживание переносов строки:
```bash
   git config --global core.autocrlf false
```
Удаляем закешированный индекс:
```bash
   git rm --cached -r .
```
Сбрасываем состояние до последнего коммита:
```bash
   git reset --hard
```
# Изменить существующий комит
```bash
   git commit --amend
```
# Трэк удалённой ветки
```bash
git branch --track test origin/test
```
# Сбросить мердж
```bash
git reset --merge
```
# Показать удалённые ветки
```bash
git branch -r
git branch -a
git branch -vv
```
# Удаление локальной ветки
```bash
   git branch -d ci
```
```bash
   git branch -D ci
```
# Push новой ветки
```bash
   git push --set-upstream origin gitignore
```
# Изменить имя пользователя и e-mail
```bash
   git config user.name "khitrov.av"
```
```bash
   git config user.email "khitrov.aleksandr@gmail.com"
```
# Удалить локальные изменения
```bash
   git stash save --keep-index --include-untracked
```
# Добавить удалённый репозиторий
```bash
   git remote set-url --add --push origin ssh://git@gitverse.ru:2222/cruiser/git.git
```