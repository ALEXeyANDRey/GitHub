# Инструкция по работе с Git

## Начало работы с репозиторием
Команда,которая создаёт локальный репозиторий
> git init

Если вы до этого не водили имя/почту, то нужно их добавить
>git config --global user.name Имя

>git config --global user.email Почта



## Добавление изменений 
Для того чтобы начать остлеживаный файл с именем file_name:
> git add file_name
И чтобы зафиксировать все файлы, которые мы отслеживаем:
>git commit -m "some message"



## Отслеживание состояния репозитория 
Показывает состояние репозитория, то есть файлы которые были добавлены в репозиторий или изменены:
> git status

Показывает историю коммитов:
> got log

Показывает разницу между текущим состоянием и тем что отслеживается:
>git diff



## Переход между коммитами
Можно перейти к прошлому коммиту командой:
>git checkout commit_code

commit_code - код коммита, который можно посмотреть в git log

Для того чтобы вернуться к актуальному комиту:
> git checkout master

## Ветки в git

Чтобы посмотреть все ветки, нужно ввести:
> git branch

Чтобы создать новую ветку с именем branch_name:
> git branch branch_name

Переход к ветке branch_name:
> git checkout branch_name 

## Слияние веток и решение конфликтов

Чтобы слить ветку branch_name в текущую, нужно:
> git merge branch_name

В  случае возникновения конфликта при merge, нужно выбрать какой из вариантов нам нужен (или оставить оба) и по необходимости модифицировать их

## Справка
Для того чтобы вызвать справвку по какой-то команде, нужно дописать к ней тег --help
> git add --help

>git commit --help

>git merge --help

> git checkout --help

>git branch --help

## Удаление веток:
Для удаления веток branch_name, нужно ввести:

> git branch -d branch_name
она удалиться есть нет никаких ошибок

## Слияние веток и решение конфликтов

Чтобы слить ветку branch_name в текущую, нужно:
> git merge branch_name

## Клонирование репозитория
Клонировать удаленный репозиторий в локальный :
>git clone https://github.com/(ссылка репозитория с удаленного репозитория)
Oтправляем коммит в master в удалённом репозитории
> git push
