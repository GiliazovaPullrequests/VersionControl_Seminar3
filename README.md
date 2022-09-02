# Начальная работа с системой контроля Git

|Команда | Описание |
|----- |------
|*git version* - |команда для проверки версий git
|*git init* - |команда для проверки пустого репозитоория
|*git status* - |проверка текущего состояния файла
|*git add имя_файла.расширение* - |добавление версионности файла
|*git commit -m "Message" - |команда для фиксации изменения файлов 
|*git log* - |вывод истории коммитов в хронологическом порядке
|*git diff* - |вывод изменений на текущий момент по отношению к последнему коммиту
|*git checkout master/main, название ветки* - |переход между изменениями или возврат к текущему состоянию 

>цитата
>>второй уровень цитирования
>>>можно углублять уровни цитирования до 15-ти

[Ссылка на картинку](https://imagename2.ru/imgbig/imagename_ru_20226.jpg)

![картинка](https://imagename2.ru/imgbig/imagename_ru_20226.jpg)



## 1. Что же такое Git?

Git - это распределенная система управления версиями. Это означает, что  локальный клон проекта, является полным репозиторием управления версиями. Полнофункциональные локальные репозитории упрощают работу в автономном режиме или в удаленном расположении. разработчики фиксируют свою работу локально, а затем синхронизируют свои копии репозитория с копией на сервере. 
Проект Git был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано.



## Список очень нужных команд в git?

1. *git branch* - это команда Git для управления ветками. Используйте эту метку для обозначения всех вопросов, связанных с ветками, их созданием, структурой, управлением и удалением. Общие сведения. git branch – это команда для управления ветками в репозитории Git.


2. *git branch <branch_name>* -  эта коианда необходима, для того,чтобы создать новую ветку

3. *git checkout <branch_name>* - переключиться на указанную ветку и обновить рабочую директорию.

4. *git merge <branch_name>* - эта команда нужна если вы хотите  слить ветки

5. *git branch -d <branch_name>* - Чтобы удалить локальную ветку в Git нужно выполнить команду (вместо mybranch необходимо поставить название ветки, которую вы хотите удалить)

6. git clone <url-адрес репозитория> – клонирование внешнего репозитория на  локальный ПК

7.	git pull – получение изменений и слияние с локальной версией

8.	git push – отправляет локальную версию репозитория на внешний

