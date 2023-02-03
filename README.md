# Начальная работа с системой контроля версий 
## Значение команд в **git** 

* **git --version** - команда для проверки версии git

* **git init** - инициализируем пустой репозиторий

* **git status** - проверяем текущее состояние файлов

* **git add** имя_файла_с_расширением - добовляем версионость файлу

* **git add .** - добавляем версионность всем файлам в папке

* **git commit -m** "сообщение" - команда для фиксации изменений файлов

* **git commit -am** "Сообщение" - фиксация изменений, не требует git add .

* **git diff** - вывод изменений на текущий момент по отношению к последнему коммиту

* **git log** - вывод истории коммитов в хронологическом порядке

* **git checkout** хэш_коммита - переход между изменениями

* **git checkout master** - возврат к текущему состоянию

* **git checkout** название_ветки - переход в другую ветку

* **git checkout -b** имя_ветки - создаёт и сразу переходит в созданую ветку

* **git branch** - показывает все ветки в репозитории, а также в какой ветке мы находимся на данный момент

* **git branch** названин_ветки - создаёт новую ветку

* **git branch -d** названин_ветки -удаляет выбраную ветку

* **git merge** название_ветки - проводит слияние двух веток (_при слиянии нужно нажодиться в той ветке которая будет главной_)

* **git log --graph** - показывает все коммиты из всех веток

* **git clone ссылка** - команда для загрузки удалённого репозитория

* **git push** - команда для отправки из локального репозитория в удалённый

* **git pull** - команда для подгрузки изменений из удалённого репозитория в локальный

