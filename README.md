# Инструкция GIT

## Что такое GIT 

>Git (произносится «гит»[7]) — распределённая система управления версиями. Проект был создан [Линусом Торвальдсом](https://ru.wikipedia.org/wiki/Торвальдс,_Линус "Статья на WiKi") для управления разработкой ядра *Linux*, первая версия выпущена 7 апреля 2005 года. 

>На сегодняшний день его поддерживает **Джунио Хамано**

![alt-текст](https://gb.ru/favicon.ico "Соберем мозг в кулак")

## Основные команды  GIT

*git --version* - команда для проверки версии git

*git init* - инициализация пустого репозитория

*git status* - проверка текущего состояния файлов

*gid add имя_файла* - добавить версионность файлу

*gid add .* - добавить версионность всей папке

*git commit -m "имя файла"* - комманда для фиксации измменений файлов 

*git commit -am "имя файла"* - комманда для фиксации изменившихся неновых файлов

*git log* - вывод истории коммитов в хронологическом порядке

*git diff* - вывод изменений на текущий момент по отношению к последнему коммиту


*git checkout хеш_коммита* - перейти к указанному коммиту

*git checkout master* - перейти к актуальному состоянию ветки master


git diff - увидеть разницу между текущим файлом и закоммиченным файлом

git branch -посмотреть список веток репозитории

git branch <название ветки> - создать новую ветку

git checkout <название ветки> - переход на другую ветку

git branch -d <название ветки> - удаление ветки

# Удаленные репозитории

git push - Отправление репозитория на удаленый репозиторий

git pull - Выкачивание актуальной версии репозитория с удаленного и сливание с локальной версией

git clone ссылка - клонирование репозитория с интернета

…or create a new repository on the command line

* echo "# Instr2" >> README.md
* git init
* git add README.md
* git commit -m "first commit"
* git branch -M main
* git remote add origin https://github.com/stevgeniy/Instr2.git
* git push -u origin main


…or push an existing repository from the command line

* git remote add origin https://github.com/stevgeniy/Instr2.git
* git branch -M main
* git push -u origin main