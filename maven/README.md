
# Taskmaster

## Descripción del proyecto

TaskMaster es una aplicación de consola que muetra tareas pendientes.

---

## ▶️ Comandos usados con Maven

### Creación del proyecto:
```bash
mvn archetype:generate -DgroupId=com.equipo.taskmaster -DartifactId=taskmaster -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

### Paso 5: Pruebas unitarias con JUnit
```bash
mvn test
```
- Se añadieron las dependencias de 'org.apache.commons' y 'junit' al archivo pom.xml

#### 🧪 Resultados de Test

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

### Paso 6: Empaquetado y ejecución del .jar
```bash
mvn clean package
mvn exec:java
```

### Paso 7: Agregar perfiles y propiedades

- Se agregaron los perfiles de 'dev' y 'prod' al archivo pom.xml

```xml
  <profiles>
    <profile>
      <id>dev</id>
      <properties>
        <env.name>Desarrollo</env.name>
      </properties>
    </profile>

    <profile>
      <id>prod</id>
      <properties>
        <env.name>Producción</env.name>
      </properties>
    </profile>
  </profiles>
```

```bash
mvn compile
mvn exec:java -Pdev -Denv.name=Dev
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------< com.equipo.taskmaster:taskmaster >------------------
[INFO] Building taskmaster 1.4
[INFO]   from pom.xml
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- exec:3.1.0:java (default-cli) @ taskmaster ---
¡Bienvenido a TaskMaster!
Ambiente: Dev
Tareas pendientes:
- Estudiar Maven
- Leer sobre CI/CD
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  0.256 s
[INFO] Finished at: 2025-06-11T22:11:21-04:00
[INFO] ------------------------------------------------------------------------
```

## 📦 Dependencias utilizadas

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

## 📁 Estructura del proyecto

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
