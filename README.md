# _Инструкция для **Git**_

![Изображение логотипа git](Git_1.jpg)
## Что такое Git?
Git - это одна из реализаций распределенных систем контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.

> **Система контроля версий** — это система, записывающая изменения в файл или набор файлов в течение времени и позволяющая вернуться позже к определённой версии.
___
## Подготовка репозитория
Для создания локального репозитория необходимо выполнить команду *__git init__* в папке с репозиторием. 

### Git add
Для добавления изменений в коммит используется команда *__git add__*. Чтобы использовать команду *git add*, напишите *git add имя_файла_с_расширением* или *git add .* для всех файлов в текущей папке. 

### Создание коммитов
Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *__git commit -m "Сообщение"__* после *git add* или *__git commit -am "Сообщение"__*, которая не требует *git add* и добавляет в коммит изменившиеся неновые файлы. 

### Git log
Чтобы посмотреть историю коммитов, нажмите *__git log__*. Для краткости *__git log --oneline__*, для отображения веток *__git log --graph__*.
___
## Перечень основных команд для Git

* *__git --version__* - команда для проверки версии Git
* *__git init__* - инициализация пустого локального репозитория
* *__git status__* - проверка текущего состояния файлов в репозитории
* *__git add имя_файла_расширение__* - добавить версионность файлу
* *__git add .__* - добавить версионность всем файлам в текущей папке
* __*git commit -m "Название коммита и дополнительные комментарии"*__ - команда для фиксацмии изменений файлов с указанием комментариев
* __*git commit -am "название коммита"*__ - команда для фиксации изменившихся неновых файлов (одновременно с добавлением версионности)
* __*git log*__ - вывод истории коммитов в хронологическом порядке
* __*git diff*__ - вывод изменений на текущий момент по отношению к последнему коммиту
* __*git checkout хэш_коммита*__ - перейти к указанному коммиту
* __*git checkout master*__ - перейти к актуальному состоянию ветки master
___
## Создание веток
![Изображение ветвления](Branches_3.png)

Для того, чтобы создать ветку, нужно использовать команду *__git branch название_ветки__* (перейти с помощью *__git checkout название_ветки__*) или сразу с переходом *__git checkout -b название_ветки__*. Чтобы удалить ветку, нажмите *__git branch -d название_ветки__*. Чтобы посмотреть список веток, нажмите *__git branch__*. Чтобы слить ветку в текущую, нажмите *__git merge название_ветки__*.

* __*git branch*__ - выводит список ветокв в репозитории и показывает, где мы находимся сейчас
* __*git branch имя_ветки*__ - создаёт новую ветку с выбранным названием
* __*git checkout имя_ветки*__ - перейти к актуальному состоянию ветки с указанным названием
* __*git merge имя_ветки*__ - происходит слияние с текущей веткой ветки с указанным названием
* __*git branch -d имя_ветки*__ - удаление ветки с выбранным названием
* __*git log --graph*__ - выводит журнал изменений с более наглядным отображением веток и коммитов в виде графа
___

## Команды для работы с удаленным репозиторием в Git
![Изображение логотипов git and GitHub](Git_github_2.jpg)

- __*git fetch*__ - связывается с удалённым репозиторием и забирает из него все изменения, которых у вас пока нет и сохраняет их локально
- __*git pull*__ - работает как комбинация команд git fetch и git merge, т.е. Git вначале забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой
- __*git push*__ - используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в удаленный репозиторий, поэтому она использует аутентификацию.
- __*git remote*__ - служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например "origin". Вы можете использовать несколько удалённых репозиториев для работы и git remote поможет добавлять, изменять и удалять их.
- __*git archive*__ - используется для упаковки в архив указанных коммитов или всего репозитория.
- __*git submodule*__ - используется для управления вложенными репозиториями. Например, это могут быть библиотеки или другие, используемые не только в этом проекте, ресурсы.
___

## Как устроен GitHub
![Изображение логотипа GitHub](GitHub_1.png)
>__*GitHub*__ — это хостинг: он позволяет хранить проекты удалённо на сервере и работать с ними из любой точки мира. Доступ к файлам есть у всех, у кого есть ссылка.

**Одна из главных функций GitHub** — контроль версий. Все изменения в коде можно отследить, поэтому в командной разработке это незаменимая вещь.

Кроме того, для начинающих разработчиков **GitHub** — это не только хостинг, но и способ собрать портфолио. Он позволяет продемонстрировать свои навыки и знания в виде реализованных проектов — во вкладке Repositories.
___
Более подробную информацию о командах Git можно найти на официальном сайте по [ссылке](https://git-scm.com/book/ru/v2/%D0%9F%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5-C%3A-%D0%9A%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B-Git-%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D1%8B%D0%B5-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B).

___
