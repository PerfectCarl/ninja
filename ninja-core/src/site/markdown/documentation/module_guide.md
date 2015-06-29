Ninja modules are classic Maven modules that are then registred in a web application in the `Module.java` class.

```java
@Singleton
public class Module extends AbstractModule {


    protected void configure() {

        install(new Jade4NinjaModule());

        ...    

    }

}
```

How to build 
============


How to publish
==============
