# Инструкция по работе с git

## Что такое git
Git - это одна из реализаций распределенных систем контроля версий, что позволяет иметь версионность как в локальном репозитьарии, так и в удаленном репозитарии (общем для всех). Git является на данный момент самой популярной системой контроля версий.

## Подготовка репозитория
Для создания репозитария используется команда *git init*. В терминале в папке с будущим репозитарием достаточно написать *git init*, и эта папка станет репозитарием.

## Создание коммитов
Для создания коммитов необходимо использовать команду *git commit -m "комментарий к коммиту"*

## Просмотр состояния репозитория
Для просмотра состояния репозитория используется команда *git status*. Для этого необходимо в папке с терминалом написать *git status*, и увидеть несколько возможных состояний:
1. Nothing to commit - это значит, что репозитории нет абсолютно никаких изменений
2. Unversioned file

## Добавление файла к сохранению
Для добавления файла в текущий коммит используется команда *git add*. Для этого достаточно в терминале с папкой репозитария написать *git add <название файла>*.

## Фиксация изменений
Для сохранения коммита используется команда *git commit*. Для этого в терминале с папкой репозитария необходимо написать команду *git commit -m "<сообщение к коммиту>"* Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***

## Журнал изменений
Для просмотра истории коммитов, т.е. истории наших изменений используется команда *git log*. Для этого необходимо в терминале с папкой-репозиторием написать *git log*.

## Перемещение между "сохранениями"
Для того, чтобы перемещаться между коммитами, необходимо использовать команду *git checkout*. Для этого в терминале с папкой репозитария необходимо написать *git checkout <номер коммита>*. Номер коммита берётся из истории изменений. После такого "перемещения" мы попадаем в состояние **Detached head*. Для возвращения в обычное состояние используется команда *git checkout master*.

## Ветки в git
Для создания черновиков в git используются ветки в которых можно проводить редактирование с последующим внесением законченных изменений в чистовую версию. Для создания ветки используется команда *git branch название ветки*. Для переключения между ветками используется команда *git checkout название ветки*.

## Слияние веток и решение конфликтов
Для слияния веток используется команда *git merge <название ветки, из которой сливаются изменения>*. Изменения вносятся в текущую ветку.

В случае, если строка в основной ветке отличается от строки в другой ветке, из которой осуществляется слияние, возникает конфликт версий. В данном случае необходимо вручную выбрать нужный вариант:
1. Оставить версию из текущей ветки
2. Принять изменения из другой ветки
3. Принять оба варианта
4. Создать новый вариант

## Удаление веток
Для удаления веток используется команда *git branch -d <название ветки>*

## Получение удаленного репозитория
Для того, чтобы скачать удаленный репозиторий, необходимо использовать команду *git clone*. В терминале, в котором открыта любая другая пустая папка, необходимо написать *git clone <ссылка на репозиторий>*. Репозиторий скачается в папку, название которой будет совпадать с названием репозитория.

## Скачивание изменений с удаленного репозитория
Для того, чтобы скачать изменения с удаленного репозитория, необходимо использовать команду *git pull*. В терминале с папкой с репозиторием, связанным с удаленным репозиторием, пишем *git pull origin <название ветки>* для того, чтобы принять изменения из указанной ветки удаленного репозитория в текущую ветку.

## Отправка изменений в удаленный репозиторий


