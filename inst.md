# Инструкция по работе с Git

## Начальная работа с системой контроля версий

### **Команда git --version**
*git --version* - команда для просмотра версии git


>![git version](./assets/git_version.png)

### **Команда git init**

*git init* - инициализируем пустой репозиторий

>![git init](./assets/git_init.png)

### **Команда git status** 

*git status* - проверяем текущее состояние файлов

>![git status](./assets/git_status.png)

### **Команда git add**
*git add* - добавляем версионность файлу

>![git add](./assets/git_add.png)

### **Команда git commit**

*git commit -m "Message"* - команда для фиксации изменений файлов

>![git commit](./assets/git_commit.png)

### **Команда git log**

*git log* - вывод истории коммитов в хронологическом порядке

>![git log](./assets/git_log.png)

### **Команда git diff**

*git diff* - вывод изменений на текущий момент по отношению к последнему коммиту

>![git diff](./assets/git_diff.png)

### **Команда git checkout**

*git checkout master либо хэш-номер коммита* - переход между изменениями либо возврат к текущему состоянию

>![git checkout](./assets/git_checkout_branch.png)

>![git checkout master](./assets/git_checkout_master.png)

### **Команда git branch**

**git branch** - просмотр списка веток

>![branch_list](/assets/git_branch_list.png)

**git branch <имя ветки>** - создание новой ветки.

>![branch_new](./assets/git_new_branch.png)

**git checkout -b <имя ветки>** - альтернативное создание новой ветки, с последующим переходом на неё.

>![checkout_branch](/assets/git_new_branch_alt.png)

### **Слияние веток и конфликты**

Для слияния веток используется команда **git merge <имя ветки>**. Вызов команды надо осуществлять из ветки в которую будет производиться слияние. К примеру, если мы хотим добавить наши изменения из ветки **slave** в ветку **master**, то команда будет выглядеть следующим образом: **git merge slave**.

>![git_merge](/assets/git_merge.png)

При слиянии веток возможен конфликт. Чаще всего он возникает из-за одновременных изменений части текста в двух ветках.

>![git_conf](/assets/git_conflict.png)

Для binary файлов вариантом решения конфликта является сохранение одного из вариантоа файлов как основного.

>![git_bin](/assets/git_conflict_bin.png)

После того, как конфликт будет разрешён, при попытке слияния веток, мы должны увидеть следующее сообщение:

>![git_resolved](/assets/git_config_resolved.png)