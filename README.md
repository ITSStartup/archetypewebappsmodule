##Maven Archetype-webapps-module 

webapps module archetype maven for creating web application with Hibernate, Spring, Jersey, DBUnit and Util Java API separated by modules  back/front-end.

###Required 

* Maven installed 

###Features 

* DAO Generic implemented; 
* Service Generic implemented; 
* Structure for DBUnit done; 
* back/front end separated in modules: webapps-core and webapps-web 
* [flyway plugin](http://flywaydb.org) setup for db migration; 


###How to Install local?

Step 1 

```java
git clone git@github.com:ITSStartup/archetypewebappsmodule.git
```

Step 2 

* Go to the folder and execute: 

```java
mvn clean install 
```

Step 3 

* create new maven project via Eclipse ;
* in Catalog choose **All Catalogs**;
* in filter type: br.

Now its is expected you see in group id: *br.com.its.archetypes*

* choose the archetype and go ahead clicking in next 

Step 4 Resolving dependency in module webapps-web

This module has dependency of **webapps-core**. The archetype has default configuration, but you must update according to your project. Check the steps:

**Steps** 

* import maven project webapps-core and webapps-web for your IDE; 
* open webapps-web/pom.xml ;
* remove webapps-core 1.0.0 of dependency (its default of archetype and it does not work for your custom structure); 
* click in add; 
* type **webapps**; 
* Choose **webapps-core** according to  **groupId** that was defined when you created the project; 

**Testing**

If you did not change any  default configuration in pom.xml of the modules, now we can test. 

1. go to parent module and execute:

```java
mvn clean install 
```

2. now starting apps

```java
mvn tomcat:run
```

3. Access http://localhost:8080/webapps-web/


**Conclusion**

webapps-module archetype is flexible to  change and to be  customatized according to your project. Feel free and improve it and send pull request.
