# Вкратце о системе #

djet project - это система для управления базы данных djet, построенная вокруг имеющейся на момент начала 2015 года базы Mysql. База включает около 80 таблиц для каждой из которых сделан интерфейс для изменения / добавления / удаления записей.

Фронтенд проекта построен на react-js и вцелом одинаков для каждой из таблиц.

Изначально все таблицы были разбиты на несколько групп(категорий), я решил сохранить эту группировку в меню и в структуре приложений, поэтому таблицы для каждой группы используют свой контроллер. 

Внутри каждого контроллера create / delete / update методы идентичны.
Вместо index метода используется свой для каждой таблицы который соответствует ее названию в мн.ч.  

## Установка ##

1. склонировать проект
2. произвести bundle install
3. установить node (brew install npm)
4. установить зависимости js - npm isntall
5. установить bowerлокально - npm install bower -g
6. mkdir vendor/assets/js (вынести в git)
7. установить зависимости от bower (потом уберем) rake bower:install