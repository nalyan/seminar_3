# Инструкция по работе с git

## Что такое git
Git - это одна из реализаций распределенных систем контроля версий, что позволяет иметь версионность как в локальном репозитьарии, так и в удаленном репозитарии (общем для всех). Git является на данный момент самой популярной системой контроля версий.

## Подготовка репозитория
Для создания репозитария используется команда *git init*. В терминале в папке с будущим репозитарием достаточно написать *git init*, и эта папка станет репозитарием.

## Создание коммитов
Для создания коммитов необходимо использовать команду *git commit -m "комментарий к коммиту"*

### Просмотр состояния репозитория
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

## Слияние веток и решение конфликтов

## Удаление веток