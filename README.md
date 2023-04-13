# Build tools - Maven
Build tools is a Java project for learning build tools Maven and Gradle(Maven in this case).
### Tools
To buind project using maven [Apache Maven] is requeired(https://maven.apache.org/).
### Build
Run following command to build project.
```bash
mvn clean install
```
it will automatically test and build each module and package them in 'maven/target' folder.

Modules 'admin', 'services', 'utils' to 'jar-final-app.jar' file and 'web' module to 'war-final-app.war' file
### Test
Run following command to test all modules
```bash
mvn test
```

# Build tools - Gradle
Build tools is a Java project for learning build tools Maven and Gradle(Gradle in this case).
### Tools
Before proceeding, install a [JDK](https://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html)
(must be Java 8 or later) and [Gradle](https://docs.gradle.org/current/userguide/installation.html).
### Build
Run following command to build project
```bash
gradle clean build
```
### Test
Run following command to test all modules
```bash
gradle test
```
### Building a single jar
To package modules 'admin', 'services', 'utils' run following command.

.jar file will be packaged to '/build' folder
```bash
gradle packageJar
```
### Building a single war
To package modules 'web' run following command.

.war file will be packaged to '/build' folder
```bash
gradle packageWar
```