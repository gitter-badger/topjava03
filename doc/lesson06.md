# Занятие 6 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfkF5c1hiWmstT0prODdtZkVuNFlMZmdtN3J0OUcyY0lkT2NlVzlUMXRUUlk">Материалы урока</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUVZobXRzNWFzUW8">HW5: Spring Profiles. Spring Data JPA</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZFZhZGdrMnBYN00">1 HW5.patch</a>**
(ДЗ, добавил профили в SpringMain, в User добавил и закоментировал List<UserMeal> userMeals- можете раскоментировать и проверить что по get все достается,
поправил баг в JPA реализации- при merge надо возвращать результат мержа. Это сказывается только если мы работаем в транзакции с возвращенным результатом, в SimpleJpaRepository правильно)

-  <a href="http://stackoverflow.com/questions/3669883/hibernate-where-do-insertable-false-updatable-false-belong-in-composite-pr#answer-9442483">FK как примитив в Entity</a>
-  <a href="http://javarticles.com/2013/12/spring-profiles.html">Spring Profiles</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeTV0SUFfblk5NE0">Кэш Hibernate</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQXBJQ1JRRHFwR0E">2 hibernate cache.patch</a>**
   (JpaUtil не определен в профиле jdbc: тесты JdbcUserServiceTest к починке в ДЗ) 

-  <a href="http://habrahabr.ru/post/135176/">Уровни кэширования Hibernate</a>
-  <a href="http://habrahabr.ru/post/136375/">Hibernate Cache. Практика</a>
-  Починка тестов: <a href="http://stackoverflow.com/questions/1603846/hibernate-2nd-level-cache-invalidation-when-another-process-modifies-the-databas">инвалидация кэша Hibernate</a>
-  Ресурсы:
   -  Подключение <a href="http://www.ehcache.org/generated/2.9.0/html/ehc-all/#page/Ehcache_Documentation_Set%2Fco-hib_about_using_ehcache_with_hibernate.html%23wwconnect_header">кэша Hibernate 2-го уровня</a>
   -  <a href="http://stackoverflow.com/questions/3663979/how-to-use-jpa2s-cacheable-instead-of-hibernates-cache">JPA2 @Cacheable vs Hibernate @Cache</a>
   -  <a href="http://habrahabr.ru/post/25140/">Распределённая система кеша ehcache</a>
   -  <a href="http://docs.jboss.org/hibernate/orm/4.3/manual/en-US/html_single/#performance-cache-mapping">Cache mappings</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVE1jWkRucm1UTjA">Spring Web</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZlNmSkplTy1KWUk">3 spring web init.patch</a>**

-  Добавляем в проект веб зависимости
-  Поднятие контекста Spring в веб приложении. <a href="http://www.mkyong.com/servlet/what-is-listener-servletcontextlistener-example/">ServletContextListener</a>. Задание дефолтного профиля.
-  Получение контекста Spring в веб-контейнере
-  Имплементируем UserController. <a href="http://design-pattern.ru/patterns/mvc.html">Паттерн MVC</a>
-  Ресурсы:
   -  <a href="https://docs.oracle.com/javaee/6/tutorial/doc/bnafi.html">Servlet Lifecycle</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFN3k0ZVk1MnF5TjQ">JPS, JSTL, internationalization</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFejFZWjhER0diTk0">4 jsp jstl i18n.patch</a>**

-  <a href="http://devcolibri.com/1250">JSTL для написания JSP страниц</a>


## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTnRoeUlOWXpSMWs">Динамическое изменение профиля при запуске. Конфигурирование Tomcat через maven plugin и jndi</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFM3M1Skt0T3BsWUU">5 tomcat pool jndi.patch</a>**

-  Динамическое изменение профиля Spring при запуске (-Dspring.profiles.active="datajpa,postgres")
-  Конфигурирование пула коннектов в Tomcat и jndi-lookup.

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQThUX2VyQXNiTHM">Spring Web MVC</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQ1V6aHRUWlFwWGM">6 spring webmvc.patch</a>**

-  <a class="anchor" id="mvc"></a><a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html">Spring Web MVC</a>
-  <a href="http://design-pattern.ru/patterns/front-controller.html">Паттерн Front Controller</a>
-  Добавляем DispatcherServlet и MVC application context. <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/images/mvc-contexts.gif">Иерархия контекстов в Spring Web MVC</a>
-  <a href="http://www.tutorialspoint.com/spring/spring_web_mvc_framework.htm">Сценарий обработки запроса</a>. <a href="http://www.studytrails.com/frameworks/spring/spring-mvc.jsp">HandlerMappings</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-viewresolver-resolver">View resolving</a>: прячем jsp под WEB-INF.
-  HandlerMapping: <a href="http://www.mkyong.com/spring-mvc/spring-mvc-simpleurlhandlermapping-example/">SimpleUrlHandlerMapping</a>, <a href="http://www.mkyong.com/spring-mvc/spring-mvc-beannameurlhandlermapping-example/">BeanNameUrlHandlerMapping</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-config-static-resources">Маппинг ресурсов.</a>
-  Ресурсы:
   -  <a href="http://www.jpalace.org/document/34/spring-mvc-tutorial">Spring MVC Tutorial</a>
   -  <a href="http://devcolibri.com/120">Spring MVC — Hello world</a>
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html">Web MVC framework</a>
   -  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-webappctx-special-beans-tbl">Special bean types in the WebApplicationContext</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUEctTkRSMWNvRjg">Spring Internationalization</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFaXRrSnBpejJDd0E">7 spring i18n.patch</a>**

-  <a href="http://simplespringtutorial.com/i18n.html">Spring Internationalization or i18n</a>
-  <a href="http://learningviacode.blogspot.ru/2012/07/reloadable-messagesources.html">Reloadable MessageSources</a>
-  <a href="http://nginx.com/resources/admin-guide/serving-static-content/">nginx: Serving Static Content</a>

## Домашнее задание HW06
    Починить тесты Jdbc (разделить тесты для jdbc и jpa/datajpa)
    Починить mock тесты
    Имплементировать UserMealController с выводом таблицы meals в mealList.jsp

Optional

    Дату-время вывести в формате yyyy-MM-dd HH:mm
          
-  <a href="https://vk.com/topic-88584431_31644662">Обсуждение ДЗ в группе VK</a>
