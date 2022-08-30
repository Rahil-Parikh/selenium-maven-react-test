# Selenium-Maven-React-Test

This project is a dependency of [Rahil-Parikh/MSD-demo-pipeline](https://github.com/Rahil-Parikh/MSD-demo-pipeline).
This is a Java based implementation of a Selenium sample testing app and contains the following.

## Maven Project
Requires Selenium dependencies to be built and requires gekodriver (Firefoox Webdriver)  directory path in the environment $PATH variable.
The command required to build a dependency jar has to be executed at pom.xml folder level. The command is :
```
mvn clean install assembly:assembly -DdescriptorId=jar-with-dependencies
```
This will generate a jar called selenium.react.test-0.0.1-SNAPSHOT-jar-with-dependencies.jar inside target folder
Inorder to run the Test, execute following command in one line: 
```
java -Dfile.encoding=UTF-8 -classpath target/selenium.react.test-0.0.1-SNAPSHOT-jar-with-dependencies.jar selenium.react.test.ReactTest
```
