# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

# Добавляем текст инструкции:

## Что такое Git?

Git - это одна из реализаций распределенных систем контроля версий, имеющая как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля в мире. 

## Подготовка репозитория

Для создания репозтория необходимо выполнить команду *git init* в папке с репозиторием

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add имя_файла* или *git add .*

## Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit -m "Сообщение"* или *git commit -am "Сообщение"*

## Создание ветки

Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки* (последняя команда ещё и переместит в новую ветку)

## Git log
Чтобы посмотреть историю комитов, нажмите *git log*. Если нужно кратко, то *git log --oneline*. Для отображения веток команда *git log --graph*. 

## Слияние веток
Чтобы слить ветку в текущую, нажмите *git merge имя_ветки*

# Git clone ссылка
Команда для загрузки удаленного репозитория

# Git push
Команда отправки из локального репозитория в удаленный

# Git pull
Команда для загрузки изменений из удаленного репозитория в локальный

# Git branch
Просмотр списка веток

# Git branch название_ветки
Создание новой ветки

# Git checkout -b название_ветки
Перейти к другой ветке, если ее нет, то создать

# Git branch -d название_ветки
Удалить ветку