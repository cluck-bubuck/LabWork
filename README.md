# ***Отчет по  лаборатоной работе***
+ *Создал репозиторий на компьютере*
```
git init
```

+ *Подлючился к удаленному репозиторию в GitHub*
```
git remote add origin https://github.com/cluck-bubuck/LabWork
```

+ *Загрузил изменения на сервер*
```
git add .
git commit -m “Cool commit“
git push origin master
```

+ *Проверил наличие добавленного коммита*
```
git log
```
> _Ответ от Git:_
```
   commit 1fafec0ebcd4da536b0383a0872b570866eb202e (HEAD -> master, origin/master)
Author: cluck-bubuck <127479787+cluck-bubuck@users.noreply.github.com>
Date:   Mon Mar 11 16:26:26 2024 +0500

    Cool Commit
```

+ *Просмотрел все ветки*
```
git branch
```
> _Ответ от Git:_
```
* master
```

+ *Создал еще одну ветку, проверил ее наличие и удалил ее*
```
git branch second
git branch

git branch -d second
git branch
```
> _Ответ от Git:_
```
* master
  second
```
> _Ответ2 от Git:_
```
Deleted branch second (was 1fafec0).
* master
```
+ *Проверил статус*
```
git status
```
> _Ответ от Git:_
```
On branch master
nothing to commit, working tree  clean
```

+ *Отменяю изменения в файле Редме файл.txt*
```
git checkout -- Редме файл.txt
```

+ *Клонировал репозиторий*
```
git clone https://github.com/cluck-bubuck/LabWork
```

+ *Зачем нужно ребазирование*
```
git rebase master
```
**git rebase** – команда, перемещающая все коммиты: от общего коммита двух веток до последнего коммита текущей ветки на вершину переданной ветки.

+ *Создал конфликт (вроде бы)*
*Создал ветку и внес изменения в файл*
```
git checkout main
echo "qwerty" >> Редме файл.txt
git add Редме файл.txt
git commit -m "main branch"
```
*Внес  изменения в другой ветке*
```
git checkout -b new-branch
echo "ytrewq" >> Редме файл.txt
git add Редме файл.txt
git commit -m "other branch"
```
+ *Создал 5 коммитов для Редме файл.txt*
###1
```
git commit -m "я"
git add .
```
> _Ответ от Git:_
```
[master 1fafec0]  я
1 file changet, 2 insperations(+)
```
###2
```
git commit -m "любл"
git add .
```
> _Ответ от Git:_
```
[master 1fafec0]  любл
1 file changet, 2 insperations(+)
```
###3
```
git commit -m "кодить"
git add .
```
> _Ответ от Git:_
```
[master 1fafec0]  кодить
1 file changet, 2 insperations(+)
```
###4
```
git commit -m "и"
git add .
```
> _Ответ от Git:_
```
[master 1fafec0]  и
1 file changet, 2 insperations(+)
```
###5
```
git commit -m "гитхаб"
git add .
```
> _Ответ от Git:_
```
[master 1fafec0]  гитхаб
1 file changet, 2 insperations(+)
```

+ *Сделал git merge - делает слияние веток, созданных git branch в одну*
```
git checkout master
git merge
```
+ *Отправил репозиторий в удаленный репозиторий*
```
git push origin master
```

+ *Отправил из удаленного репозитория обратно*
```
git pull origin master
```

+ *Создал новую ветку, закинул в нее файл и вроде как 26 пункт тут выполнил*
```
git checkout -b damnBr
git add another2.txt
git push origin damnBr
git pull origin damnBr:master
```
