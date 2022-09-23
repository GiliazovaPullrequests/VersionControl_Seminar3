Создали удаленный пустой (!) репозиторий на github: https://github.com/bogomolga/edu.git

**В VS Code выполняем следующие команды:**

```json
git remote add origin https://github.com/bogomolga/edu.git

origin - это мы так назвали наш длинный адрес "origin", т.е. origin="https://github.com/bogomolga/edu.git". Можно называть "origin2"

git branch -M main //говорим, что главная ветка у нас будет называться "main"
git push -u origin main //
```
**Терминал:**
```json
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git remote add origin https://github.com/bogomolga/edu.git
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git branch -M main
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git push -u origin main
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 220 bytes | 44.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0       
To https://github.com/bogomolga/edu.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push>
{code}
```

После этого файлы из локального репозитория появляются в удаленном репозитории на github.

Редактируем файл в удаленном репозитории и коммитим там же.

В локальном шлем команду git pull:

и
```json
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.34 KiB | 16.00 KiB/s, done.
From https://github.com/bogomolga/edu
   5764cc5..218b581  main       -> origin/main
Updating 5764cc5..218b581
Fast-forward
 readme.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push>
```

далее

```json
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git commit -am "edit"
[main 086eed1] edit
 1 file changed, 2 insertions(+)
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 252 bytes | 84.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bogomolga/edu.git
   218b581..086eed1  main -> main
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\pull_push>
```

**Делаем Fork:**

```json
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone> git clone https://github.com/bogomolga/VersionControl_Seminar3.git        
Cloning into 'VersionControl_Seminar3'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 2
Receiving objects: 100% (3/3), done.
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone> cd VersionControl_Seminar3
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\VersionControl_Seminar3> git branch
* main
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\VersionControl_Seminar3> git log
commit 0a2f089446a71a13190d16c244a104e293b1d899 (HEAD -> main, origin/main, origin/HEAD)
Author: GiliazovaPullrequests <110250115+GiliazovaPullrequests@users.noreply.github.com>
Date:   Fri Jul 29 21:09:54 2022 +0500

    Initial commit
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\VersionControl_Seminar3> git branch Bogomolova
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\VersionControl_Seminar3> git checkout Bogomolova
Switched to branch 'Bogomolova'
PS C:\Users\Olga\Documents\!Обучение GB\Введение в контроль версий\clone\VersionControl_Seminar3> git branch
* Bogomolova
  main
```