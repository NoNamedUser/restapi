1. Подключена зависимость flyway.  
2. Создан файл flyway.properties в директории resources/db/migration.  
3. Создан скрипт инициализации базы данных. В нем создается таблица products и при  
    каждом новом запуске приложениея осуществляется проверка ее существования,  
    как это указано в application.properties(spring.jpa.hibernate.ddl-auto=validate).  
4. Созданы 2 sql-скрипта для проверки работоспособности миграций:  
    а) Добавление колонки в таблицу продуктов.  
    б) Удаление добавленной колонки из таблицы.