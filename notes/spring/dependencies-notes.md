# Java & Spring Boot Dependencies Reference / Referencia de Dependencias de Java y Spring Boot

### 1. Spring Boot Base Dependencies

_Core dependencies required for Spring Boot projects._

| Description                                       | Dependency                                                                                                                                                                                                                                          |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot starter core (auto-configures Spring) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter'` |

---

### 2. Web / REST

_Dependencies for building REST APIs and web applications._

| Description                                           | Dependency                                                                                                                                                                                                                                                              |
| ----------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot web starter (Spring MVC, Tomcat)          | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-web</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-web'`             |
| Spring Boot Thymeleaf starter (server-side templates) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-thymeleaf</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-thymeleaf'` |

---

### 3. Security

_Dependencies for authentication, authorization, and security._

| Description             | Dependency                                                                                                                                                                                                                                                            |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Security starter | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-security</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-security'` |

---

### 4. Persistence (JPA / Hibernate)

_Dependencies for ORM, JPA, and database interaction._

| Description                  | Dependency                                                                                                                                                                                                                                                            |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot Data JPA starter | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-data-jpa</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-data-jpa'` |

---

### 5. Databases

_Dependencies for relational databases._

| Description            | Dependency                                                                                                                                                                                                                               |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MySQL JDBC driver      | **Maven:**<br>`xml<br><dependency><br>  <groupId>mysql</groupId><br>  <artifactId>mysql-connector-java</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'mysql:mysql-connector-java'` |
| PostgreSQL JDBC driver | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.postgresql</groupId><br>  <artifactId>postgresql</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'org.postgresql:postgresql'`   |
| H2 in-memory database  | **Maven:**<br>`xml<br><dependency><br>  <groupId>com.h2database</groupId><br>  <artifactId>h2</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'com.h2database:h2'`                   |

---

### 6. Validation

_Dependencies for bean validation._

| Description                              | Dependency                                                                                                                                                                                                                                                                |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot starter validation (JSR-303) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-validation</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-validation'` |

---

### 7. Testing

_Dependencies for unit and integration testing._

| Description                               | Dependency                                                                                                                                                                                                                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Spring Boot starter test (JUnit, Mockito) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-test</artifactId><br>  <scope>test</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>testImplementation 'org.springframework.boot:spring-boot-starter-test'` |

---

### 8. Documentation (Swagger / OpenAPI)

_Dependencies for API documentation._

| Description          | Dependency                                                                                                                                                                                                                                                          |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Springdoc OpenAPI UI | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springdoc</groupId><br>  <artifactId>springdoc-openapi-ui</artifactId><br>  <version>1.8.0</version><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springdoc:springdoc-openapi-ui:1.8.0'` |

---

### 9. Logging

_Dependencies for logging._

| Description                                  | Dependency                                                                                                                                                                                                                                                          |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot logging starter (Logback, SLF4J) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-logging</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-logging'` |

---

### 10. Utilities

_Common utility dependencies._

| Description         | Dependency                                                                                                                                                                                                                  |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Apache Commons Lang | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.apache.commons</groupId><br>  <artifactId>commons-lang3</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.apache.commons:commons-lang3'` |

---

### 11. Lombok

_Dependency to reduce boilerplate code using annotations._

| Description    | Dependency                                                                                                                                                                                                                                                                              |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lombok library | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.projectlombok</groupId><br>  <artifactId>lombok</artifactId><br>  <scope>provided</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>compileOnly 'org.projectlombok:lombok'<br>annotationProcessor 'org.projectlombok:lombok'` |

---

### 12. DevTools & Development

_Dependencies for development efficiency._

| Description                                           | Dependency                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Spring Boot DevTools (automatic restart, live reload) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-devtools</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'org.springframework.boot:spring-boot-devtools'` |

---

## **Versión en Español**

### 1. Dependencias Base de Spring Boot

_Dependencias básicas requeridas para proyectos Spring Boot._

| Descripción                               | Dependencia                                                                                                                                                                                                                                         |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Núcleo de Spring Boot (autoconfiguración) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter'` |

---

### 2. Web / REST

