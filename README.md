# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains
## Что такое Git?

Git - это одна из реализаций распределенных систем контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой   популярной реализацией систем контроля версий в мире. 

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием. 

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add имя_файла_с_расширением* или *git add .* для всех файлов в текущей папке. 

## Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit -m "Сообщение"* после git add или *git commit -am "Сообщение"*, которая не требует git add и добавляет в коммит изменившиеся неновые файлы. 

## Git log

Чтобы посмотреть историю коммитов, нажмите *git log*. Для краткости *git log --oneline*, для отображения веток *git log --graph*.

## Создание ветки

Для того, чтобы создать ветку, нужно использовать команду *git branch название_ветки* (перейти с помощью git checkout название_ветки) или сразу с переходом *git checkout -b название_ветки*. Чтобы удалить ветку, нажмите *git branch -d название_ветки*. Чтобы посмотреть список веток, нажмите *git branch*. Чтобы слить ветку в текущую, нажмите *git merge название_ветки*.

## Команда git clone составная:
Oна не только
загружает все изменения, но и пытается слить 
все ветки на локальном компьютере и в
удаленном репозитории.

## git push 
Отправить свою версию репозитория во
внешний репозиторий поможет команда git
push. При первом её использовании нужна
авторизация.
Эта команда позволяет отправить нашу
версию репозитория на внешний
репозиторий. ТРЕБУЕТ АВТОРИЗАЦИИ 
на внешнем репозитории.

## git pull
Эта команда позволяет скачать все 
из текущего репозитория и автоматически
сделать merge с нашей версией.

## Как настроить совместную работу

1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. 
 GitHub при создании нового репозитория подскажет, как это можно сделать
4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно, 
вам нужно будет авторизоваться на удалённом репозитории
5. Провести изменения “с другого компьютера”
6. Выкачать (pull) актуальное состояние из удалённого репозитория

## pull request

* команда для предложения изменений
* запрос на вливание изменений в репозиторий. 

В больших компаниях один ответственный за проект создает аккаунт. Другие пользователи дают
команду  pull request. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала
пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем
клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет
изменения командой push в свой аккаунт на GitHub и даёт команду pull request. 

## Как сделать pull request
1. Делаем   (ответвление) репозитория fork
2. Делаем git clone   версии репозитория СВОЕЙ
3. Создаем новую ветку и в НЕЕ вносим свои изменения
4. Фиксируем изменения (делаем коммиты)
5. Отправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку pull request