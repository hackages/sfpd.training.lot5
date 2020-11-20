# CDI (Contexts and Dependency Injection) Features

## Workshop 

### CDI Bean from an Interface 

* In your module `day4/arquillian-tutorial` 
    1. Let's refactor the code, create a interface `MyGreeterService` with a method 
    > String createGreeting(String name);
    1. Make the class `Greeter` implement the created interface
    1. Rename `Greeter` to  `MyDefaultGreeterServiceImpl` 
    1. In the test class, do not include `MyDefaultGreeterServiceImpl` in your JAR (via ShrinkWrap)
    1. Instead add `MyGreeterService` 
    1. Run the test successfully
    1. In the test class, add the field 
    > @Inject BeanManager beanManager;
    1. Create a test method to confirm the Beans present in CDI Context
    > beanManager.getBeans(MyGreeterService.class);

* In your module `day4/arquillian-persistence-tutorial` 
    1. Create a new test for our business services (interfaces) such as `ProductService`,  `CustomerService`,  `OrderService`  
    1. Let's refactor the code in the same fashion as the previous block 
    1. Run the test successfully 
    
### Self paced Experiments with CDI Features 

https://docs.oracle.com/javaee/6/tutorial/doc/gjehi.html 

## Online Resources

* [JEE8 Samples](https://github.com/javaee-samples/javaee8-samples)

* [What's better](https://dzone.com/articles/spring-boot-or-jakarta-ee-whats-better) 