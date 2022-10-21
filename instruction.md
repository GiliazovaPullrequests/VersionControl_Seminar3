# `Instruction to Markdown!`

>## *Git commands/orders*.

*git version* -команда проверки версии git.

*git init* - инициализируем пустой репозиторий.

*git status* - проверяем текущее состояние файлов.

*git add имя_файла.расширение* - добавляем версионность файлу.

*git add . file name* - добавляем версионность всем файлам в папке.

*git commit -m "Описание коммита"* - фиксация изменений файлов.

*git commit -am "описание коммита"* - добавляем версионность всем файлам в папке + фиксация изменений файлов, фактически заменяет *git add + git commit -m*.

*git log* - вывод истории коммитов в хронологическом порядке.

*git diff* - вывод изменений на текущий момент по отношению к последнему коммиту.

*git checkout хеш_символы* - переключение на нужный коммит.

*git checkout имя_ветки* - переключение на нужную ветку.

*git checkout -b имя_ветки* - создание новой ветки и автоматический переход на неё.

*git branch master/название_нужной_ветви* - переключение между ветками.

*git branch* - список существующих веток с отметкой нашего местоположения.

*git merge Название_ветки* - добавление в ветку master побочной ветви.

*git merge lists* - добавляет в текущую ветку.

*git branch -d Название_ветки* - удаление ветки.

*git log --graph* - визуальное отображение веток со своими коммитами.

*git reflog* - текстовое, в столбик, отображение веток со своими коммитами.

*clear* - очистка терминала.

*mkdir имя файла* - создание нового файла из терминала.

>>### *Git remote orders* 

*git clone ссылка* - команда для загрузки удаленного репозитория.

*git remote add origin ссылка репозитория* - добавление удаленного репозитория.

*git branch -M master/(main IOS)* - указываем основную ветку.

*git push -u origin master* - отправляем в интернет (на удаленный репозиторий).

*git push* - отправляем репозиторий в интернет, а именно в репозитории GitHub.

*git pull* - загрузка изменений из интернета и слияние (автоматический merge) файлов.  

## *Text selection.*

Symbol # - Header/Title (supports 6 levels).

Symbol = and - underline (at least 3 in a row) allocate header of first (=) and second (-) levels.

Symbol (** _ **) or (__ __) bold inscription.

Symbol (* _ *) or (_ _) italic inscription.

Symbol (** _ **) italic bold inscription.

Alternative methods of text selection with bold and italic, can be combined as:  ( _ ** _ ** _ ).

Symbol (~~) crossed out inscription.

Symbol (>) in start of the line make Quotes to previous line.

## *Lists.*

Symbol (*) or (+) in start of the line - list inscription. Like this:
* Element 1.
* Element 2.
+ Etc.

Symbol (1,2,3) in start of the line - numbered list inscription. Like this:
1. Element.
2. Element.
3. Etc.

## *Pictures.*

To insert images into text:

![Почти жиза для моей работы в картинке!](123.jpg)

## *Links.*

!(https://git-scm.com/book/ru/v2/Git-%D0%B8%D0%B7%D0%BD%D1%83%D1%82%D1%80%D0%B8-%D0%A1%D1%81%D1%8B%D0%BB%D0%BA%D0%B8-%D0%B2-Git) 

+ I hope theme of this link is another big lesson!?

## *Table.*

__*My little pigs*__
|Number|Name|	Born|	Weight|
|:---:|:---:|:---:|:---:|
1|Priscilla|	12.06.2022|	22|
2|Cirilla|	12.06.2022|	23|
3|Jason|	03.07.2022|	19|
4|Monika|	03.07.2022|	18|

## *Quotes.*

Сережа сказал: 
 >Я устал.
 >>Или нет, но сделаю вид, что да - подумал Сережа в голове.
 
 А Маша сказала: 
 >Устал и устал, кого это волнует?
 >>Меня действительно волнует, но я никогда в этом не признаюсь - звонкой мыслью пронеслась грустная мысль Маши.

## `Conclusions.`

# Remote repositiry GitHub.

+ Предоставляет майкрософт.
+ Самый поопулярный сервис Git.
+ Много полезных функций.
+ Огромный архив различного кода.

## Start GitHub algorithm. 

### Действия при начале работы с GitHub:

+ Cоздать аккаунт на Github.com.
+ Cоздать локальный репозиторий.
+ Cвязать локальный и удаленный репозиторий. Гит при создании нового репозитория подскажет как это можно сделать.
+ Отправить локальный репозиторий в удаленный на Гитхаб (push).
+ Произвести изменения с "другого компьютера".
+ Выгрузить актуальное состояние из удаленного репозитория (pull). 

### Действия при работе в стороннем проекте:

+ Делаем "вилку" (fork) интересующего нас репозитория.
+ Делаем (git clone) для нашей версии этого репозитория.
+ Создаем ветку с предлагаемыми изменениями.
+ Производим все изменения только в этой ветке.
+ Отправляем изменения на свой аккаунт (push).
+ И после этого на GitHub появится возможность отправить pull request.