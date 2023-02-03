# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains
## Что такое система контроля версий Github?

Git - это одна из реализаций распределенных ситстем контроля версий , которая работает как  с локальными, так и удаленными репозиториями. Является самой популярной реализацией систем контроля в мире. 

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием. с Этого начинается работа в теминале.

## Git add - add, add

Для добавления изменений в  commit используется команда *git add*. Чтобы использовать команду  *git add*,  напишите *git add имя_файла* или *git add*

## Создание коммитов

Для того, чтобы создать commit (сохранение), необходимо выполнить команду *git commit -m "Сообщение"* или *git commit -am "Сообщение"*. Обычно следует сразу за командой *git add*.

## Создание веток

Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки* (последняя команда переместит в новую ветку)

## Git log

Чтобы посмотреть история коммитов , нажмите *git log*. Если нужно кратко, то *git log  --oneline*. Для отображения веток команда *git log --graph*. Чтобы отобразить журнал сжато, используется команда *git log --oneline*.

## Слияние веток

Чтобы слить ветки в текущую, нажмите *git merge имя_файла*.

## Conflict branch

Создание ветки для отображения.

*git clone ссылка* - команда для загрузки удаленного репозитория

*git push*  - команда для отправки из локального репозитория в удаленный

*git pull* - команда для подгрузки изменений из удаленного репозитория в локальный

*git branch* - посмотреть список веток

*git branch название_ветки* - создать новую ветку

*git checkout -b название_ветки* - перейти к другой ветке и , если ее нет, то создать

*git branch -d название_ветки* - удалить ветку