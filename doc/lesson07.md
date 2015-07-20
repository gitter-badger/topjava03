# Занятие 7 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfjVnUVhINEg0d09Nb3JsY2ZZZmpsSWp3bzdHMkpKMmtPTlpjckxyVzg0SWc">Материалы урока</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFc2dFeU1KbmZ1Ym8">Tomcat pool. Auto generate DDL.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTWozUGdPRUE0MEU">1 generate ddl.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFX1V5VHBOSVc2b3c">HW6</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbWlCRFlLcE5zLUE">2 HW6.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQXhBN1pqa3FyOUE">Тестирование Spring MVC</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeGdPZlJEZS1kMmM">3 controller test.patch</a>**

-  <a href="http://hamcrest.org/JavaHamcrest/">Hamcrest</a>
-  <a href="http://www.petrikainulainen.net/programming/spring-framework/unit-testing-of-spring-mvc-controllers-normal-controllers/">Unit Testing of Spring MVC Controllers</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWE5oSmJFZGZBRlE">REST контроллеры</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVGJ1MkhnNFlrUDg">4 rest controller.patch</a>**
  (переименовал AdminUserRestController -> AdminRestController и UserRestController -> ProfileRestController)

-  <a href="https://ru.wikipedia.org/wiki/JSON">JSON (JavaScript Object Notation</a>
-  <a href="https://spring.io/understanding/rest">Understanding REST</a>
-  <a href="http://www.infoq.com/articles/springmvc_jsx-rs">JAX-RS vs Spring MVC</a>
-  <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-ann-requestmapping">Request mapping</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFQmNwOXJ6RFk4M1U">Тестирование REST контроллеров. Добавление Jackson.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbktibjY3bHZUUmc">5 rest test jackson.patch</a>**

-  https://github.com/FasterXML/jackson-databind

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNWEyVGJIU2JMTFE">jackson-datatype-hibernate. Тестирование через матчеры.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFR2JwcTJ4STdRSE0">6 jackson hibernate.patch</a>**
-  Сериализации hibernate lazy-loading с помощью <a href="https://github.com/FasterXML/jackson-datatype-hibernate">jackson-datatype-hibernate</a>

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZ2p1Q0xISzVIbTg">7 test with matcher</a>**
-  <a href="http://habrahabr.ru/post/259055/">Тестируем Spring Rest контроллеры</a>, Проверка JSON-содержимого ответа через собственный ResultMatcher

        <li>Настройка сериализации JSON. Тестирование через <a href="http://www.soapui.org/">SoapUi</a>.</li>
        <li>Решение проблемы с UTF-8 в StringHttpMessageConverter</li>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVXNmOUdBbUxxWVU">Тестирование через SoapUi. UTF-8</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFX1VjVVdITVV2YXc">8 soapui utf_8 converter.patch</a>**

-  <a href="http://www.soapui.org/">SoapUi</a>, открыть проект config\Topjava-soapui-project.xml 
-  Проверка UTF-8: http://localhost:8080/topjava/rest/profile/text
-  <a href="http://forum.spring.io/forum/spring-projects/web/74209-responsebody-and-utf-8">ResponseBody and UTF-8</a>

## Домашнее задание HW06
    Сделать тест для UserMealController
    Добавить ResourceControllerTest на получение style.css

    Реализовать AbstractUserMealController / UserMealRestController
    LocalDateTime передавать даты в формате ISO_LOCAL_DATE_TIME (например '2011-12-03T10:15:30'), java.time.format.DateTimeFormatter#ISO_DATE_TIME
    Для преобразования в LocalDateTime можно 
        1. принимать в параметрах String и конвертить самому, используя ru.javawebinar.topjava.util.TimeUtil
                      
        2. правильнее: написать StringToLocalDateTimeConverter конвертор, см. пример:
        http://docs.spring.io/spring/docs/current/spring-framework-reference/html/validation.html#core-convert-Spring-config 
    
    
    Загрузить проект soap-ui проект (\config\Topjava-soapui-project.xml) и протестировать UserMealRestController 

    Сделать тесты UserMealRestControllerTest

-  <a href="https://vk.com/topic-88584431_31673314">Обсуждение ДЗ в группе VK</a>
