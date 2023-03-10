# **Инструкция по работе в GIT**

# *Описание команд в GIT*

## Рассмотрим основные команды используемые в работе ##

команда *git init* - отвечает за создание репозитория. после ввода данной команды GIT начинает отследивание файла

команда *git add <имя_файла>* команда добавляет файл в проект 

команда *git status* - отображает статус происходящего с папкой или файлом

команда *git commit* - берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок

команда *git commit -m* - фиксирует внесенные изменения и позволяет добавить коментарий о них

команда *git commit -am* - в дополнение к включению сообщения о фиксации, эта опция позволяет пропустить этап подготовки. Добавление -aавтоматически добавит все файлы, которые уже отслеживаются Git (изменения в файлах, которые вы зафиксировали ранее).

команда *git commit -a* - совершит коммит, автоматически индексируя изменения в файлах
проекта. Новые файлы при этом индексироваться не будут! Удаление же файлов
будет учтено.

команда *git log* - позволяет отслеживать какие были изменения 

команда *git log --oneline* - выведет на каждый из коммитов по строчке, состоящей из хэша
(уникального идентификатора каждого коммита)

команда *git log --all* - покажет информацию по всем веткам

команда *git log --oneline --all* - Выводим полный граф коммитов, отводя по одной строке на коммит.

команда *git checkout* - команда git checkout позволяет переключаться между последними коммитами

команда *git diff* - данная команда позволяет просмотреть выполненные изменения между сохранениями

команда *git diff <1> <2>* - покажет изменения между двумя отдельными файлами, ветками.

## Работа с изображениями ##
для вставки изображения необходимо выполнить команду **![текст если изображение отсутсвует](имя файла)**

проверяем вставку картинки ![phote](Git.jpeg)
если файла с каритнкой не будет, то будет отображаться надпись в квадратных скобках.

## Работа по слиянию веток ##
для слияния веток используется команда git merge имя ветки. если уже есть какой-то текст, то конфликт необходимо будет разрешить. указать руками, что мы добавляем, а что удаляем. после слияния сохраняемся и удаляем ненужные ветки

## Игнорирование файлов ##

для игнорирования файлов необходимо создать специальную папку и переместить в нее файл, что бы GIT перестал отслеживать этот файл. разберем на нашей картинке

необходимо создать файл с именем *.gitignore*

в данный файл прописываем имя файла, который мы хотим игнорировать *Git.jpeg*

сохраняем этот файл и комитим. важно сохранять надо именно файл *.gitignore*

## Команды для работы с ветками ##

команда *git branch* выводит список всех созданых веток

команда *git branch имя ветки* создает новую ветку

команда *git merge имя ветки* производит слияние двух веток(переносит всю информацию из указанной ветки в ту ветку где мы находимся)

команда *git branch -d* удаление ветки. удалять ветку можно когда все данные из нее уже перенесены

команда *git log --graph* показывает комиты по веткам

## Удаление веток ## 
После слияния удаляем ветки командой git branch -g <имя ветки>

## Работа с удаленным репозиторем

Для работы с удаленным репозиторием необходимо зарегестрироваться на https://github.com/

при работе в удаленном репозитоии учетная запись должна быть активна.

создаем новый репозиторий. страница создания информативная. читаем и делаем

После создания удаленного репозитория попадаем на старницу дальнейший действий. Система предлагает 3 варианта действия

*создайте новый репозиторий в командной строке*

*добавить существующий репозиторий* 

*взять код из другого истояника*

рассмотрим второй вариант. все команды так же прописаны на сайте. нам неообходимо поправить наименование ветки

первый раз при выполнении команды *git push -u origin master* необходимо пройти автоизацию на githab

После выполнения всех команд данные загружаются в удаленный репозитоий. достаточно обновить страницу git hab

любые изменения сделанные в локальном репозитории автоматически не загружаюттся на git hab. для "отправки" необходимо использовать команду *git push*

вносить изменения в проект можно так же на git hab. для этого проваливаемся в наш файл на удаленном рапозитории и нажимаем на редактирование.








