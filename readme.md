Данный репозиторий будет использоваться для создание резервной копии коллекций из Postman
<br>
<br>
# Текущие JOB для резервного копирования
Сейчас действуют две job для резервного копирования.

Найти их можно следующим путем:
в Postman нажать `Home` -> `Integration`
![Интеграция](/image/01.jpg)

![Интеграция](/image/02.jpg)


Вот две джобы:
- `Backup-Other-Request` - делает резервную копию коллекции **Regression**
- `Backup-Regression-Collection` - делает резервную копию коллекции **Отдельные запросы**
![Интеграция](/image/03.jpg)

# Создание новой JOB для резервного копирования

в Postman выполнить следующие шаги:
1.  Перейти `Home` -> `Integration` -> `Backup a collection`
2.  Нажать `Add integration`
  ![Добавление интеграции](/image/04.jpg)
3. Ввести токен - хранится в конфлюен, называется `token_for_backup_postman_collection`
     ![Добавление интеграции](/image/05.jpg)
4. Нажать `Authenticate and Proceed`
5. Заполнить следующие поля:
   1. Название JOB (Оно будет отображаться в postman)
   2. Выбрать workspace в котором находится коллекция для резервного копирования
   3. Выбрать коллекцию, которую нужно добавить на GitHub
   4. Выбрать репозиторий, в нашем случае это `METIBQA/Postman_backup`
   5. Ввести название папки на GitHub, которая будет использоваться для резервного копирования, в нашем случае это `Postman Collections`
   6. Ввести название файла, который будет создан на GitHub
   7. Выбрать ветку, в которую будет выполняться резервное копирование, в нашем случае `main`
   8. Нажать `Add integration`

  ![Добавление интеграции](/image/06.jpg)