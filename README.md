## Инструкции по работе с Git

*git init* - инициализируем пустой репозиторий

*git status* - проверяем текущее состояние файлов

*git add* - добавляем версионность файлу

*git commit -m "Message"* - команда для фиксации изменений файл

*git log* - вывод истории комитов в хронологическом порядке

*git diff* - вывод изменений на текущий момент по отношению к последнему комиту

*git checkout master либо хэш-номер комита* - переход между изменениями либо возврат к текущему состоянию

*git clone ссылка* - команда для загрузки удалённого репозитория

*git push* - команда для отправки из локального репозитория в удалённый

*git pull* - команда для подгрузки изменений из удалённого репозитория в локальный

*git branch* - посмотреть список веток

*git branch название_ветки* - создать новую ветку

*git checkout -b название_ветки* - перейти к другой ветке и, если её нет, то создать

*git branch -d название_ветки* - удалить

## Что такое Git?

Git - это одна из реализаций распределенных систем контроля версий, имеющая как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля в мире. 

## Подготовка репозитория

Для создания репозтория необходимо выполнить команду *git init* в папке с репозиторием


## Создание коммитов 

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit -m "Сообщение"* или *git commit -am "Сообщение"*

## Создание ветки

Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки* (последняя команда ещё и переместит в новую ветку)
## Git log
Чтобы посмотреть историю комитов, нажмите *git log*. Если нужно кратко, то *git log --oneline*. Для отображения веток команда *git log --graph*. 

## Слияние веток
Чтобы слить ветку в текущую, нажмите *git merge имя_ветки*


Git — это набор консольных утилит, которые отслеживают и фиксируют изменения в файлах (чаще всего речь идет об исходном коде программ, но вы можете использовать его для любых файлов на ваш вкус). Изначально Git был создан Линусом Торвальдсом при разработке ядра Linux. Однако инструмент так понравился разработчикам, что в последствии, он получил широкое распространение и его стали использовать в других проектах. С его помощью вы можете сравнивать, анализировать, редактировать, сливать изменения и возвращаться назад к последнему сохранению. Этот процесс называется контролем версий.

## Установка

* Linux — нужно просто открыть терминал и установить приложение при помощи пакетного менеджера вашего дистрибутива. Для Ubuntu команда будет выглядеть следующим образом:
sudo apt-get install git
* Windows — мы рекомендуем git for windows, так как он содержит и клиент с графическим интерфейсом, и эмулятор bash.
* OS X — проще всего воспользоваться homebrew. После его установки запустите в терминале:
brew install git

## Работа в репозитории

Как правило, есть два варианта начать работу с репозиторием Git:

* Можно выбрать локальный каталог и создать новый репозиторий в нем.
 * Можно клонировать существующий репозиторий с локального компьютера или сервера. Обычно проекты клонируются именно с сервера.

## Клонирование существующего репозитория

Когда вы работаете в команде, разрабатываемые проекты часто размещают на сервере. Это один из самых распространенных сценариев. Вам нужно получить копию проекта последней версии на свой компьютер, чтобы далее вносить в него свой вклад.