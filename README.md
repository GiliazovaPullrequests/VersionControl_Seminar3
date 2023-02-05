# VersionControl_Seminar3

## Начальная работа с системой контроля версий

- git --version - команда для проверки версии `<git>`.

- [git init](https://www.atlassian.com/ru/git/tutorials/setting-up-a-repository/git-init) - инициализируем пустой репозиторий

- [git status](https://www.atlassian.com/git/tutorials/inspecting-a-repository#:~:text=The%20git%20status%20command%20displays,regarding%20the%20committed%20project%20history.) - проверить текущее состояние файлов

- [git add имя*файла*с_расширением](https://www.atlassian.com/git/tutorials/saving-changes) - добавляем версионность файлу

- [git add .](https://www.atlassian.com/git/tutorials/saving-changes) - добавляем версионность всем файлам в папке

- [git commit -m "Сообщение"](https://www.atlassian.com/git/tutorials/saving-changes/git-commit) - команда для фиксации изменений файлов

- [git commit -am "Сообщение"](https://www.atlassian.com/git/tutorials/saving-changes/git-commit) - фиксация изменений , не требует `<git add .>`

- [git diff](https://www.atlassian.com/git/tutorials/saving-changes/git-diff) - вывод изменений на текущий момент по отношению к последнему коммиту

- [git log](https://www.atlassian.com/git/tutorials/git-log) - вывод истории коммитов в хронологическом порядке

- [git checkout хэш_коммита](https://www.atlassian.com/git/tutorials/using-branches/git-checkout) - переход между изменениями

- [git checkout master](https://www.atlassian.com/git/tutorials/using-branches/git-checkout) - возврат к текущему состоянию

- _git clone ссылка_ - команда для загрузки удалённого репозитория

- _git push_ - команда для отправки из локального репозитория в удалённый

- _git pull_ - команда для подгрузки изменений из удалённого репозитория в локальный

- _git branch_ - посмотреть список веток

- *git branch название*ветки\_ - создать новую ветку

- *git checkout -b название*ветки\_ - перейти к другой ветки и если её нет, то создать

- *git branch -d название*ветки\_ - удалить ветку

## Что такое git?

Git - это одна из реализаций распределенных систем контроля версий, имеющая как и лакальный, так и удаленные репозитории. Является самой популярной реалезацией систем контроля в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду _git init_ в папку с репозиторием.

## Git add

Для добавления изменений в коммит используется команда _git add_. Чтобы использовать команду _git add_, напишите *git add имя*файла* или \_git add .*.

## Создание коммитов

Для того, чтобы создать коммит(сохранением), необходимо выполнить команду _git commit -m "сообщение"_ или _git commit -am "Сообщение"_.

## Создание ветки

Для того, чтобы создать ветку, нужно использовать *git branch имя*ветки* или \_git checkout -b имя*файла\_ (последняя команда ещё и перемистит в новую ветку).

## Перейти к другой ветки

Для того, чтобы перейти к другой ветке, нужно использовать _git checkout имя_ветки_

## Git log

Чтобы посмотреть историю коммитов, нажмите _git log_. Если нужно кратко, то _git log --one line_. Для отображения веток команды _git log -- graph_.

## Слияние веток с помощью _git merge_

Чтобы слить ветку в текущую, нажмите *git merge имя*ветки\_.
