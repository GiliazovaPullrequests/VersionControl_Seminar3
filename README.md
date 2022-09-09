## Что такое Git?

Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием.

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add "имя файла"*

## Создание коммитов

Для того чтобы создать коммит (сохранение),необходимо выполнить команду *git commit -m "Сообщение"*

## Создание ветки

Для того,чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки*

## Переход между ветками

Для перехода между ветками нужно использовать команду *git checkout имя_ветки*. Для просмотра количества и наименования веток в файле нужно использовать команду *git branch* 

## Работа с внешним репозиторием

Для работы с внешним репозиторием необходимо использовать команду *git clone <url-адрес репозитория>*

## git pull

Что бы получить изменения и провести слияние внешнего репозитария с локальной версией необходимо ввести команду *git pull*
## git  push

Для отправки локальной версии репозитория на внешний необходитмо использовать команду *git push*
