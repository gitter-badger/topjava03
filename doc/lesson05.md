# Занятие 5 онлайн проекта <a href="http://javawebinar.ru/topjava/">Topjava</a>
*Домашнее задание желательно прислать до вечера четверга (09.07).*

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfmctT3oyNW1qaVhDb2p0bGpyTFVlaUJ2VVpOdVgtWF9KTUFBMWFaR2xVYVE">Материалы урока</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFVFVVUGctMUxxSkE">Разбор вопросов</a>

-  <a href="http://stackoverflow.com/questions/9887242/using-postgresql-why-doesnt-hibernate-jpa-create-cascade-constraints/9925761#9925761">Hibernate/JPA cascade</a>
-  <a href="http://stackoverflow.com/questions/13835980/is-there-a-way-to-pass-detached-object-to-jpa-persist-detached-entity-passed-t">Merge для Detached Entity</a>
-  <a href="http://www.youtube.com/watch?v=1KphwODu1gg">Видео: работа в ZK с OpenJPA (в чем Hibernate хуже)</a>
-  <a href="https://developer.jboss.org/wiki/OpenSessionInView">Паттерн- открытие транзакции в фильтре</a> и <a href="http://stackoverflow.com/questions/1103363/why-is-hibernate-open-session-in-view-considered-a-bad-practice">почему это bad-practice</a>
-  <a href="https://en.wikibooks.org/wiki/Java_Persistence/Identity_and_Sequencing#Sequence_Strategies">Sequence Strategies</a>
-  <a href="http://stackoverflow.com/questions/9470442/why-is-the-hibernate-default-generator-for-postgresql-sequencegenerator-not?lq=1">SequenceGenerator/IdentityGenerator in PostgreSql</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNFMyMGJCZWE4elk">HW4: JPA. @Rule</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFX3FfcHhQVXBxdXc">1 HW4.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZENCVEhDMkZiV00">Транзакции</a>
-  <a href="https://jira.spring.io/browse/DATAJPA-601">readOnly и Propagation.SUPPORTS</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNW0yVWhXcGNPU2M">Профили Maven и Spring</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFWkE1U2dFc3Vqakk">2 profiles connection pool.patch</a>**

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTWJOdHduOWtNcTA">Пулы коннектов</a>

-  Выбор реализации пула коннектов: <a href="http://jolbox.com/">BoneCP</a>, <a href="http://commons-dbcp.apache.org">Commons Database Connection Pooling</a>, <a href="https://github.com/brettwooldridge/HikariCP">HikariCP</a>
-  <a href="http://blog.trustiv.co.uk/2014/06/battle-connection-pools">Battle of the Connection Pools</a>
-  <a href="http://blog.ippon.fr/2013/03/13/improving-the-performance-of-the-spring-petclinic-sample-application-part-3-of-5">Tomcat pool</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFYVdyMFYxRUR6bWM">Spring Data JPA</a>
- **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNTloSEVtUktrT1U">3 spring data jpa.patch</a>**

-  <h3><a class="anchor" id="datajpa"></a><a href="http://projects.spring.io/spring-data-jpa/">Spring Data JPA</a></h3>
-  Замена AbstractDAO: <a href="http://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.repositories">JPA Repositories</a>
-  Разрешение зависимостей: <a href="http://howtodoinjava.com/2014/02/18/maven-bom-bill-of-materials-dependency/">Maven BOM [Bill Of Materials] Dependency</a>
-  <a href="http://habrahabr.ru/post/232381/">Делегирование. (Spring Data JPA)</a>
-  <a href="http://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.query-methods.query-creation">Query methods</a>
    
-  Ресурсы:
   -  <a href="http://jeeconf.com/archive/jeeconf-2013/materials/spring-data/">Spring Data – новый взгляд на persistence (видео с JeeConf)</a>
   -  <a href="https://github.com/spring-projects?query=spring-data">Github repositories</a></li>
   -  <a href="http://www.petrikainulainen.net/spring-data-jpa-tutorial">Spring Data JPA Tutorial</a></li>
   -  <a href="https://blog.42.nl/articles/spring-data-jpa-with-querydsl-repositories-made-easy/">Spring Data JPA with QueryDSL</a></li>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFeC1XbVNfakhZM0U">Spring кэш</a>
-  **<a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUWFrUTlsLWJEYlk">4 spring cache</a>**

-  <a href="http://habrahabr.ru/post/113945/">Кеширование в Spring Framework</a>

-  Ресурсы:
   -  <a href="http://docs.spring.io/spring-framework/docs/current/spring-framework-reference/html/cache.html">Spring cache Abstraction</a>
   -  <a href="http://habrahabr.ru/post/25140/">Распределённая система кеша ehcache</a>
   -  Починка JUnit: <a href="http://stackoverflow.com/questions/10013288/another-unnamed-cachemanager-already-exists-in-the-same-vm-ehcache-2-5">один кэш на JVM</a>

## <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZFdWWFdwams0eGM">Домашнее задание HW05</a>
     Имплементировать и протестировать DataJpaUserMealRepositoryImpl 
     Разделить реализации Repository по профилям Spring: jdbc, jpa, datajpa 
            (общее в профилях можно объединять, например <beans profile="datajpa,jpa">)
     Сделать тесты всех реализаций (jdbc, jpa, datajpa) через наследование (без дублирования),
             общее из UserMealServiceTest.java и UserServiceTest.java - также вынеси в базовый класс.
          
-  <a href="https://vk.com/topic-88584431_31592002">Обсуждение ДЗ в группе VK</a>