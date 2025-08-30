# SpringBoot-Notes
Welcome to my Spring & Spring Boot learning repository! This repository contains all my personal notes and code snippets as I continue learning and exploring Spring Framework and Spring Boot for building robust, scalable Java-based backend applications.
#Table of Contents
- Project Setup
- Spring Framework
    - Dependency Injection (DI)
    - IoC Container
    - Bean Configuration (XML)
    - Injection Types
    - Autowiring
    - Tight vs Loose Coupling
    - Stereotype Annotations
- Spring Boot
    - Spring Boot Annotations
    - API Layers
    - Dependency Injection in Boot
    - Working with REST APIs
- Sample XML Config
- More Concepts

#Project Setup
- Create a new project using IntelliJ IDEA.
- Add dependencies from Maven Repository, e.g., spring-context, into the pom.xml.
- Create an xml config file in src/main/resources.
- Load configuration in code:
      ApplicationContext context = new ClassPathXmlApplicationContext("config.xml");
#Spring Core
- IoC (Inversion of Control): Spring manages object creation (DI).
- Bean Config (XML):
        <beans>
          <bean id="student" class="org.example.Student">
            <property name="age" value="20"/>
            <property name="pan" ref="pen"/>
          </bean>
          <bean id="pen" class="org.example.Pan"/>
        </beans>
- Dependency Injection Types: Setter, Constructor, Field
- Autowiring: byName, byType, @Primary, @Qualifier
- Loose vs Tight Coupling: Interfaces reduce dependency

#Annotations
- @Component, @Autowired, @Value, @Qualifier
- @ComponentScan("org.example")
- @Bean, @Configuration for Java-based config

#Spring Boot
- Convention over configuration, embedded server
- Layers: Controller → Service → Repository
- Annotations: @RestController, @Service, @Repository
- API: @GetMapping, @PostMapping, etc.
- JSON auto-conversion via Jackson
- Input: @RequestBody, @PathVariable
  
->SERVLET
->Bean Scopes
->Exception Handling in Spring Boot
->Spring Boot Profiles
# Notes
- Bean scopes: singleton (default), prototype
- Use start.spring.io to bootstrap Spring Boot apps

 contact me-
Nivash 
- linkedin-linkedin.com/in/nivash-m-2k4  
- nivashmareesh07@gmail.com



