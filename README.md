# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

## Что такое Git?

Git - это одна из реализиций распределённых систем коттроля версий, как и локальные так и удалённые репозитории. Является самомой популярной реализацией контроля версий в мире.


[https://en.wikipedia.org/wiki/Git](Wikipedia)



## Подготовка репрозитория

Команда git init создает новый репозиторий Git. 

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием.

> Команда git init создает новый репозиторий Git. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий. Большинство остальных команд Git невозможно использовать без инициализации репозитория, поэтому данная команда обычно выполняется первой в рамках нового проекта.

## Git add

Для добавления изменения в комит используется команда *git commit* что бы использовать команду *git add*, нажмите *git add <имя файла>*.

> Данная команда добавит в индекс все файлы, в которых были изменения, а также новые файлы.

После того, как изменения были проиндексированы, их нужно закоммитить

## Создание комитов 

Для того что бы создать комит (сохранение), необходимо  выполнить команду *git commit -m "сообщение".

## Создание ветки 

![ветка](https://fuzeservers.ru/wp-content/uploads/a/3/e/a3e535d1274f699c072bc764e75ef711.png)


Для того что бы создать ветку, нужно использовать *git branch <имя ветки>* или *git checkout -b <имя ветки>*.

> Ветка представляет собой отдельное направление разработки. Ветки выступают в качестве абстрактного представления для процесса редактирования/индексации/коммита.