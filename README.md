# Введение

## Начальная работа с системой контроля версий

**git --vrsion** - комманда для проверки версии git

**git init** - инициализация пустого репозитория

**git status** - проверка текущего состояния файлов

**git add file_name** - добавление версионности необходимому файлу

**git add .** - добавить версионность всем файлам в папке (пробел перед точкой обязателен)

**git commit -m "comment"** - зафиксировать изменения с комментарием к версии

**git commit -am "comment"** - зафиксировать изменения с комментарием к версии, без использования **git add** (использование git add обязательно при начале работы, в дальнейшем можно **-am**)

**git log** - вывод истории коммитов в хронологическом порядке

**git diff** - вывод изменений на текущий момент по отношению к последниму коммиту

**git checkout** - возвращение к неоходимому коммиту

**git checkout master** - возвращение к актуальному состоянию ветки master


## Добавление элементов

**Для добавления изображения** используется синтаксис ! [комментарий к изображению] (имя изображения.с указанием расширения). Изображение помещается в папку репозитория.
Например:

![Извиняшка](%D0%98%D0%B7%D0%B2%D0%B8%D0%BD%D1%8F%D1%88%D0%BA%D0%B0.png)

**Для игнорирования файлов** при коммите необходимо создать файл ".gitignore" в папке репозитория. В файле указывается список файлов необходимых для игнорирования с указанием расширения. Сохранить и закоммитить его

**Для добавления ссылок** используется синтаксис [текст для отображения] (ссылка).
Например:
[GeekBrans](https://gb.ru/)

**Для обозначения цитат** используется знак "больше". Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Например:
>Танки грязи не боятся

# Что такое Github?

Git - одна из реализаций систем контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной реализаций систем контроля врсий в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду git init в папке с репозиторием

### Git add
Для добавления изменений в коммит используется команда *git add имя_файла* 

### Создание коммитов

Для создания коммитов необходимо выполнить комманду *git commit -am "сообщение"*


### Создание ветки
Для создания ветки испульзуется комманда *git branch имя_ветки* или *git checkout -b имя_ветки* для моментального переключения на создаваемую ветку


## Работа с удаленными репозиториями

### Копирование удаленного репозитория

Для копирования на локальный компьютер удаленного репозитория используется команда *git clone*. Данная команда не только загружает все изменения, но и пытается слить все ветки на локальном компьютере и в удаленном репозитории.

### Скачивание удаленного репозитория

Для скачивания удаленного репозитория на локальный компьютер используется команда *git pull*. Эта комманда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией.

### Отправка своей версии репозитория во внешний

Отправить свою версию репозитория во
внешний репозиторий поможет команда *git
push*. При первом её использовании нужна авторизация.

Эта команда позволяет отправить нашу
версию репозитория на внешний
репозиторий. ТРЕБУЕТ АВТОРИЗАЦИИ 
на внешнем репозитории.

### Запрос на вливание изменений в удаленный репозиторий

 Предлагать изменения на GitHub нужно в отдельной ветке. Сначала пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем
клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет
изменения командой *git push* в свой аккаунт на GitHub и на сайте даёт команду *pull request*.