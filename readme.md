# Инструкция по работе с git

## Что такое гит?
***Git*** - самая популярная реализауия распространнённой системы контроля версий (версионность поддерживается и на сервере , и у каждого клиента). Самой распространнённой реализацией ***Git*** является (*GitHub*)[htps://github/com]

## Подгатовка репазитория.
Для создания репозитория используется команда "git init". Для этого необходимо открыть в терминале папку с будующим репозиторим и написать "git init'.

## Создание коммита.

### Добовление файлов 
Для добовления файла к новому коммиту используется команда *git add*. Используется она следующим образом: в терминале с папкой-репозиторием пишется *git add<название файла>*.

### Создание коммита 
Для создания новой фиксации(коммита) используется команда *git commit*. Для этого в терминале с папкой-репозиторием пишим "git commit -m "<сообщение к коммиту>". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***

## Перемещение между сохранениями.
Для переключениями между фиксациями(коммит) используется команда *git checkout*. Для этого необходимо как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш(номер). Росле чего в терминале с папкой-репозиторием надо написать *git checkoot <хеш коммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором ни какие следующие коммиты сохранятся не будут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Журнал изменений.
Для просмотра историй измененний спользуется команда "git log". Для этого в терминале с папкой-репозиторием необходимо написать "git log". 
### Просмотр списка веток.
Для просмотра веток используется команда *git branch*. Выделеная зелёным ветка, это та на которой мы находимся.


## Ветви в гит и переход между ними.
Для того что бы создать новую ветвь, в которой мы будем работать не изменяя основную, необходимо в терменале с папкой-репозиторием написать *git branch <название новой ветки>*. 
### Создание веток в git.
Для создания новой ветки спользуется команда "git branch". Для этого в терминале с папко0-репозимтоия необходимо написать "git branch<название внтви>".
### Перемещение между ветками
Для перехода на другую ветку используется команда *git checkout*. Для этого в терменале с папкой-репозиторием пишем *git checkout<название ветви>*

### Переход.
Для перехода из одной ветви в другую необходимо в терменали папки-репозитория написать *git branch <название необходимой ветви>*. Что бы узнать сколько у нас ветвей, их названия и в какой из них мы находимся в данный момент, необходимо в термнали папке-репозитория написать каманду *git branch*.


## Слияние веток и разрешение конфликтов.
Для слияния ветвей необходимо для начала перейти в ту ветве, к которой мы будем добовлять новую. Находясь в нужной нам ветви мы пишем в терминале с папкой-репозиторием команду *git merge <название ветви которую хотим добавить>* При слиянии могут возникнуть конфликты из-за разной хранимой информации. Есть несколько решений этой проблемы:
1. Можно воспользоваться автоматической предлагаемой функцией и оставить либо имеющуюся информацию данной ветви, либо информацию из добавленной ветви выбров соответствующие команды в выделенном поле.
2. Можно вручную оставить ту информацию которая нас интересует. Для этого мы просто вручную удоляем все не нужные нам элементы в выделенном поле.  

## Удоление веток.
После того как информация из второстепенной ветви была слита с основной веткой, второстепенную можно удолить. Для этого в терминале с папкой-репозиторием необходимо ввести команду *git branch -d <название удоляемой ветви>*. 
