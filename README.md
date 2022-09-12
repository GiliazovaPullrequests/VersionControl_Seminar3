# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

## Что такое Git?

Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире. 

## Подготовка репозитория

Для создания папки (например, на рабочем столе) через терминал, необходимо ввести команду:
mkdir Desktop/folder_name/
Для перехода в данную папку и последующего создания в ней репозитория вводим команду:
cd Desktop/folder_name/
либо выбираем данную папку нажатием табулятора после ввода команды cd
Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием.

## Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add "имя файла"*

## Создание коммитов 

Для того чтобы создать коммит (сохранение),необходимо выполнить команду *git commit -m "Сообщение"*

## Создание ветки

Для того,чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки*

## Git clone
Для того, чтобы создать копию удаленного репозитория локально на своем компьютере, необходимо использовать команду *git clone адрес репозитория*

## Git Push
Для того, чтобы зафиксировать сделанные в локальной копии файла изменения (чтобы они отображались в удаленном репозитории), используем команду: *git push*

## Git Pull
Если мы работаем в удаленном репозитории и создаем там коммиты, то для их отображения в локальной версии необходимо ввести в терминале: *git pull*

## Ветвление 
Для создания веток редактирования используем команды:
*git branch имя_ветки* или *git checkout -b имя_ветки*

Переключение между ветками происходит при использовании команды ***git checkout имя_ветки***

Для объединения веток используется команда ***git merge имя_ветки*** однако следует помнить, что данная команда переносит изменения указанной ветки в активню на текущий момент ветку (возможно понадобится выполнить переход на ветку *мастер* а затем выполнить слияние)

После слияния веток имеет смысл удалять лишние. Делается это командой ***git branch -d имя_ветки***

## Переходы между версиями
Для возврата к какому-либо из прошлых закоммиченных состояний выполняем команду: **git checkout + _номер коммита_ + _путь к файлу_**

## Настройка .gitignore
Если у нас в проекте есть файлы или директории, которые мы не хотим коммитить, мы можем удостовериться, что они случайно не попадут в git add -A при помощи файла .gitignore 
Реализуем все это следующим образом:

1. Создем вручную файл под названием .gitignore и сохраняем его в директорию проекта.
2. Внутри файла перечисляем названия файлов/папок, которые нужно игнорировать, каждый с новой строки.
3. Файл .gitignore должен быть добавлен, закоммичен и отправлен на сервер, как любой другой файл в проекте.

