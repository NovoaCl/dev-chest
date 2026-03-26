# Java & Spring Boot Annotations Reference / Referencia de Anotaciones de Java y Spring Boot

### 1. Basic Java Annotations

*Core annotations provided by Java for code documentation and behavior.*

| Description                                           | Annotation             |
| ----------------------------------------------------- | ---------------------- |
| Indicates that a method overrides a superclass method | `@Override`            |
| Marks an element as deprecated                        | `@Deprecated`          |
| Suppresses compiler warnings                          | `@SuppressWarnings`    |
| Indicates a functional interface                      | `@FunctionalInterface` |
| Marks a method as safe for concurrent use             | `@SafeVarargs`         |

---

### 2. Spring Core Annotations

*Core annotations for Spring framework components.*

| Description                                      | Annotation                 |
| ------------------------------------------------ | -------------------------- |
| Marks a class as a Spring-managed component      | `@Component`               |
| Specialized component for service layer          | `@Service`                 |
| Specialized component for repository (DAO) layer | `@Repository`              |
| Marks a class as a Spring controller             | `@Controller`              |
| Indicates configuration class                    | `@Configuration`           |
| Enables Spring Boot auto-configuration           | `@EnableAutoConfiguration` |
| Indicates a method produces a bean               | `@Bean`                    |

---

### 3. Dependency Injection

*Annotations for injecting beans into Spring-managed components.*

| Description                                                   | Annotation                     |
| ------------------------------------------------------------- | ------------------------------ |
| Injects a dependency automatically by type                    | `@Autowired`                   |
| Specifies which bean to inject when multiple candidates exist | `@Qualifier`                   |
| Injects a dependency via constructor                          | `@Inject` (JSR-330 compatible) |
| Injects value from properties or environment                  | `@Value("${property.name}")`   |

---

### 4. Configuration

*Annotations used for application and Spring configuration.*

| Description                                    | Annotation                 |
| ---------------------------------------------- | -------------------------- |
| Marks a class as configuration                 | `@Configuration`           |
| Declares a method as a bean producer           | `@Bean`                    |
| Enables automatic configuration in Spring Boot | `@EnableAutoConfiguration` |
| Marks a class to enable component scanning     | `@ComponentScan`           |

---

### 5. Web / REST

*Annotations for building REST APIs and web controllers.*

| Description                                              | Annotation        |
| -------------------------------------------------------- | ----------------- |
| Combines `@Controller` and `@ResponseBody` for REST APIs | `@RestController` |
| Maps HTTP requests to methods or classes                 | `@RequestMapping` |
| Maps GET HTTP requests                                   | `@GetMapping`     |
| Maps POST HTTP requests                                  | `@PostMapping`    |
| Maps PUT HTTP requests                                   | `@PutMapping`     |
| Maps DELETE HTTP requests                                | `@DeleteMapping`  |
| Binds a method parameter to a path variable              | `@PathVariable`   |
| Binds a method parameter to request parameters           | `@RequestParam`   |
| Binds the HTTP request body to an object                 | `@RequestBody`    |

---

### 6. Persistence (JPA / Hibernate)

*Annotations for database entity mapping and persistence.*

| Description                                | Annotation        |
| ------------------------------------------ | ----------------- |
| Marks a class as a JPA entity              | `@Entity`         |
| Marks the primary key of an entity         | `@Id`             |
| Specifies how the primary key is generated | `@GeneratedValue` |
| Maps a field to a database column          | `@Column`         |
| Specifies relationships: OneToOne          | `@OneToOne`       |
| Specifies relationships: OneToMany         | `@OneToMany`      |
| Specifies relationships: ManyToOne         | `@ManyToOne`      |
| Specifies relationships: ManyToMany        | `@ManyToMany`     |
| Specifies table name for an entity         | `@Table`          |
| Marks a field as transient (not persisted) | `@Transient`      |

---

### 7. Validation

*Annotations for validating method parameters, fields, or beans.*

| Description                          | Annotation            |
| ------------------------------------ | --------------------- |
| Validates a bean or method parameter | `@Valid`              |
| Ensures the field is not null        | `@NotNull`            |
| Ensures the field is not empty       | `@NotEmpty`           |
| Ensures the field is not blank       | `@NotBlank`           |
| Validates string length              | `@Size(min=, max=)`   |
| Validates numeric minimum            | `@Min(value)`         |
| Validates numeric maximum            | `@Max(value)`         |
| Validates email format               | `@Email`              |
| Validates pattern with regex         | `@Pattern(regexp="")` |

---

### 8. Security

*Annotations for securing methods and endpoints.*

