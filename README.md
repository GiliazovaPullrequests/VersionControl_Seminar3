## Что такое Git?

Git — это система для управления версиями исходного кода программ. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров.Является самой популярной реализацией систем контроля версий в мире. 

С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду ***git init*** в папке с репозиторием.


## Создание коммитов

Для того, чтобы создать коммит (соохранение), необходимо выполнить команду ***git commit -m "Сообщение"***

***git commit -am "message"*** - команда для сохранения изменений в файле без использования команды ***git add***

## Git add 

Для добавления изменений в коммит используется команда ***git add***. Чтобы использовать команду ***git add***, напишите ***git add "имя файла"***

## Откат последнего коммита

Откатить последний коммит можно с помощью команды ***git revert***. Создастся новый коммит, содержащий обратные преобразования относительно предыдущего, и добавится к истории текущей ветки.

## Создание ветки

Для того, чтобы создать ветку, нужно использовать ***git branch имя_ветки*** или ***git checkout -b имя_ветки***

## Удаление ветки

Удалить ветку можно параметром ***branch*** с добавлением флага ***-d*** и указанием имени ветки. Если вы завершили работу над веткой и объединили её с основной, можно её удалить без потери истории. Однако, если выполнить команду удаления до слияния — в результате появится сообщение об ошибке. Этот защитный механизм предотвращает потерю доступа к файлам.

Для принудительного удаления ветки используется флаг ***-D*** с заглавной буквой. В этом случае ветка будет удалена независимо от текущего статуса, без предупреждений.

## Слияние двух веток

Объединить две ветки можно с помощью команды ***git merge branch_name***. Команда объединит указанную ветку с основной.

## Отображение журнала фиксации в виде графика для текущей или всех веток

Просмотреть историю коммитов в виде графика для текущей ветки можно с помощью команды  ***gti log и флагов --graph --oneline --decorate***. Опция ***--graph*** выведет график в формате ASCII, отражающий структуру ветвления истории коммитов. 
В связке с флагами ***--oneline*** и ***--decorate***, этот флаг упрощает понимание того, к какой ветке относится каждый коммит.

## Прекращение слияния при конфликте

Прервать слияние в случае конфликта можно командой  ***git merge --abort*** . Она позволяет остановить процесс слияния и вернуть состояние, с которого этот процесс был начат.

## Добавление удалённого репозитория

Добавить удалённый репозиторий можно командой ***git remote add***, указав shortname и url требуемого репозитория

## Просмотр удалённых URL-адресов

Просматривать удалённые URL-адреса можно командой ***git remote -v***. Этот параметр отображает удалённые подключения к другим репозиториям.

## Получение дополнительных сведений об удалённом репозитории

Получить подробные сведения об удалённом репозитории можно с помощью команды ***git remote show*** с указанием имени репозитория — например, ***origin***.

## Отправка изменений в удалённый репозиторий

Отправлять изменения в удалённый репозиторий можно с помощью команды ***git push*** с указанием имени репозитория и ветки.
Эта команда передаёт локальные изменения в центральный репозиторий, где с ними могут ознакомиться другие участники проекта.

## Получение изменений из удалённого репозитория

Для загрузки изменений из удалённого репозитория используется команда ***git pull***. При этом скачивается копия текущей ветки с указанного удалённого репозитория и объединяет её с локальной копией.

## Слияние удалённого репозитория с локальным

Слияние удалённого репозитория с локальным выполняется командой ***git merge*** с указанием имени удалённого репозитория.

## Отправка новой ветки в удалённый репозиторий

Передать новую ветку в удалённый репозиторий можно с помощью команды ***git push -u***, указав имя репозитория и имя ветки.

## Удаление удалённой ветки

Чтобы избавиться от удалённой ветки, используется команда ***git push --delete origin existing_branch***

## Клонирование репозитория
После того, как ваш (или чей-то) проект оказался на GitHub, любой желающий может скачать его копию с помощью команды ***git clone***.

## Использование перебазирования

Для доступа к этой функции используестя команда ***git rebase branch_name***. Перебазирование — это процесс объединения или перемещения последовательности коммитов на новый родительский снимок.
Эта команда изменит основу ветки с одного коммита на другой, как если бы вы начали ветку с другого коммита. В Git это достигается за счёт создания новых коммитов и применения их к указанному базовому коммиту. Необходимо понимать, что, хотя ветка и выглядит такой же, она состоит из совершенно новых коммитов.
