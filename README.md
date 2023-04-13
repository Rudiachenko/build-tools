### Tools
To build project Maven or Gradle is required:
https://maven.apache.org/
https://docs.gradle.org/current/userguide/installation.html

### Maven Build
Run following command to build project.
```bash
mvn clean install
```
*You are calling the mvn executable, which means you need Maven installed on your machine.

*You are using the clean command, which will delete all previously compiled Java .class files and resources (like .properties) in  project. Your build will start from a clean state.

*Install will then compile, test & package project and even install/copy your built .jar/.war file into your local Maven repository.
### Test
Run following command to test all modules
```bash
mvn test
```

### Gradle Build
Run following command to build project
```bash
gradle clean build
```
Logic the same as in Maven
### Test
Run following command to only test all modules
```bash
gradle test
```
### Building a single jar
To package modules 'admin', 'services', 'utils' run following command.

.jar file will be packaged to '/build/jars' folder
```bash
gradle packageJar
```
### Building a single war
To package modules 'web' run following command.

.war file will be packaged to '/build/wars' folder
```bash
gradle packageWar
```