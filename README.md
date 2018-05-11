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

Look at the gs-gradle-0.1.0.jar
The class files are bundled up. It’s important to note, that even though you declared joda-time as a dependency, the library isn’t included here. And the JAR file isn’t runnable either.


##Run app after adding application plugin
$ ./gradlew run



To bundle up dependencies requires more thought.
For example, if we were building a WAR file, a format commonly associated with packing in 3rd party dependencies,
we could use gradle’s WAR plugin.
If you are using Spring Boot and want a runnable JAR file, the spring-boot-gradle-plugin is quite handy.
At this stage, gradle doesn’t know enough about your system to make a choice.
But for now, this should be enough to get started using gradle.