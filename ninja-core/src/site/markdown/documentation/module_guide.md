Ninja modules are classic Maven modules that are then registred in a web application in the `Module.java` class.

```java
@Singleton
public class Module extends AbstractModule {

    protected void configure() {

        install(new MyModule());
        ...    
    }
    
}
```

How to build 
============
  - `mvn eclipse:eclipse` will generate an Eclipse project from the `pom.xml`
  - `mvn package` will build the module and run the tests 

How to publish
==============
 - `mvn install` will install the module locally so you can test it in your application. You will be able to reference your new module in your application dependencies 
 - `mvn deploy` will publish the module to a centralized online repository
