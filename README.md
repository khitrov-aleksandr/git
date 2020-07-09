# git
## Игнорирование переноса строки
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
## Трэк удалённой ветки
```bash
git branch --track test origin/test
```
## Сбросить мердж
```bash
git reset --merge
```
## Показать удалённые ветки
```bash
git branch -r
git branch -a
git branch -vv
```
## Удаление локальной ветки
```bash
   git branch -d ci
```
```bash
   git branch -D ci
```
## Push новой ветки
```bash
   git push --set-upstream origin gitignore
```
## Изменить имя пользователя и e-mail
```bash
   git config user.name "khitrov.av"
```
```bash
   git config user.email "khitrov.aleksandr@gmail.com"
```
## Удалить локальные изменения
```bash
   git stash save --keep-index --include-untracked
```
