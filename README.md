# Spring-Boot

# Spring Boot Basics 🚀

This repository is designed for beginners to understand the **fundamentals of Spring Boot**.  
It covers simple examples, annotations, dependencies, and how to run a Spring Boot application.    
 
--- 
 
## 📌 What is Spring Boot? 
Spring Boot is a Java-based framework used to create stand-alone, production-ready Spring applications with minimal configuration.  
It simplifies the development process by providing embedded servers (like Tomcat), auto-configuration, and starter dependencies.

---

## 📂 Project Structure
spring-boot-basics/
│-- src/
│ └── main/
│ └── java/com/example/demo/
│ └── HelloController.java
│-- pom.xml
│-- README.md


---

## ⚙️ Dependencies
The main dependencies used in this project:
- **spring-boot-starter-web** → To build web applications (REST APIs).
- **spring-boot-starter-test** → For unit testing.
- **spring-boot-devtools** → For auto-reloading during development.

---

## 📄 Example Code

**HelloController.java**
```java
package com.example.demo;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class HelloController {

    @GetMapping("/hello")
    public String sayHello() {
        return "Hello, Spring Boot!";
    }
}
