## Что такое Git?

Git - это одна из реализаций распределенных систем контроля версий, имеющих как локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория

Для создания репозитория необходимо создать команду "git init" в папке с репозиторием.

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add "имя файла"*

## Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit -m "Сообщение"*

## Создание веток

Для того, чтобы создать ветку, нужно использовать *git branch "имя ветки"*

## Переход между ветками

Для того, чтобы перейти между ветками, нужно использовать *git checkout "имя ветки"*

## Создание ветки и переход в нее

Для того, чтобы создать ветку и перейти в нее, нужно использовать *git checkout -b "имя ветки"*

## Удаление ветки

Для того, чтобы удалить ветку, нужно использовать *git branch -d "имя ветки"*

## Вывод истории коммитов

Для того, чтобы вывести на экран историю всех коммитов, нужно использовать *git log*

## Cливание веток

Для того, чтобы слить ветку, нужно использовать *git merge "имя ветки"*

## Вывод коммитов в графическом виде

Для того, чтобы вывести дерево коммитов в графическом виде, нужно использовать *git log --graph*

## Отмена команды *merge*

Для того, чтобы отменить команду *merge* и вернуться к исходному состоянию, нужно использовать *git merge --abort*