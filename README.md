# Git. Github. Работа с удаленными репозиториями

<image src="data:image/png;base64,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" alt="git+github">

## **Что такое Git**

**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## **Что такое Github**

**GitHub** — крупнейший веб-сервис для хостинга IT-проектов и их совместной разработки. Создатели сайта называют **GitHub** «социальной сетью для разработчиков». Кроме размещения кода, участники могут общаться, комментировать правки друг друга, а также следить за новостями знакомых. С помощью широких возможностей **Git** программисты могут объединять свои репозитории — **GitHub** предлагает удобный интерфейс для этого и может отображать вклад каждого участника в виде дерева.

## **Что такое удаленный репозиторий**

**Удалённые репозитории** представляют собой версии вашего проекта, сохранённые в интернете или ещё где-то в сети. У вас может быть несколько удалённых репозиториев, каждый из которых может быть доступен только для чтения или для чтения/записи. Взаимодействие с другими пользователями предполагает управление удалёнными репозиториями, а также отправку и получение из них данных. Управление репозиториями включает в себя как умение добавлять новые, так и умение удалять устаревшие репозитории, а также умение управлять различными удалёнными ветками, объявлять их отслеживаемыми или нет и так далее.

---
## **Список основных команд:**

* *Подготовка репозитория*

  Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием.

* *Просмотр удалённых репозиториев*

  Для того, чтобы просмотреть список настроенных удалённых репозиториев, вы можете запустить команду *git remote*. Она выведет названия доступных удалённых репозиториев.

* *Добавление изменений в коммит*

  Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add "имя_файла"*

* *Создание коммитов*

  Для того чтобы создать коммит (сохранение),необходимо выполнить команду *git commit -m "Сообщение"*

* *Создание ветки*

  Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки*

* *Переключение между ветками*

  Для того, чтобы переключиться с одной ветки на другую, нужо выполнить команду *git checkout имя_ветки*

* *Клонирование репозитория*

  Для клонирования переданного репозитория на ваш компьютер нужно использовать команду *git clone*

* *Передача изменеий в удаленный репозиторий*

  Команда *git push* используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.

* *Получение изменений из удаленного репозитория*

  Команда *git pull* получает изменения из переданного удаленного репозитория и обновляет рабочую копию в соответствии с удаленным репозиторием.

* *Переименование удалённых репозиториев*

  Для переименования удалённого репозитория можно выполнить *git remote rename старое_имя_репозитория новое_имя_репозитория*

* *Удаление удаленных репозиториев*

  Если по какой-то причине вы хотите удалить удаленный репозиторий, можете использовать *git remote remove имя_репозитория* или *git remote rm имя_репозитория*

