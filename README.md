# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains
1. информационные команды 

   * *git --version* - команда для проверки версии git
   ![](images/git_version.JPG "пример выполнения команды")

   * *git status* - проверяем текущее состояние файлов
   ![](images/git_status.JPG "пример выполнения команды")

   * *git log* - вывод истории коммитов в хронологическом порядке
   ![](images/git_log.JPG "пример выполнения команды")

2. комманды фиксирующие изменения файла или файлов

   * [*git init*](https://git-scm.com/docs/git-init) - инициализация пустого репозитория

   * [*git add .\имя файла.расширение*](https://git-scm.com/docs/git-add) - добавляем версионность файлу

   * *git add .* - добавляем версионность всем файлам в папке

   * [*git commit -m "smth"*](https://git-scm.com/docs/git-commit) - команда для фиксации изменений файлов

   * *git commit -am "smth"* - версионность и коммит в одной команде

3. команды показывающие изменения в разных коммитах 
   
   * *git diff* - вывод изменений на текущий момент по отношению к последнему коммиту

   * *git checkout хэш_коммита* - переходим к содежанию файла при данном коммите

   * *git checkout master* - переход к текщему состоянию 

4. команды для взаимодействия с ветвями
   
   * *git branch* - показ всех созданных веток и обозначение той, которая активна

   * *git branch smth* - создание новой ветки с именем smth

   * *git checkout smth* - переход с текущей ветки на ветку smth

   * *git checkout -b smth* - создание ветви smth и переход на нее

   * *git merge smth* - слияние ветки smth с текущей ветвью

5. команды для работы с удаленным репозиторием.

   * [*git clone url*](https://github.com/git-guides/git-clone) - создание копии удаленного репозитория с адресом url в локальном

   * [*git remote*](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories) - просмотр информации о подключенных удаленных репозиториях

   * [*git remote add name url*](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories) - подключение удаленного репозитория с именем name и адресом url

   * [*git pull*](https://github.com/git-guides/git-pull) - запись изменений из удаленного репозитория в текущую ветвь локального

   * [*git push*](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository) - запись изменений из локального репозитория в удаленный