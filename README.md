## Общая информация
**Курс**: 2  
**Семестр**: 2(4)  
**Учебный год**: 2019-2020  
**Дисциплина**: Системы управления версиями  
**Тема**: Личный кабинет сотрудника фитнес-клуба. Тренеры, тренировки, клиенты, программы тренировок, абонементы. Интеграция с 1С:Фитнес.  
**Группа**: МОСм-181  
**Студент**: Серов Андрей  

## Объекты системы
- Тренер
- Клиент
- Тренировка
- Отработанные тренировки
- Абонемент

## Сценарии
- Регистрация тренера
- Вход тренера
- Личный кабинет:
  - Изменение личных данных
  - Просмотр плановых тренировок (тренировки, которые тренер обязан провести)
  - Просмотр отработанных тренировок
- Просмотр всех тренеров
- Добавление клиентов
- Просмотр всех клиентов
- Изменение данных о клиенте
- Удаление клиента
- Создание тренировки
- Создание абонементов
- Просмотр тренировок и клиетов имеющие абонемент на данную тренировку
- Изменение данных тренировки
- Изменение данных абонемента
- Удаление тренировки
- Удаление абонемента
- Создание проведенных тренировок
- Просмотр всех проведенных тренировок и присутствующих клиентов на данных тренировка 


# Схема БД
![image](/database_schema.png)

# Спринт
Недельный спринт с 30.03 до 03.04. 

Задачи:
- Проетирвование базы данных
- Реализация базы данных
- Реализация регистрации пользователя(тренера):
  - Форма регистрации на frontend'e
  - Логика регистрации на backend'e
- Реализация авторизации пользователя(тренера):
  - Форма авторизации на frontend'e
  - Логика авторизации на backend'e
- Страница списка клиентов:
  - Реализовать форму создания клиента на frontend'e с возможностью повторного переиспользования в форме изменения клиента в дальнейшем
  - Реализовать запрос на создание клиента
  - Реализовать запрос на получение списка клиентов
  - Реализовать таблицу отображения списка клиентов
  - Реализовать компонент изменения данных клиента
  - Реализовать запрос на удаление клиента
- Страница списка трениров:
  - Реализовать запрос на получение списка трениров
  - Реализовать таблицу отображения трениров
  - Реализовать форму создания тренировки на frontend'e с возможностью повторного переиспользования в форме изменения тренировки в дальнейшем
  - Реализовать запрос на создание тренировки
  - Реализовать запрос на получение списка тренировок c их клиентами
  - Реализовать таблицу отображения списка тренировок c их клиентами
  - Реализовать компонент изменения данных тренировки
  - Реализовать запрос на удаление тренировок
- Страница отработанных тренировок
  - Реализовать форму создания отработанной тренировки
  - Реализовать запрос на создание отработанной тренировки
  - Реализовать запрос на получение отработанных тренировов
  - Реализовать таблицу отображения списка отработанных тренировок
  - Реализовать запрос на удаление отработанной тренировки
- Личный кабинет
  - Реализовать форму отображения личных данных и возможностью их изменять
  - Реализовать запрос на получение личных данных
  - Реализовать запрос на изменение личных данных
  - Реализовать список отображения прикрепленных тренировок
  - Реализовать список отображения отработанных тренировок


  
# Запуск
### Запуск backend
```
pipenv install
pipenv shell
cd backend/
python manage.py migrate
python manage.py runserver
```

### Запуск frontend
```
cd frontend/
npm install
npm run dev
```

### Переходим на страницу http://localhost:3000/