| Description                                | Annotation                     |
| ------------------------------------------ | ------------------------------ |
| Enables method-level security annotations  | `@EnableGlobalMethodSecurity`  |
| Secures a method or endpoint with a role   | `@Secured("ROLE_NAME")`        |
| Pre-authorizes access based on expression  | `@PreAuthorize("expression")`  |
| Post-authorizes access based on expression | `@PostAuthorize("expression")` |

---

### 9. Testing

*Annotations for writing unit and integration tests.*

| Description                          | Annotation           |
| ------------------------------------ | -------------------- |
| Marks a Spring Boot test class       | `@SpringBootTest`    |
| Mocks a bean in the Spring context   | `@MockBean`          |
| Marks a test method in JUnit         | `@Test`              |
| Repeats a test or parameterized test | `@ParameterizedTest` |
| Before each test execution           | `@BeforeEach`        |
| After each test execution            | `@AfterEach`         |
| Before all tests in class            | `@BeforeAll`         |
| After all tests in class             | `@AfterAll`          |

---

### 10. Lombok

*Annotations from Lombok library to reduce boilerplate code.*

| Description                                     | Annotation                 |
| ----------------------------------------------- | -------------------------- |
| Generates getters and setters                   | `@Data`                    |
| Generates only getters                          | `@Getter`                  |
| Generates only setters                          | `@Setter`                  |
| Generates a constructor with required arguments | `@RequiredArgsConstructor` |
| Generates a no-args constructor                 | `@NoArgsConstructor`       |
| Generates an all-args constructor               | `@AllArgsConstructor`      |
| Generates `equals` and `hashCode`               | `@EqualsAndHashCode`       |
| Generates `toString` method                     | `@ToString`                |

---

### 11. Advanced Utilities

*Additional Spring and Java annotations for advanced usage.*

| Description                    | Annotation                  |
| ------------------------------ | --------------------------- |
| Conditional bean registration  | `@Conditional`              |
| Profile-specific configuration | `@Profile("dev")`           |
| Scheduling tasks               | `@Scheduled(cron = "...")`  |
| Asynchronous methods           | `@Async`                    |
| Transaction management         | `@Transactional`            |
| Caching support                | `@Cacheable`, `@CacheEvict` |

---

## **Versión en Español**

### 1. Anotaciones Básicas de Java

*Anotaciones proporcionadas por Java para documentación y comportamiento del código.*

| Descripción                                                 | Anotación              |
| ----------------------------------------------------------- | ---------------------- |
| Indica que un método sobrescribe un método de la superclase | `@Override`            |
| Marca un elemento como obsoleto                             | `@Deprecated`          |
| Suprime advertencias del compilador                         | `@SuppressWarnings`    |
| Indica una interfaz funcional                               | `@FunctionalInterface` |
| Marca un método como seguro para uso concurrente            | `@SafeVarargs`         |

---

### 2. Anotaciones de Spring Core

*Anotaciones básicas del framework Spring para componentes.*

| Descripción                                                | Anotación                  |
| ---------------------------------------------------------- | -------------------------- |
| Marca una clase como componente gestionado por Spring      | `@Component`               |
| Componente especializado para la capa de servicios         | `@Service`                 |
| Componente especializado para la capa de repositorio (DAO) | `@Repository`              |
| Marca una clase como controlador de Spring                 | `@Controller`              |
| Indica una clase de configuración                          | `@Configuration`           |
| Habilita la autoconfiguración de Spring Boot               | `@EnableAutoConfiguration` |
| Indica que un método produce un bean                       | `@Bean`                    |

---

### 3. Inyección de Dependencias

*Anotaciones para inyectar beans en componentes gestionados por Spring.*

| Descripción                                                  | Anotación                      |
| ------------------------------------------------------------ | ------------------------------ |
| Inyecta una dependencia automáticamente por tipo             | `@Autowired`                   |
| Especifica qué bean inyectar cuando hay múltiples candidatos | `@Qualifier`                   |
| Inyecta una dependencia mediante constructor                 | `@Inject` (compatible JSR-330) |
| Inyecta valor desde propiedades o ambiente                   | `@Value("${property.name}")`   |

---

### 4. Configuración

*Anotaciones para configuración de aplicación y Spring.*

| Descripción                                           | Anotación                  |
| ----------------------------------------------------- | -------------------------- |
| Marca una clase como clase de configuración           | `@Configuration`           |
| Declara un método como productor de bean              | `@Bean`                    |
| Habilita autoconfiguración en Spring Boot             | `@EnableAutoConfiguration` |
| Marca una clase para habilitar escaneo de componentes | `@ComponentScan`           |

---

### 5. Web / REST

*Anotaciones para construir APIs REST y controladores web.*

