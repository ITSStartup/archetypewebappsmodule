##Maven Archetype-webapps-module 

webapps module archetype maven for creating web application with Hibernate, Spring,Spring Security, Jersey, DBUnit and Util Java API separated by modules  back/front-end.

###Required 

* Maven installed 

###Features 

* DAO Generic implemented; 
* Service Generic implemented; 
* Structure for DBUnit done; 
* back/front end separated in modules: webapps-core and webapps-web 
* flyway plugin setup for db migration; 


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
