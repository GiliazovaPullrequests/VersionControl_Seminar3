# VersionControl_Seminar3 Homework

# <span style="color:green">*Инструкция по git*</span>

## 1. Команды для работы с локальными репозиториями

|<span style="color:orange">Команда</span>|<span style="color:orange">Назначение</span>|
|-----|------------|
| git <span style="color:blue">**version**</span>| проверка версии git     |
| git <span style="color:blue">**init**</span>|инициализируем пустой репозиторий |
| git <span style="color:blue">**status**</span>| проверяем текущее состояние файла |
| git <span style="color:blue">**add**</span> *имя файла.расширение*| добавляем версионность файлу|
| git <span style="color:blue">**commit -m</span>** "*message*"|фиксируем изменения в файле (перед комиитом файл должен быть обязательно сохранен) |
| git <span style="color:blue">**commit -am</span>** "*message*"|позволяет сделать commit без add |
| git <span style="color:blue">**log**</span>|вывод истории коммитов в хронологическом порядке |
| git <span style="color:blue">**log --graph**</span>| вывод истории коммитов в виде схемы-дерева|
| git <span style="color:blue">**diff**</span>| вывод изменений на текущий момент по отношению к последнему коммиту|
| git <span style="color:blue">**checkout**</span> *хэш код коммита или имя ветки*|переход между версиями или ветками |
| git <span style="color:blue">**branch**</span> | вывод списка веток (звездочкой отмечена текущая ветка)|
| git <span style="color:blue">**merge**</span> *имя ветки* | слияние ветки с текущей|
| git <span style="color:blue">**branch -d**</span> *имя ветки* |удаление ветки |
| <span style="color:blue">**clear**</span>  |очистить терминал | 

## 2. Команды для работы с удаленными репозиториями

|<span style="color:orange">Команда</span>|<span style="color:orange">Назначение</span>|
|-----|------------|
| git <span style="color:blue">**clone**</span> *ссылка на удаленный репозиторий*| создать локальную копию удаленного репозитория   |
| git <span style="color:blue">**cd**</span> *имя локальной копии удаленного репозитория* |перейти из папки, созданной в компе, в папку локальной копии удаленного репозитория |
| git <span style="color:blue">**push**</span>| добавляем изменения, сделанные в локальном репозитории, в удаленный репозиторий |
| git <span style="color:blue">**pull**</span> | добавляем изменения, сделанные в удаленном репозитории, в локальный репозиторий|

## 3. Прочие заметки

* <span style="color:orange">**.GITGNORE**</span>
    
    1. Создается файл с  названием <span style="color:blue">**.gitignore**</span>. 
    2. В него добавляем имя и расширение файлов, которые git должен игнорировать (не отображать их как <span style="color:red">untracked files</span> при команде git <span style="color:blue">**status**</span> ). Используется для объемных файлов, которые не принято загружать в git, например, для изображений.

* <span style="color:orange">**FORK**</span>

  <span style="color:blue">**Fork**</span> - это функция <span style="color:green">*GitHub*</span>, которая используется для того, чтобы создать для себя копию чужого репозитория (удаленную).

* <span style="color:orange">**PULL REQUEST**</span>

  Pull request - это запрос на внесение изменений в чужой репозиторий. Для того, чтобы сделать pull request, необходимо:

  1. Сделать <span style="color:blue">**fork**</span> на <span style="color:green">*GitHub*</span>;
  2. Git <span style="color:blue">**clone**</span>; 
  3. Git <span style="color:blue">**cd**</span>;
  4. Создать новую ветку;
  5. Git <span style="color:blue">**checkout**</span> в созданную ветку;
  6. Внести изменения;
  7. Git <span style="color:blue">**add**</span>;
  8. Git <span style="color:blue">**commit**</span>;
  9. Git <span style="color:blue">**push**</span> (возникнет ошибка, в тексте ошибки будет подсказка);
  10. Вставить текст из подсказки (что-то типа *git push --set-upstream origin branch_name*);
  11. У меня на <span style="color:green">*GitHub*</span> в форкнутом репозитории появляется зеленая кнопка <span style="color:green">**Compare&Pull Request**</span>;
  12. У владельца репозитория тоже появляется какой-то запрос.

-----------------------------

 
# <span style="color:green">*Git instructions*</span>

