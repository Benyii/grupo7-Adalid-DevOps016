
## Descripción del proyecto

TaskMaster es una aplicación de consola que permite almacenar y mostrar tareas pendientes. Este proyecto fue creado con el objetivo de aprender a usar Maven como herramienta de gestión de proyectos y dependencias.

---

## ▶️ Comandos usados con Maven

### Creación del proyecto:
```bash
mvn archetype:generate -DgroupId=com.equipo.taskmaster -DartifactId=taskmaster -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
mvn test
mvn clean package
mvn exec:java
```

# 📦 Dependencias utilizadas

```xml
<dependencies>
    <dependency>
        <groupId>org.apache.commons</groupId>
        <artifactId>commons-lang3</artifactId>
        <version>3.12.0</version>
    </dependency>
    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.13.2</version>
        <scope>test</scope>
    </dependency>
</dependencies>
```

# 📁 Estructura del proyecto

```bash
taskmaster/
├── pom.xml
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/equipo/taskmaster/App.java
│   └── test/
│       └── java/
│           └── com/equipo/taskmaster/AppTest.java
```

# 🧪 Resultados de Test

```bash
[INFO]
[INFO]
[INFO] -------------------------------------------------------
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.equipo.taskmaster.AppTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.012 s -- in com.equipo.taskmaster.AppTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------                                                                                                                                                                                                  
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------                                                                                                                                                                                                  
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------                                                                                                                                                                                                  
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------                                                                                                                                                                                                  
[INFO] Total time:  2.311 s
[INFO] Finished at: 2025-06-11T21:55:55-04:00
[INFO] ------------------------------------------------------------------------  
```