| Descripción                                            | Anotación         |
| ------------------------------------------------------ | ----------------- |
| Combina `@Controller` y `@ResponseBody` para APIs REST | `@RestController` |
| Mapea solicitudes HTTP a métodos o clases              | `@RequestMapping` |
| Mapea solicitudes HTTP GET                             | `@GetMapping`     |
| Mapea solicitudes HTTP POST                            | `@PostMapping`    |
| Mapea solicitudes HTTP PUT                             | `@PutMapping`     |
| Mapea solicitudes HTTP DELETE                          | `@DeleteMapping`  |
| Enlaza parámetro de método a variable de ruta          | `@PathVariable`   |
| Enlaza parámetro de método a parámetros de petición    | `@RequestParam`   |
| Enlaza el cuerpo de la petición HTTP a un objeto       | `@RequestBody`    |

---

### 6. Persistencia (JPA / Hibernate)

*Anotaciones para mapeo de entidades y persistencia de datos.*

| Descripción                                      | Anotación         |
| ------------------------------------------------ | ----------------- |
| Marca una clase como entidad JPA                 | `@Entity`         |
| Marca la clave primaria de la entidad            | `@Id`             |
| Especifica cómo se genera la clave primaria      | `@GeneratedValue` |
| Mapea un campo a una columna de base de datos    | `@Column`         |
| Relación uno a uno                               | `@OneToOne`       |
| Relación uno a muchos                            | `@OneToMany`      |
| Relación muchos a uno                            | `@ManyToOne`      |
| Relación muchos a muchos                         | `@ManyToMany`     |
| Especifica el nombre de tabla de la entidad      | `@Table`          |
| Marca un campo como transitorio (no persistente) | `@Transient`      |

---

### 7. Validación

*Anotaciones para validar parámetros de método, campos o beans.*

| Descripción                            | Anotación             |
| -------------------------------------- | --------------------- |
| Valida un bean o parámetro de método   | `@Valid`              |
| Asegura que el campo no sea nulo       | `@NotNull`            |
| Asegura que el campo no esté vacío     | `@NotEmpty`           |
| Asegura que el campo no esté en blanco | `@NotBlank`           |
| Valida longitud de cadena              | `@Size(min=, max=)`   |
| Valida valor mínimo numérico           | `@Min(value)`         |
| Valida valor máximo numérico           | `@Max(value)`         |
| Valida formato de correo electrónico   | `@Email`              |
| Valida patrón con expresión regular    | `@Pattern(regexp="")` |

---

### 8. Seguridad

*Anotaciones para proteger métodos y endpoints.*

| Descripción                                         | Anotación                      |
| --------------------------------------------------- | ------------------------------ |
| Habilita anotaciones de seguridad a nivel de método | `@EnableGlobalMethodSecurity`  |
| Protege un método o endpoint por rol                | `@Secured("ROLE_NAME")`        |
| Preautoriza acceso basado en expresión              | `@PreAuthorize("expression")`  |
| Postautoriza acceso basado en expresión             | `@PostAuthorize("expression")` |

---

### 9. Testing

*Anotaciones para pruebas unitarias e integración.*

| Descripción                          | Anotación            |
| ------------------------------------ | -------------------- |
| Marca clase de prueba de Spring Boot | `@SpringBootTest`    |
| Mockea un bean en contexto Spring    | `@MockBean`          |
| Marca método de prueba en JUnit      | `@Test`              |
| Repite o parametriza prueba          | `@ParameterizedTest` |
| Ejecuta antes de cada prueba         | `@BeforeEach`        |
| Ejecuta después de cada prueba       | `@AfterEach`         |
| Ejecuta antes de todas las pruebas   | `@BeforeAll`         |
| Ejecuta después de todas las pruebas | `@AfterAll`          |

---

### 10. Lombok

*Anotaciones de Lombok para reducir código repetitivo.*

| Descripción                                  | Anotación                  |
| -------------------------------------------- | -------------------------- |
| Genera getters y setters                     | `@Data`                    |
| Genera solo getters                          | `@Getter`                  |
| Genera solo setters                          | `@Setter`                  |
| Genera constructor con argumentos requeridos | `@RequiredArgsConstructor` |
| Genera constructor sin argumentos            | `@NoArgsConstructor`       |
| Genera constructor con todos los argumentos  | `@AllArgsConstructor`      |
| Genera `equals` y `hashCode`                 | `@EqualsAndHashCode`       |
| Genera método `toString`                     | `@ToString`                |

---

### 11. Utilidades Avanzadas

*Anotaciones adicionales de Spring y Java para uso avanzado.*

| Descripción                         | Anotación                   |
| ----------------------------------- | --------------------------- |
| Registro condicional de beans       | `@Conditional`              |
| Configuración específica por perfil | `@Profile("dev")`           |
| Programación de tareas              | `@Scheduled(cron = "...")`  |
| Métodos asíncronos                  | `@Async`                    |
| Gestión de transacciones            | `@Transactional`            |
| Soporte de caching                  | `@Cacheable`, `@CacheEvict` |

---
