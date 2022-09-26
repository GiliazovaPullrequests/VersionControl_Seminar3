# Инструкция по работе с Git

## Что такое Github?

Github - это одна из реализаций распределённых систем контроля версий, и имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире. 


## Подготовка репозитория

Для создания реозитория необходимо выполнить команду *git init* в папке с репозиторием.

## Git add

Для добавления изменений в коммит (сохранение) используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add имя_файла*.

## Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit -m "Сообщение".

## Создание ветки

Для того, чтобы создать ветку, нужно использовать *git branch имя_ветки* или *git checkout -b имя_ветки*

## Что такое удаленный репозиторий

Репозиторий, хранящийся в облаке, на стороннем сервисе, специально созданном для работы с git имеет ряд преимуществ. Во-первых - это своего рода резервная копия вашего проекта, предоставляющая возможность безболезненной работы в команде. А еще в таком репозитории можно пользоваться дополнительными возможностями хостинга. К примеру -визуализацией истории или возможностью разрабатывать вашу программу непосредственно в веб-интерфейсе.

## Подключение к удаленному репозиторию

Чтобы загрузить что-нибудь в удаленный репозиторий, сначала нужно к нему подключиться. Регистрация и установка может занять время, но все подобные сервисы предоставляют хорошую документацию.
Чтобы связать наш локальный репозиторий с репозиторием на GitHub, выполним следующую команду в терминале. Обратите внимание, что нужно обязательно изменить URI репозитория на свой.

## Отправка изменений на сервер

Сейчас самое время переслать наш локальный коммит на сервер. Этот процесс происходит каждый раз, когда мы хотим обновить данные в удаленном репозитории.
Команда, предназначенная для этого - push. Она принимает два параметра: имя удаленного репозитория (мы назвали наш origin) и ветку, в которую необходимо внести изменения (master — это ветка по умолчанию для всех репозиториев).

## Как удалить локальный репозиторий

Вам не понравился один из ваших локальных Git-репозиториев и вы хотите стереть его со своей машины. Для этого вам всего лишь надо удалить скрытую папку *.git* в корневом каталоге репозитория. Сделать это можно 3 способами:

1. Проще всего вручную удалить эту папку *.git* в корневом каталоге **Git Local Warehouse**.

2. Также удалить, не устраивающий вас, репозиторий можно на github. Открываете нужный вам объект и переходите в пункт меню Настройки. Там, прокрутив ползунок вниз, вы попадете в зону опасности, где один из пунктов будет называться «удаление этого хранилища».

3.  Последний метод удаления локального хранилища через командную строку, для этого в терминале необходимо ввести следующую команду: 

                        cd repository-path/

                        rm -r .git*
       
## Пошаговая инструкция по работе с удаленными репозиториями

1. Создали аккаунт на GitHub.com
2. Создать локальный репозиторий 
3. "Подружить" ваш локальный и удаленный репозиторий. GitHub при создании нового репозитория подскажет, как это можно сделать)
4. отправить (push) ваш локальный репозиторий в удаленный , при этом, вам, возможно нужно будет авторизоваться на удаленном репозитории.
5. Провести изменения "с другого компьютера"
6. Выкачать (pull) актуальное состояние из удаленного репозитория 

# Настройка совместной работы

1. Делаем форк (fork) интересующего нас репозитория.
2. Мы делаем git clone для нашей версии этого репозитория.
3. Мы создаем ветку с предлагаемыми изменениями.
4. Производим все изменения только в этой ветке.
5. Отправляем эти изменения на свой аккаунт (push).
6. В окне на GitHub появляется возможность отправить pull request.
