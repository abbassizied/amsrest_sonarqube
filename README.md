

- on linux
```sh
mvn clean verify sonar:sonar \
  -Dsonar.projectKey=ams_rest \
  -Dsonar.projectName='ams_rest' \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.token=sqp_7369bfd4293a4cdde190d56cf4fb2103fd2beef2
``` 

- on windows:
```sh
mvn clean install -DskipTests

mvn clean verify sonar:sonar -Dsonar.projectKey=ams_rest -Dsonar.projectName='ams_rest' -Dsonar.host.url=http://localhost:9000 -Dsonar.token=sqp_7369bfd4293a4cdde190d56cf4fb2103fd2beef2 -DskipTests


mvn clean verify sonar:sonar -DskipTests
``` 




# refs:

- [sonar-maven-plugin](https://central.sonatype.com/artifact/org.sonarsource.scanner.maven/sonar-maven-plugin/3.9.0.2155)
- [Sample project](https://github.com/SonarSource/sonar-scanning-examples/tree/master/sonar-scanner-maven/maven-basic)
- [SonarQube extension for Jenkins](https://docs.sonarsource.com/sonarqube/latest/analyzing-source-code/scanners/jenkins-extension-sonarqube/)

- [Introduction to the server installation](https://docs.sonarsource.com/sonarqube/latest/setup-and-upgrade/install-the-server/introduction/)
- [Installing the SonarQube database](https://docs.sonarsource.com/sonarqube/latest/setup-and-upgrade/install-the-server/installing-the-database/)
- [JaCoCo :: Maven Plugin ](https://mvnrepository.com/artifact/org.jacoco/jacoco-maven-plugin/0.8.12)
- [SonarScanner for Maven](https://docs.sonarsource.com/sonarqube/latest/analyzing-source-code/scanners/sonarscanner-for-maven/)



