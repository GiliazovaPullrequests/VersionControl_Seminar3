## Что такое GIT?

Git-это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

##Подготовка репозитория.

Для создание репозитория необходимо выполнить команду git init в папке с репозиторием

## Git add

Для добавления измений в коммит используется команда git add. Чтобы использовать команду git add напишите git add <имя файла> или *git add .*

## Создание коммитов

Для того, чтобы создать коммит(сохранение) необходимо выполнить команду git commit. Выполняется она так: git commit -m "<сообщение к коммиту>. 

## Создание веток

Для того, чтобы создать ветку, используется команда git branch. Делается это следующим образом в папке с репозиторием: git branch <название новой ветки>

## Git log

Чтобы посмотреть историю коммитов, нажмите *git log*. Если нужно кратко, то *git log -- oneline. Для продолжения веток команда *git log --graph*.

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge имя_ветки*

## Удаление веток

Для удаления ветки ввести команду "git branch -d 'name branch'"

## Журнал изменений

Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда git log. Для этого достаточно выполнить команду git log в папке с репозиторием.

## Перемещение между сохранениями

Для того, чтобы перемещаться между коммитами, используется команда git checkout. Используется она в папке с пепозиторием следующим образом: git checkout <номер коммита>

## Подготовка репозитория

Для создание репозитория необходимо выполнить команду git init в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Git clone

Команда для загрузки удаленного репозитория

## Git push

Команда для отправки из локального репозитория в удаленный

## Git pull

Команда для подгрузки изменений из удаленного репозитория в локальный

## Git branch

Посмотреть список веток

## Git branch название_ветки*

Создать новую ветку

## Git checkout -b название_ветки*

Перейти к другой ветке и, если ее нет, создать

## Git branch -d  название_ветки*

Удалить ветку


