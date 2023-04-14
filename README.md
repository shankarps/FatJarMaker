## FatJarMaker

This project is a utility tool to combine multiple Jar files to make a single fat Jar.

This project is useful when deploying Amazon Kinesis Data applications (KDA) that requires multiple Jar libraries.

KDA requires that the multiple Jar files be combined into a single Jar file for deployment.

This project was created specifically for helping this question on stackoverflow.com - https://stackoverflow.com/questions/76000492/how-to-make-fat-jar-in-aws-kda-flink-application

### Prerequisites
   **Important** Ensure that the two prerequisites are installed.

1. Java 11 (or your most compatible version)
   * For MacOS use SDKMan to install Java.
   * For Windows, follow the instructions in the JDK's user manual.
2. Maven 3.x
    * For MacOS use Homebrew to install 

### Instructions

1. Clone the project. ```git clone https://github.com/shankarps/FatJarMaker.git```
2. Modify the pom.xml file to add the dependencies you want to combine into the fat jar.
3. Run command ```mvn clean package```
4. The fat jar will be in the subfolder ./target. The default name will be "FatJarMaker-1.0-SNAPSHOT-combined.jar"
