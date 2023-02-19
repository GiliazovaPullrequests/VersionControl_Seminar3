## _Инструкция для **Git**_

* **git** --version - команда для проверки версии git

* **git init** - инициализация локального репозитория

* **git status** - получить информацию от git о его текущем состоянии

* **git add** - добавить файл или файлы к следующему коммиту

* **git commit** -m "massage" - создание коммита

* **git log** - вывод на экран истории всех коммитов с их хеш-кодами

* **git checkout** - переход от одного коммита к другому

* **git checkout** master - вернуться к актуальному состоянию и продолжить работу

* **git diff** - увидеть разницу между текущим файлом и закоммиченным файлом

* **git branch** -посмотреть список веток репозитории

* **git branch** <название ветки> - создать новую ветку

* **git checkout** <название ветки> - переход на другую ветку 

* **git branch** -d <название ветки> - удаление ветки

* **git push** - Отправление репозитория на удаленый репозиторий

* **git pull** - Выкачивание актуальной версии репозитория с удаленного и сливание с локальной версией

* **git clone** ссылка - клонирование репозитория с интернета

## Как сдавать домашние задания через **Pull request**

1. Зарегистрироваться на сайте [Github](https://github.com/) и войти на Github используя свои учетные данные.

2. Найти на сайте Github Public repository для сдачи заданий через пулл-реквесты. [Ссылка для домашнего задания](https://github.com/GiliazovaPullrequests/VersionControl_Seminar3).

3. Нажать кнопку "**Fork**" для копирования в свой репозиторий на Github, а затем кнопку "**Create fork**".

4. В своем профиле найти [новый репозиторий](https://github.com/pvplpt/VersionControl_Seminar3).

5. Нажать кнопку "**<> Code**",  перейти на закладку "**Local**", перейти на закладку "**HTTPS**"

6. Скопировать ссылку на репозиторий: https://github.com/pvplpt/VersionControl_Seminar3.git

7. На своем компмпьютере запускаем Visual Studio Code и открываем папку без git, в которую планирется клонировать репозиторий с Github.

8. В VS Code открываем терминал(Ctrl+`)

9. Проверяем, что git в текущей папке не инициализирован командой **git status** 

10. Выполняем копирование удаленного репозитория по ссылке скопированной в п.6 командой **git clone** https://github.com/pvplpt/VersionControl_Seminar3.git

11. Закрываем текущую папку в VS Code(Ctrl+K F)

12. Открываем новую папку **VersionControl_Seminar3** в VS Code и откываем терминал (Ctrl+`), если он не открыт.

13. Проверяем статус репозитория командой **git status**

14. Проверяем список веток и текущую командой **git branch**

15. Принято любые изменения вносить в отдельную ветку. Для сдачи домашнего задания нужно создать новую ветку со своей фамилией. Выполним команду **git checkout** -b Pozdnyakov.

16. Вносим и сохраняем необходимые изменения нужных файлом и папок

17. Добавяем файл или файлы к следующему коммиту камандой **git add .**

18. Создаем новый коммит командой **git commit** -m "added new text"

19. Пушим новую ветку на удаленный репозиторий командой **git push** --set-upstream origin Pozdnyakov

20. Откываем [удаленный репозиторий](https://github.com/pvplpt/VersionControl_Seminar3) 

21. Нажимаем кнопку "**Compare & pull request**"

22. Нажимаем кнопку "**Create pull request**"

23. В новой папке **seminar3** в текстовом файле **seminar3_pull_request_Pozdnyakov.txt** сохраняем ссылку на Pull request: https://github.com/GiliazovaPullrequests/VersionControl_Seminar3/pull/383

24. Сохраняем снимок экрана страницы браузера с pull request запросом в папку **seminar3** в файл **seminar3_pull_request_Pozdnyakov.png**

25. Архивируем и сжимаем папку **seminar3** командой **tar** -czvf seminar3.tgz seminar3/

26. Отправляем архив **seminar3.tgz** на проверку.

