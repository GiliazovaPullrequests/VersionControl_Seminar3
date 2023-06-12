# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains
## Начальная работа с системой контроля версий

* git --version - команда для проверки версии git

* git init - инициализирует пустой репозиторий

* git stastus - проверяем текущее состояние файлов

* git add имя файла с расширением - добавляем версионность файлу

* git add . - добавляем версионность всем файлам

* git commit -m "сообщение" - команда для фиксации изменений файла

* git commit -am "сообщение" - фиксация сообщений, не требует add

* git diff - вывод изменений на текущий момент по отношению к последнему коммиту

* git log - вывод истории коммитов в хронологическом порядке

* git checkout хэш комита -переход между изменениями

* git checkout master - возврат к текущему состоянию

> Цитата: "Первая команда — git init. Она позволяет сделать из нашей папки репозиторий". 

[ссылка][https://gist.github.com/Jekins/2bf2d0638163f1294637#Blockquotes]

![картинка](/images/git-push-origin.png)

## Чтот такое Git?

Git - это одна из реализаций распределенных систем контроля версий, имеющая как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля в мире

## Git Add
Для добавления изменений в коммит используется команда "git add имя _файла" или "git add."

## Создание коммитов

Для того, чтобы создать коммит, необходимо выполнить команду "git commit -m "сообщение" или "git commit -am "сообщение"

## Создание веток

Для того, чтобы создать ветку нужно использовать "git branch имя_ветки" или "git checkout -b имя_ветки". Последняя команда позволяет создать ветку и перейти на неё. 

## Git log

Чтобы посмотреть историю коммитов, нажмите "git log". Если нужно кратко, то "git log --oneline". Для отображения веток команда "git log --graph"

## Слияние веток

Чтобы слить ветку в текущую, нажмите "git merge имя_ветки".

## Решение конфликта

После слияния веток может появится окно конфликта, где нужно выбрать какое состояние файла мы оставляем:текущее, измененное или будем исправлять вручную.

 # Работа с внешними репозиториями

* git clone url-адрес - клонирует внешний репозиторий на локальный ПК

* git pull - получение изменений и слияние с локальной версией

* git push - отправляет локальную версию реппозитория на внешний хаб 

Для работы с внешним репозиторием на локальном ПК необходимо

1. Сделать Fork реппозитория с чужого аккаунта.

2.Скопировать адресс (код) перенесенного репозитория со своего аккаунта.

3. В VScod создать папку и в терминале с помощью git clone _(CTRL+V)_ (вставляем скопированную ссылку) клонируем внешний репозиторий на личный ПК.

4. С помощью cd _имя папки_ войти в папку внешнего репозитория.

5. С помощью git log проверяем появился ли комит внешнего репозитория

6. Создаем свою ветку. Вносим изменения и сохраняем их (git add, git commit).

7. С помощью git push отправляем на свой внешний аккаунт изменения.

8. В своем аккаунте нажимаем кнопку _Compare & pull request_. 

9. Затем кнопку _create pull request_.


