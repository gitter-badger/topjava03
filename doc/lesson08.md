# Занятие 8 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfkpMd2UyWjBsc2JsSE4tRDFkU3BvMktFQkhUN1J6VExxSUUzOHlSR0RhNm8">Материалы урока</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVUFIeHVZdHNRUU0">Вступление. HW7.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWDRoLWYxVGEzZDQ">1 HW7.patch</a>**


##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZ2lmZjRsdFdIYlE">WebJars. Dandelion bundles</a>
>  Проект http://dandelion.github.io/components/core/ мигрировал на версию 1.xx, которая несовместима с 0.10.1
>  При этом документацию к старой версии удалили. Поэтому в будующем планирую или мигрировать на новую версию Dandelion,
>  или, лучший вариант, мигрировать на angular.js.      

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFdk1VaGR0SlVEYXM">2 webjars dandelion bundles.patch</a>**

-  Подключение веб ресурсов. <a href="http://www.webjars.org/">WebJars</a>.
-  Подключаем <a href="http://dandelion.github.io">Dandelion</a>.

##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFalh3bjhwZjJnZDg">Bootstrap. Datatables.</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFcF9LbnItaTJvM0k">3 bootstrap datatables.patch</a>**

-  <a href="http://getbootstrap.com/getting-started/">Подключаем Bootstrap</a>. Форматируем JSP.
-  <a href="http://www.tutorialrepublic.com/twitter-bootstrap-tutorial/">Twitter Bootstrap Tutorial</a>
-  <a href="http://www.w3schools.com/bootstrap/">Bootstrap 3 Tutorial</a>
-  <a href="http://bootstrap-ru.com/203/javascript.php">Javascript плагины для Bootstrap</a>
-  Создание таблиц на основе проекта Dandelion-Datatables. Форматирование.

##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFX0VoMU9JYW5zN0E">AJAX. jQuery. Notifications.</a>
>  Правка к видео: WEB-INF/jsp/userList.jsp:52 (пропущен атрибут name="item_id"). 
>  form.serialize() сериализует по name.  

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFbDhfdURJbDBQV28">4 ajax jquery.patch</a>**

-  <a href="https://ru.wikipedia.org/wiki/AJAX">AJAX</a>. <a href="https://ru.wikipedia.org/wiki/JQuery">jQuery</a>
-  Событие $(document).ready. Запросы ajax. Обратный вызов (Callback).
-  Редактирование таблицы на основе <a href="http://getbootstrap.com/javascript/#modals">модального окна Bootstrap</a>. 
-  Реализация удаления/добавления пользователей.
-  Ресурсы:
    -  <a href="http://anton.shevchuk.name/jquery/">jQuery для всех</a>.
    -  <a href="http://anton.shevchuk.name/javascript/jquery-for-beginners-ajax/">jQuery для начинающих. AJAX</a>.
    -  <a href="http://anton.shevchuk.name/javascript/jquery-for-beginners-selectors/">jQuery для начинающих. Селекторы</a>.
    -  <a href="http://api.jquery.com/">jQuery API</a>
    -  <a href="http://getbootstrap.com/javascript/">Bootstrap JavaScript</a>
    -  <a href="http://legacy.datatables.net/ref">DataTables 1.9.4 API</a>

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFSkhldmMxSUtJdnc">5 notification.patch</a>**
-  Обработка ajaxError. <a href="http://ned.im/noty/">jQuery notification</a>

##  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFRVkzcFMwc0hrYmM">Добавление Spring Security</a>  
>  Правка к видео: путь в intercept-url должен быть полный - pattern="/rest/admin/**"

>  В Spring Security 4.x по умолчанию включен csrf. Будем его проходить на 10м занятии.  

-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZTlOTXAyX2ZCSEU">6 add security.patch</a>**

-  <a href="http://projects.spring.io/spring-security/">Spring Security</a>

-  <a href="https://ru.wikipedia.org/wiki/Протокол_AAA">Протокол AAA</a>
-  <a href="https://ru.wikipedia.org/wiki/Аутентификация_в_Интернете">Методы аутентификации</a>.
-  <a href="https://en.wikipedia.org/wiki/Basic_access_authentication">Basic access authentication</a>

-  <a href="http://articles.javatalks.ru/articles/17">Использование ThreadLocal</a>

-  Добавляем в проект spring-security и security filter
-  Конфигурируем security context для ресурсов и REST
-  Тестируем Security REST через SoapUI

## Домашнее задание HW08
    Перевести mealList на dandelion (mealList.jsp, UserMealAjaxController, локализация)
    Реализовать удаление/добавление записи еды.

Optional.

    Реализовать enable/disable User через checkbox в userList.jsp (достаточно реализовать только в DataJpa)
    
-  <a href="https://vk.com/topic-88584431_31711302">Обсуждение ДЗ в группе VK</a>
