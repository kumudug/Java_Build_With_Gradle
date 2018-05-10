# Java_Build_With_Gradle
Building Java Projects with Gradle. This guide walks you through using Gradle to build a simple Java project.

https://spring.io/guides/gs/gradle/

gradle tasks - shows a list of gradle tasks

gradle build - build the project using gradle

## Gradle Wrapper
To build without having gradle installed.
Run : $ gradle wrapper --gradle-version 4.7
This adds gradlew and gradlew.bat to root and add gradle-wrapper.jar and gradle-wrapperproperties inside gradle/wrapper folder
Now you can build your project without gradle using
./gradlew build

