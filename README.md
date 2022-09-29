__Дооформить инструкцию по работе с Git, используя возможности Markdown (цитаты, картинки, ссылки и т.п.) и приложить свой проект в заархивированном виде (всю папку целиком).__
<style> .notice_Me {color: #8A2BE2 ; font-size:200%}</style>
## Ну что, начнём с начала.
До любых действий git нужно скачать. Вместе с ним можно опционально скачать графический интерфейс. 
Основные команды консоли привязаны не к терминалу, а к версии гита. Есть отличный шанс того что они не изменятся пока Мы живы, потому что обратную совместимость никто не отменял.
Всё начинается с ключа git, так Мы без мышки обращаемся к программе... не скажу к какой, это секретный секрет. Кстати можно и с мышкой тоже это самое делать:

 есть например git kraken, который советуют на подготовительном курсе по гиту, он красивый, удобный, и тормозит на служебном ноутбуке...

 Есть так же git GUI, выглядит как крепкий скворечник. Идёт в комплекте с гитом. Не пользовался, надо потом потестить.

 В том что касается консоли у visual studio code нет на неё монополии. Начнём с того что она первоочёдно не выводит какую-то свою консоль, а пользуется тем что предоставляет среда. Для "окон" это powershell. Но cmd тоже есть! К чему это Я ... для работы с гитом без редактирования файлов можно просто открыть одну из этих консолей без посредников.

 А если нужно ещё и в файлах что-то писать, то можно воспользоваться консолью которая идёт в комплекте с гитом: git bash. там у нас соответственно появляются команды touch для создания файла, echo для редактирования, и cat для чтения. Мне впрочем что-то подсказывает, что в консолях винды можно то же самое сделать.
 __edit: можно познакомить git bash с vscode.__

Своя собственная консоль есть и в git kraken. С софтом пока всё.

## Перейдём к базовым командам.
|Команда&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|Давай поговорим|
|:-|---|
|||
|git init|Всё всегда начинается с команды git init.  Она создаёт или считывает репозиторий по !этому адресу. Так что глаза на лоб, и смотрим где мы собираемся работать.|
|git --version|Можно, посмотреть сразу версию гита (git --version). Мало ли.|
|###|Для первейшего запуска нужно указать кто Мы, как Нас искать, и что Мы хотим для удобства:|
|git config —global user.name "[name]"|My name is Hi!| 
|git config —global user.email "[email]"|don't.|
|git config —global color.ui auto|подсветка синтаксиса|
|git config —global core.editor "[program]"|дефолтный редактор, например vscode|
|git --config list|позже можно проверить шо Мы там накликали с git --config list|

После того как мы обнюхали папку init'ом...


|Команда&nbsp;&nbsp;&nbsp; |Комментарий|
|:-|---|
|git status| ...можно написать git status. Он напишет что всё как раньше, или что раньше было лучше.|

Перемены формируются через кусочки информации называемые **коммиты**. Оперировать ими, _на верхем уровне_ просто:
|Команда&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; |Комментарий|
|:-|---|
|git add  #filename|добавляет #filename в заготовку коммита. Чтобы #filename можно было добавить он должен измениться, т.е. Мы его меняем и сохраняем. Гит статус говорит "раньше было лучше", а Мы ему- "теперь всё будет по-новому!"|
|git add .| добавляет к коммиту все изменения сразу|
|git add -f| добавляет файлы из .gitignore если такие есть. _А чистит ли он гитигнор? Надо проверить._|
|git add -p #filename| разбивает дельту на блоки и позволяет отклонить или принять изменения по частям. Интересная штука! Проверяем на практике, |
|git add -e| Модифицирует файл во временной папке коммита на лету. Они это называют index. Что нужно знать о -e: _There are also more complex operations that can be performed. But beware that because the patch is applied only to the index and not the working tree, the working tree will appear to "undo" the change in the index. For example, introducing a new line into the index that is in neither the HEAD nor the working tree will stage the new line for commit, but the line will appear to be reverted in the working tree. **Avoid using these constructs, or do so with extreme caution.**_ Т.е. ребята с сайта _сами_ говорят "не лезь". Но для чего-то же они это добавили...|
|rm --cache #filename|Если мы отдали файл в коммит но передумали, то можно сказать git rm --cache #filename чтобы пропустить файл в этот раз. Можно пропускать систематически, для этого есть файл .gitignore но о нём позже.|
|git commit| git commit в общем виде создаёт снимок изменений которые Мы согласились объявить через git add.|
|###|С ней в комплекте есть несколько интересных ключей, включая эти:|
|git commit -m "text"| задаёт комментарий без привлечения внешнего редактора|
|git commit -a| git add . +git commit #предложит описать коммит|
|git commit -am "text"| git add . +git commit -m "text"|
|git checkout #hash| двигает нас по коммитам, смещает при этом head. Тут есть нюанс: если после чекаута Мы сделаем перемену, любую, и закоммитим её, то у нас получатся коммиты на которые нет ссылок. Сборщик мусора в гите такой же как в питоне( или vice versa), т.е. удаляет то что нельзя получить из консоли. Так шо обережно, можно накосячить. Интернет говорит, что лучше пользовать ...|
|git revert |эта радость генерирует коммит-противоход, возвращая текущий, ну т.е. уже следующий после head коммит в состоянии того который ревёртом был вызван. Безопасно, а главное делать ничего особо не надо. |
|git reset | сбрасывает ветку до некоего коммита аж тремя способами : mixed soft и hard. Хард опасен, перемещает head(см.checkout).|
|<div class="notice_Me"> ### </div>| <span style="color:purple;font-weight:700;font-size:18px"> let Us proceed.</span> |
|git clone #url|Как аргумент принимает ссылку. Ссылка может быть как сразу на чужой репозиторий, так и на _наш форк_ чужого репозитория. Оба решения на выходе дают нам чужой код локально, намагниченный на носитель, но есть различия. Форк даёт нам администраторские права на нашу копию кода. Изменения которые мы вносим в локальную версию форка можно выгружать без ограничений( ну разве что ограничения по объёму файла но для тхт файлов какая это проблема?).Дальше отношения форка  и _мастера_ напоминают отношения между локальной и удалённой версией репозитория. Мы можем предлагать изменить код-_мастер_, но: * пуши тут называются  pull requestы; * наши пулл реквесты тут должен одобрить куратор _мастера_..  Если же Мы клонируем чужую репку напрямую есть отличный шанс ничего не выгрузить в сеть потому что полномочия. Репозиторий может и публичный, но право изменения есть у ограниченного числа пользователей. Так вот... нет авторизации== нет прямого редактирования _мастера_.|
|git pull| "На себя". Копирует файлы с удалённого репозитория сюда и пытается их адаптировать, ну т.е. merge. Принимает как аргументы имена веток типа git pull origin main, где на первом месте имя ветки ~~удалённой~~ отдалённой **:))** , а на втором- локальной, целевой. |
|git push|"делимся". Отправляет файлы _туда_! _Скорее всего там тоже пытается их смёржить, можно даже попробовать потом это проверить..._ Тоже принимает имена веток как аргументы |


Есть и другие команды, но по итогу мы строим вот это: ![здесь не будет вашей рекламы...](Стадии_принятия_файла.jpg)