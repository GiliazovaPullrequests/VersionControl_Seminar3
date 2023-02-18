# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

## git init
Инициализирует новый репозиторий Git. Если вы хотите использовать в проекте контроль версий, эту команду следует изучить раньше остальных.
## git add
Переносит изменения из рабочего каталога в раздел проиндексированных файлов. В этом разделе можно подготовить снимок состояния, прежде чем сделать коммит изменений в официальную историю.

## git branch
Эта команда выступает универсальным инструментом администрирования веток. С ее помощью можно создавать изолированные среды разработки в одном репозитории.

Команда *git branch* позволяет создавать, просматривать, переименовывать и удалять ветки. Она не дает возможности переключаться между ветками или выполнять слияние разветвленной истории. Именно поэтому команда git branch тесно связана с командами git checkout и git merge.

*git branch*
Отображение списка веток в репозитории. Это синоним команды *git branch --list*

*git branch -d <branch>*
Удаление указанной ветки. Это «безопасная» операция, поскольку Git не позволит удалить ветку, если в ней есть неслитые изменения.
*git branch -a*
Вывод списка всех удаленных веток.
*git branch branch_name* -  создание новой ветки
*git checkout -b branch_name* - создание и одновременный переход на новую ветку.
## git checkout
С командой git checkout можно не только получать старые коммиты и прежние версии файлов, но и осуществлять навигацию по существующим веткам. В сочетании с базовыми командами Git она позволяет сосредоточиться на определенном направлении разработки.

## git clean
Удаляет неотслеживаемые файлы из рабочего каталога. Это логический аналог команды git reset, которая (обычно) работает только с отслеживаемыми файлами.

## git clone
Создает копию существующего репозитория Git. Клонирование — самый распространенный способ, с помощью которого разработчики могут получить рабочую копию центрального репозитория.

## git commit
Получает проиндексированный снимок состояния и выполняет его коммит в историю проекта. Эта команда в сочетании с командой git add определяет классический рабочий процесс для всех пользователей Git.

*git commit -am "message" - коммит одновременно с сохранением файла.
*git commit --amend*
Команда git commit с флагом --amend позволяет внести изменения в последний коммит. Она может оказаться полезной, если вы забыли проиндексировать файл или не указали важную информацию в комментарии к коммиту.

## git config
Удобный способ для настройки параметров конфигурации в инсталляции Git. Обычно эту команду используют сразу после установки Git на новую машину разработчика.

## git fetch
С помощью команды извлечения можно загрузить ветку из другого репозитория вместе со всеми связанными с ней коммитами и файлами, однако при этом изменения не будут интегрированы в локальный репозиторий. Благодаря этому вы сможете проверить изменения перед слиянием с проектом.

## git log
Позволяет изучить предыдущие версии проекта. Эта команда имеет несколько параметров форматирования, с помощью которых можно отобразить снимки состояния после выполнения коммитов.

## git merge
Эффективный способ интеграции изменений из разошедшихся веток. После разветвления истории проекта командой git branch можно использовать команду git merge, чтобы объединить отдельные ветки.

## git pull
Команда git pull — это автоматизированная версия команды git fetch. Она загружает ветку из удаленного репозитория и сразу же объединяет ее с текущей веткой. Эта команда представляет собой git-эквивалент команды svn update.

## git push
Команда git push противоположна команде извлечения (с некоторыми оговорками). С ее помощью можно перенести локальную ветку в другой репозиторий и без труда опубликовать поступивший код. Эта команда похожа на svn commit с тем исключением, что она отправляет не один набор изменений, а серию коммитов.
## git rebase
С помощью команды перебазирования можно переместить ветки и избежать ненужных коммитов слияния. Полученную линейную историю зачастую намного легче понять и изучить.

## git reflog
Git отслеживает изменения в конце веток с помощью механизма журналов ссылок (reflog). Он позволяет вернуться к наборам изменений, даже если на них не ссылается никакая ветка или тег.

## git reset
Отменяет изменения в файлах в рабочем каталоге. Эта команда сброса позволяет очистить или полностью удалить изменения, которые не были отправлены в публичный репозиторий.

## git status
Показывает состояние рабочего каталога и проиндексированного снимка состояния. Эту команду можно выполнять в сочетании с *git add* и *git commit*, чтобы узнать, что именно будет включено в следующий снимок.


