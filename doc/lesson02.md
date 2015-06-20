# Занятие 2 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>
*Домашнее задание желательно прислать до вечера четверга (18.06).*

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfkpsWE1uX19zV19IVHd0bTlDclc5QmhMMm4xa0Npek9DT18tdkwyLTBZdXM">Материалы урока</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZXVmYWxDOGFhc1E&authuser=0">1 HW1.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUWtsVGE0SDhzc2M">Разбор вопросов: работа с git, зависимости логгирования, jmx</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVDJZVTktQzRYTWc">Библиотека vs Фреймворк. Стандартные библиотеки Apache Commons, Guava</a>
-  <a href="http://commons.apache.org/">Apache Commons</a>, <a href="https://code.google.com/p/guava-libraries/wiki/GuavaExplained">Guava</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSFR1cDBIamIzQjA">Слои приложения. Создание каркаса приложения.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFV2RpMko2WnNvM0E">2 App layers.patch</a>**

-  <a href="https://www.genuitec.com/products/myeclipse/learning-center/spring/myeclipse-for-spring-reference-blueprints/">Архитектурные
            слои приложения в Spring</a>
-  <a href="https://ru.wikipedia.org/wiki/Инверсия_управления">Инверсия управления.</a><a href="http://image.slidesharecdn.com/springintroduction-130729220359-phpapp01/95/spring-introduction-3-638.jpg?cb=1375162442">DI/
            Service Locator</a>
-  <a href="http://habrahabr.ru/post/131993/">IoC, DI, IoC-контейнер — Просто о простом</a>   
-  Доменная модель приложения
-  <a href="http://martinfowler.com/eaaCatalog/dataTransferObject.html">Паттерн DTO</a>. <a href="http://stackoverflow.com/questions/1612334/difference-between-dto-vo-pojo-javabeans">Value Object и Data Transfer Object</a>
-  <a href="http://codehelper.ru/questions/205/new/repository-и-dao-отличия-преимущества-недостатки">Паттерны Repository и DAO</a>
-  Разбиение на пакеты по слоям и бизнес логике. Создание каркаса приложения.
-  <a href="http://en.wikipedia.org/wiki/Multilayered_architecture">Паттерн "Слои приложения"</a>

##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWXA1b0pnMGlvU0U">Обзор  Spring Framework. Spring Context.</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFRWNEMGVodTlfb2c">3 Add spring dependency.patch</a>**
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZmd5MkdoX0taeFE">4 Add spring context and main.patch</a>**
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFd09CWVhtQ2hZSUU">5 Add dependency injection.patch</a>**
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFcWh2TDVsLTRDTk0">6 Add annotation processing.patch</a>**

-  <a href="http://en.wikipedia.org/wiki/Spring_Framework">Spring Framework</a>
-  <a href="http://spring.io/projects">Проекты Spring</a>.
-  <a href=http://docs.spring.io/spring/docs/current/spring-framework-reference/html/overview.html>Обзор Spring Framework</a>
-  Ресурсы:
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/beans.html">Introduction to the Spring IoC container
       and beans</a>
   -  <a href="http://springindepth.com/book/in-depth-ioc-constructor-setter-injection.html">Constructor & Setter Injection</a>
   -  <a href="http://stackoverflow.com/questions/6827752/whats-the-difference-between-component-repository-service-annotations-in">Difference
       between @Component, @Repository & @Service annotations in Spring</a>
   -  <a href="http://www.mkyong.com/spring/spring-auto-scanning-components/">Spring Auto Scanning Components</a>
   -  <a href="https://spring.io/guides">Getting Started</a>
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/">Spring Framework Reference Documentation</a>
   -  <a href="https://github.com/spring-projects">Spring на GitHub</a>
  
## Домашнее задание HW02
    Сделать API и реализацию для классов UserMeal (с учетом того, что будем сохранять в базе)
       - Учесть, что еда принадлежит какому-то из пользователей.
       - Нельзя позволять модифицировать/смотреть чужую еду (бросать NotFoundException)
       - id авторизованного пользователя брать как LoggedUser.id().
       - Вместо реального сохранения/модификаций сделать заглушку MockUserMealRepositoryImpl
       
    Включить в контекст Spring и протестировать через SpringMain классы, относящиеся к UserMeal
    
    Optional (LoggedUser дополнится   public static int getCaloriesPerDay() {return 2000;}): 
       - Добавить в REST API методы для реализации функционала нашего приложения (c фильтрацией и UserMealWithExceed)
       - Перенести вызов и вывод отфильтрованных UserMealWithExceed из UserMealsUtil в SpringMain

-  <a href="https://vk.com/topic-88584431_31486787">Комментарии к ДЗ в группе VK</a>

    - В UserMealRestController в sava/update UserMeal приходят без User/userId
      Приложение может прислать все что угодно. Юзер может управлять ТОЛЬКО СВОЕЙ едой, поэтому он определяется на основании        прошедшего авторизацию LoggedUser.id()
    - При реализации UserMealServiceImpl постараться сделать в каждом методе только одни запрос к UserMealRepository 
    - Метод UserMealsUtil.main удалить: код перенести в SpringMain и MockUserMealRepositoryImpl
    - Т.к в model находятся только entity, хранимые в DB, UserMealWithExceed перенести в новый пакет to (transfer object)
    - В репозитори также делаем метод фильтрации.
    - UserMealWithExceeded используется только для отрисовки таблицы. 
      Возвращаем List<UserMealWithExceed> только для UserMealRestController.getAll и UserMealRestController.getBetween
