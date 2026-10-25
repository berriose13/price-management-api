# 🚀 Between — Price Analysis Backend

### Java 17 | Spring Boot 3 | Spring Data JPA | Hibernate | H2 | MapStruct

A Java backend project focused on price analysis and data management, developed using the Spring Boot ecosystem.

The project brings together RESTful web development, relational data persistence, object mapping, and an embedded database environment.

## 🛠️ Tech Stack

| Technology | Description |
|---|---|
| Java 17 | Backend programming language |
| Spring Boot 3.2.1 | Application framework |
| Spring Web MVC | HTTP and web application development |
| Spring Data JPA | Database access and persistence |
| Hibernate | Object-relational mapping |
| H2 Database | Embedded in-memory relational database |
| MapStruct | Object mapping between application models |
| Lombok | Reduction of Java boilerplate code |
| Maven | Dependency management and build automation |
| Spring Boot Test | Testing infrastructure |

## 🎯 Project Overview

Between is a backend project focused on managing and analyzing pricing information through a Java-based application.

The project uses Spring Boot to integrate application components, Spring Data JPA for persistence, and H2 as an embedded relational database.

Its technology stack provides a foundation for implementing and testing pricing-related business logic.

## 🏗️ Technical Overview

The application includes the following technical capabilities and dependencies:

- **Java Backend:** Development with Java 17 and Spring Boot.
- **Web Development:** Spring Web MVC support for HTTP-based application interfaces.
- **Data Persistence:** Relational data access using Spring Data JPA and Hibernate.
- **Embedded Database:** H2 for local development and testing.
- **Object Mapping:** MapStruct for mapping Java objects.
- **Development Productivity:** Lombok for reducing repetitive code.
- **Build Management:** Maven Wrapper for consistent project builds.
- **Testing Support:** Spring Boot testing dependencies.

## ⚙️ Getting Started

### Prerequisites

Before running the application, make sure you have:

- Java Development Kit (JDK) 17 or higher
- Git
- An IDE such as IntelliJ IDEA (optional)

The project includes Maven Wrapper, so a separate Maven installation is not required.

### 1. Clone the Repository

```bash
git clone https://github.com/berriose13/between.git
cd between
```

### 2. Build the Project

On Linux or macOS:

```bash
./mvnw clean package
```

On Windows:

```bash
mvnw.cmd clean package
```

### 3. Run the Application

```bash
./mvnw spring-boot:run
```

The default Spring Boot HTTP port is `8080`, unless overridden by the application configuration.

## 🗄️ Database Configuration

The project uses an H2 in-memory database.

The application properties include:

```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto=create

spring.h2.console.enabled=true
spring.h2.console.path=/h2-console
```

### H2 Console

Once the application is running, access:

```text
http://localhost:8080/h2-console
```

Connection settings:

| Property | Value |
|---|---|
| JDBC URL | jdbc:h2:mem:testdb |
| Username | sa |
| Password | Empty |

**Note:** H2 is configured as an in-memory database. Data is not preserved across application restarts. The configured Hibernate schema generation also recreates the schema on startup.

## 🧪 Testing

The project includes Spring Boot testing dependencies.

To execute the available tests:

```bash
./mvnw test
```

Testing support can be used to verify application components, business logic, and persistence behavior.

## 📦 Build Artifact

To generate the application JAR:

```bash
./mvnw clean package
```

Maven generates build artifacts inside the `target/` directory.

## 🔧 Configuration and Development

The application uses Maven for dependency management and Spring Boot for application configuration.

Core dependencies are defined in `pom.xml`, while the database settings are located in:

```text
src/main/resources/application.properties
```

## 👨‍💻 Author

**Eleazar Berrios**

Java Backend Developer

**GitHub:** [@berriose13](https://github.com/berriose13)

## 📌 Repository

[github.com/berriose13/between](https://github.com/berriose13/between)