_Dependencias para construir APIs REST y aplicaciones web._

| Descripción                                                 | Dependencia                                                                                                                                                                                                                                                             |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot starter web (Spring MVC, Tomcat)                | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-web</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-web'`             |
| Spring Boot Thymeleaf starter (templates del lado servidor) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-thymeleaf</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-thymeleaf'` |

---

### 3. Seguridad

_Dependencias para autenticación y autorización._

| Descripción             | Dependencia                                                                                                                                                                                                                                                           |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Security starter | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-security</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-security'` |

---

### 4. Persistencia (JPA / Hibernate)

_Dependencias para ORM, JPA y acceso a base de datos._

| Descripción                  | Dependencia                                                                                                                                                                                                                                                           |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot Data JPA starter | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-data-jpa</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-data-jpa'` |

---

### 5. Bases de Datos

_Dependencias para bases de datos relacionales._

| Descripción                 | Dependencia                                                                                                                                                                                                                              |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Driver JDBC MySQL           | **Maven:**<br>`xml<br><dependency><br>  <groupId>mysql</groupId><br>  <artifactId>mysql-connector-java</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'mysql:mysql-connector-java'` |
| Driver JDBC PostgreSQL      | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.postgresql</groupId><br>  <artifactId>postgresql</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'org.postgresql:postgresql'`   |
| Base de datos en memoria H2 | **Maven:**<br>`xml<br><dependency><br>  <groupId>com.h2database</groupId><br>  <artifactId>h2</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'com.h2database:h2'`                   |

---

### 6. Validación

_Dependencias para validación de beans._

| Descripción                              | Dependencia                                                                                                                                                                                                                                                               |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot starter validation (JSR-303) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-validation</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-validation'` |

---

### 7. Testing

_Dependencias para pruebas unitarias e integración._

| Descripción                               | Dependencia                                                                                                                                                                                                                                                                                |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Spring Boot starter test (JUnit, Mockito) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-test</artifactId><br>  <scope>test</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>testImplementation 'org.springframework.boot:spring-boot-starter-test'` |

---

### 8. Documentación (Swagger / OpenAPI)

_Dependencias para documentación de APIs._

| Descripción          | Dependencia                                                                                                                                                                                                                                                         |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Springdoc OpenAPI UI | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springdoc</groupId><br>  <artifactId>springdoc-openapi-ui</artifactId><br>  <version>1.8.0</version><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springdoc:springdoc-openapi-ui:1.8.0'` |

---

### 9. Logging

_Dependencias para registro de eventos y logs._

| Descripción                                  | Dependencia                                                                                                                                                                                                                                                         |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spring Boot starter logging (Logback, SLF4J) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-starter-logging</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.springframework.boot:spring-boot-starter-logging'` |

---

### 10. Utilidades

_Dependencias de utilidades comunes._

| Descripción         | Dependencia                                                                                                                                                                                                                 |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Apache Commons Lang | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.apache.commons</groupId><br>  <artifactId>commons-lang3</artifactId><br></dependency>`<br>**Gradle:**<br>`groovy<br>implementation 'org.apache.commons:commons-lang3'` |

---

### 11. Lombok

_Dependencia para reducir código repetitivo usando anotaciones._

| Descripción     | Dependencia                                                                                                                                                                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Librería Lombok | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.projectlombok</groupId><br>  <artifactId>lombok</artifactId><br>  <scope>provided</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>compileOnly 'org.projectlombok:lombok'<br>annotationProcessor 'org.projectlombok:lombok'` |

---

### 12. DevTools y Desarrollo

_Dependencias para eficiencia en desarrollo._

| Descripción                                             | Dependencia                                                                                                                                                                                                                                                                    |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Spring Boot DevTools (reinicio automático, live reload) | **Maven:**<br>`xml<br><dependency><br>  <groupId>org.springframework.boot</groupId><br>  <artifactId>spring-boot-devtools</artifactId><br>  <scope>runtime</scope><br></dependency>`<br>**Gradle:**<br>`groovy<br>runtimeOnly 'org.springframework.boot:spring-boot-devtools'` |

---
