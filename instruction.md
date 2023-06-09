## **Instruction to work Git**

![Git emblemm](gitt.png)

## Создание нового локального репозитория

Для создания нового репозитория (инициализации) нужно ввести команду: 

git init

## проверка состояния репозитория

Для того чтобы проверить текущее состояние репозитория необходимо использовать команду:

git status

## Добавление изменений к отслеживанию

 Для того, чтобы Git начал сдедить за изменениями в файле необходимо использовать команду:

git add "имя файла" 

## Добавление комментариев к изменениям

Для того, чтобы начать коммитить(комментировать) изменение в проекте, нужно ввести слудующую команду: 

git commit 

Если необходимо указать что именно было изменено в файле необходимо указать это после этого знака  (-m)  в кавычках, как в примере ниже

git commit -m "сообщение о изменениях"

А если изменения необходимо зафиксироать сразу же в индекс файла необходимо использовать следующую команду: 

git commit -am "сообщение о изменениях"

## Список всех изменений

Для того, чтобы посмотреть список изменений в файле необходимо ввести следующую команду:

git log

Если необходимо сократить хешномера коммитов и увидеть список в сокращенном и упрощенном варианте с которым в маленьком проекте будет удобнее работать, то лучше использовать команду ниже:

git log --oneline

Если список сокращенных имен не требуется, то можно вернутся к прежнему списку следующей командой:

git log --all

А Возврат из команды конкретного комментария к общему скиску сокращенных комментариев делается командой ниже:

git log --all --oneline

## Сравнение совершенных изменений в проекте

Сравнение совершенных изменений в проекте можно посмотреть посредством этой команды:

git diff

А если требуется посмотреть изменения к конкретном комментарии, то к нему можно будет обратиться по его номеру указав его в кавычках после команды как на примере ниже:

git diff "номер коммента"

Сравнение двух конкретных комментариев можно воспроизвести, введя следующую команду: 

git diff "номер коммента" "номер коммента"

## Выбор конкретного комментария с подробным его описанием

Данная команда позволяет просматривать наши действия и показывает где находимся в данный момент (на каком комментарии):

git checkout "номер коммента"

А Возыврат во главу к списку комментов к последнему комментарию осуществляется посредством команды:


git checkout master

##  **Ветвление**

## Просмотр имеющихся веток

Чтобы проверить наличие веток в проекте необходимо ввести команду: 

git branch

Затем, чтобы переключаться между ветками необходимо использовать команду:

git checkout "имя ветки"

Таким образом можно изменять документ в новой ветке, сохравнив оригинальную версию, до создания новой ветки. После чего, если нам потребуется вернуться
к основной версии проекта, то мы должны использовать команду:

git checkout master

Для того, чтобы удалить ветку необходимо ввести команду:

git checkout -d "имя ветки"

Но допустим, если командная строка спросит вас действительно ли вы хотите удалить ветку ? Тогда надо будет ввести почти такую же команду, что и команда выше, но за одним исключением необходимо использовать -D большое после слова checkout. Этой командой мы подтверждаем удаление ветки.
Пример:
    
git checkout -D "имя ветки" 

## Удаленные репозитории