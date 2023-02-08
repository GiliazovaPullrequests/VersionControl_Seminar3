# Инструкция по работе с Git

## Начальная работа с системой контроля версий

*git --version* - команда для проверки версии git

*git init* - инициализируем пустой репозиторий

*git status* - проверяем текущее состояние файлов

*git add* - добавляем версионность файлу

*git commit -m "Message"* - команда для фиксации изменений файл

*git log* - вывод истории коммитов в хронологическом порядке

*git diff* - вывод изменений на текущий момент по отношению к последнему комиту

*git checkout master либо хэш-номер комита* - переход между изменениями либо возврат к текущему состоянию

## Что такое Git?

Git - это  одна из реализаций распределенных систем контроля версий, имеющая как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишем *git add имя_файла* или *git add .*

## Создание коммитов

Для того, чтобы создать коммит (сохранение), неодходимо выполнить команду *git commit -m "Сообщение"* или *git commit -am "Сообщение"*

# Создание ветки

Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки* (последняя команда ещё и переместит в новую ветку)

## Git log

Чтобы посмотреть историю коммитов, нажмите *git log*. Если нужно кратко, то *git log --oneline*. Для отображения веток команда *git log --graph*.

## Слияние веток

Чтобы слить ветку в текущию, нажмите *git merge имя_ветки*

*git clone ссылка* - команда для загрузки удаленного репозитория

*git push* - команда для отправки из локального репозитория в удаленный

*git pull* - команда для подгрузки изменений из удаленного репозитория в локальный

*git branch* - посмотреть список веток

*git branch название_ветки* - создать новую ветку

*git checkout -b название_ветки* - перейти к другой ветке и, если её нет, то создать

*git branch -d название_ветки* - удалить ветку

# Изучили Github

* Найчились в целом работать с __Github__, и его терминами.

https://www.google.com/url?sa=i&url=https%3A%2F%2Flinedot.ru%2Fkartinki%2Fspasibo-kartinki%2F&psig=AOvVaw2-b6xjgaet7cDg9jf7qVXX&ust=1675964833591000&source=images&cd=vfe&ved=0CA8QjRxqFwoTCIjvlda9hv0CFQAAAAAdAAAAABAE

![SpAsIbO](https://linedot.ru/wp-content/uploads/2019/12/spasibo1.jpg)

***Спасибо вам большое за ваше внимае к нам!*** ___Будем по вам скучать___