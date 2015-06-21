# Занятие 3 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>
*Домашнее задание желательно прислать до вечера четверга (25.06).*

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfllmQWR2cE90UGp5RERHaE95cnVDNmZTRFJCejVhM191NDZlREwzeDdXdmc">Материалы урока</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWTdkTEhBNGQxRDA">HW2: делаем API UserMeal</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbHZaNnB6X05GbG8">1 HW2.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFOU8wWlpPVE05STA">Коротко о жизненном цикле Spring контекста.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFcUxNWEFNT0tDTWM">2 PostConstruct PreDestroy.patch</a>**
-  <a href="http://habrahabr.ru/post/222579/">Spring изнутри. Этапы инициализации контекста.</a>
-  Ресурсы:
   -  <a href="http://vk.com/javawebinar?z=video-58538268_169373158%2Fvideos-58538268">Евгений Борисов. Spring, часть 1</a>
   -  <a href="http://vk.com/javawebinar?z=video-58538268_169373162%2Fvideos-58538268">Евгений Борисов. Spring, часть 2</a>
   -  <a href="http://www.slideshare.net/taemonz/spring-framework-core-23721778">Презентация Spring framework core</a>

##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFODlkU1B0QnNnSGs">Тестирование через JUnit.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFanBONjJPMzVkZzA">3 Add Junit.patch</a>**
-  Перенос mock реализации в test.
-  <a href="http://junit.org/">JUnit 4</a>
-  <a href="http://habrahabr.ru/post/120101/">Тестирование в Java. JUnit</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFai1veG9qaFZlZ2s">Spring Test</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZ0h1UnB5YXVZUDQ">4 Add spring test.patch</a>**
-  Интеграция Spring и JUnit.
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#testing">Spring Testing</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVlNYczhnSU9JdXc">Базы данных. Обзор NoSQL и Java persistence solution без ORM.</a>
-  <a href="https://ru.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a>.
-  <a href="http://alexander.holbreich.org/2013/03/nosql-or-rdbms/">NoSQL or RDBMS.</a><a
                href="http://habrahabr.ru/post/77909/">Обзор NoSQL систем</a>. <a href="http://blog.nahurst.com/visual-guide-to-nosql-systems">CAP</a>
-  Обзор Java persistence solution без ORM: <a
                href="http://commons.apache.org/proper/commons-dbutils/">commons-dbutils</a>,
            <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/jdbc.html">Spring
                JdbcTemplate</a>, <a href="http://en.wikipedia.org/wiki/MyBatis">MyBatis</a>, <a href="http://www.jdbi.org/">JDBI</a>
- Ресурсы:
  - <a href="https://ru.wikipedia.org/wiki/Реляционная_СУБД">Реляционная СУБД</a>
  - <a href="http://habrahabr.ru/post/103021/">Реляционные базы</a>
  - <a href="http://ru.wikipedia.org/wiki/Java_Database_Connectivity">JDBC</a>.
                
## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQWtHYU1qTDlMWVE">Настройка Database в IDEA.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZnJKampTSFJmMGM">6 Add db props.patch</a>**
-  <a href="http://habrahabr.ru/company/JetBrains/blog/204064/">Настройка Database в IDEA</a> и запуск SQL.

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFMGNWUXhaVzdlU0k">Инициализация базы. Имплементация UserRepository через Spring Jdbc Template.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZ185clpYTm94eG8">7 populate and init db.patch</a>**
-  Скрипты инициализация базы

- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQkotMXZOLUY4QTQ">8 impl JdbcUserRepository.patch</a>**
-  Подключение <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/jdbc.html">Spring Jdbc</a>.
-  Конфигурирование DataSource. <a href="http://www.mkyong.com/spring/spring-propertyplaceholderconfigurer-example/">property-placeholder</a>.
-  Имплементация UserRepository через Spring Jdbc Template.

## <a href="">Подготовка тестовых данных и тестирование UserService.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZ185clpYTm94eG8">9 test UserService.patch</a>**
-  Подготовка тестовых данных в UserServiceTest. Добавление TestUser и ModelMatcher
-  Тестирование UserService.
-  Ресурсы:
   - <a href="http://www.youtube.com/watch?v=YzOTZTt-PR0">Николай Алименков — Босиком по граблям Hibernate</a>
   
## Домашнее задание HW03
     * Дополнить скрипты создания и инициализации базы

       src\main\resources\db\initDB.sql
       src\main\resources\db\populateDB.sql 
     
       таблицой MEALS.

     * Реализовать через Spring JDBC Template JdbcUserMealRepositoryImpl (сделать каждый метод за один SQL запрос)
       Т.к postgres драйвер не понимает LocalDateTime, использовать преобразования: 
                                                       Timestamp.valueOf(ldt) / timestamp.toLocalDateTime()
     
     * Сделать тестовые данные MealTestData, АНОЛОГИЧНЫЕ пропопулированным в populateDB.sql. 
       Тестовый класс-обертка к UserMeal не требуется, сравниваем данные через MATCHER (toString)

     
     * Запустить скрипт инициализации initDB.sql на базу и протестировать сервис UserMealService.  
       UserMealServiceTest создать из UserMealService (Ctrl+Shift+T и выбрать JUnit4) и реализовать тесты.
     
-  <a href="https://vk.com/topic-88584431_31508716">Обсуждение ДЗ в группе VK</a>
