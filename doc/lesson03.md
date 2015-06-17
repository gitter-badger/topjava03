# Занятие 3 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>
*Домашнее задание желательно прислать до вечера четверга (25.06).*

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfllmQWR2cE90UGp5RERHaE95cnVDNmZTRFJCejVhM191NDZlREwzeDdXdmc">Материалы урока</a>
- **<a href="">1 HW2.patch</a>**


##  Тестирование. Spring Test
-  Перенос mock реализации в test.
-  Тестирование через JUnit.
-  Интеграция Spring и JUnit.
-  Ресурсы:
   -  <a href="http://junit.org/">JUnit 4</a>
   -  <a href="http://habrahabr.ru/post/120101/">Тестирование в Java. JUnit</a>

##  Базы данных. Spring JDBC
-  <a href="http://alexander.holbreich.org/2013/03/nosql-or-rdbms/">NoSQL or RDBMS.</a><a
                href="http://habrahabr.ru/post/77909/">Обзор NoSQL систем</a>. <a href="http://blog.nahurst.com/visual-guide-to-nosql-systems">CAP</a>
        
-  Обзор Java persistence solution без ORM: <a
                href="http://commons.apache.org/proper/commons-dbutils/">commons-dbutils</a>,
            <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/jdbc.html">Spring
                JdbcTemplate</a>, <a href="http://en.wikipedia.org/wiki/MyBatis">MyBatis</a>, <a href="http://www.jdbi.org/">JDBI</a>
-  <a href="http://habrahabr.ru/company/JetBrains/blog/204064/">Настройка Database в IDEA</a> и запуск SQL.
-  Скрипты инициализация базы
-  Подключение Spring Jdbc.
-  Конфигурирование DataSource. property-placeholder.
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/jdbc.html#jdbc-initializing-datasource-xml">Инициализация
            базы при старте приложения</a>
-  JdbcTemplate. Имплементация JdbcUserRepository
-  Подготовка тестовых данных для UserServiceTest. Добавление TestUser и ModelMatcher
-  Тестирование UserService. Конфигурирование логирования в тестах.
-  Инициализация базы из java. ScriptUtil -> ResourceDatabasePopulator.
            <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#resources">Абстракция
                Resource</a>
-  Починка mock: подмена контекста при тестировании

## Домашнее задание HW03
     * Дополнить скрипты создания и инициализации базы

       src\main\resources\db\initDB.sql
       src\main\resources\db\populateDB.sql 
     
       таблицой MEALS.
     
     * Реализовать через Spring JDBC Template JdbcUserMealRepositoryImpl
     
     * Сделать тестовые данные MealTestData, АНОЛОГИЧНЫЕ пропопулированным в таблице 
     
     * Используя spring-test протестировать сервис UserMealService (UserMealServiceTest)  
       (из UserMealServiceImpl нажать Ctrl+Shift+T и выбрать JUnit4)
     
     Все задания делаются по аналогии с уже имеющейся реализацией для User.

-  <a href="https://vk.com/topic-88584431_31508716">Обсуждение ДЗ в группе VK</a>
