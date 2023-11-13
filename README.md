# Лабораторная работа №6
___
## Цель работы
Изучение базовых возможностей системы
управления версиями, опыт работы с Git Api, опыт работы с локальным и
удаленным репозиторием.
___
## Ход работы
### 1. Создание копии репозитория (Fork)
### 2. Настройка клиента ([см. рис. 1](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/1.png))
```
git config --global user.name "4218 Сован В.Д."
git config --global user.email slavasovan@gmail.com
```
### 3. Клонирование удалённого репозитория на компьютер ([см. рис. 2](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/2.png))
```
git clone https://github.com/SlavaSovan/LR6
```
### 4. Добавление file.txt через интерфейс GitHub ([см. рис. 3](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/3.png)).Подтяжка изменений в локальный репозиторий ([см. рис. 4](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/4.png))
```
git pull
```
### 5. Получение истории операций для каждой из веток

master ([см. рис. 5](
https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/5.png)):
```
git log
```
branch1 ([см. рис. 6](
https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/6.png)):
```
git log origin/branch1
```
### 6. Просмотр последних изменений ([см. рис. 7](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/7.png))
```
git branch -v
```
### 7. Слияние в ветку master
```
git merge origin/branch1
```
Отредактирован файл ([см. рис. 8](
https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/8.png))
и сделан коммит ([см. рис. 9](
https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/9.png))
для разрешения конфликта.

### 8. Сделаны несколько изменений с коммитами ([см. рис. 10](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/10.png))

Добавление всего содержимого рабочего каталога в индекс:
```
git add .
```
Вывод состояния файлов в рабочем каталоге и индексе:
```
git status
```
Создание коммита:
```
git commit -m "Какой-то комментарий"
```
### 9. Откат коммита ([см. рис. 11](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/11.png))
```
git reset --hard HEAD~
```
### 10. Создание ветки для отчёта и переход в неё ([см. рис. 12](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/12.png))
```
git checkout -b otchet
```
### 11. Оформление отчёта в файле README.md ([см. рис. 13](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/13.png))
### 12. Получение истории  операций в форматированном виде ([см. рис. 14](https://github.com/SlavaSovan/LR6/blob/otchet/screenshots/14.png))
```
git log --pretty=format:'%h - %cd, %an : %s' --date=format:'%F %R'
```
___
## Выводы
В ходе данной лабораторной работы были изучены
базовые возможности системы управления версиями,
получен опыт работы с Git Api, опыт работы с локальным
и удаленным репозиторием.
