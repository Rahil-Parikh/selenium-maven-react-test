[![](https://img.shields.io/badge/Made_with-Maven-maroon?style=for-the-badge&logo=Apache%20Maven&logoColor=white)](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)![Selenium](https://img.shields.io/badge/-selenium-%43B02A?style=for-the-badge&logo=selenium&logoColor=white)
<span><h2 align="center">Selenium Maven React Test</h2></span>

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
