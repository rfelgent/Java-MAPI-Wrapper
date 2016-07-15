About
=====

Fork of [Java-MAPI-Wrapper](http://github.com/brightcoveos/Java-MAPI-Wrapper)

In comparison to the original Github repo this project offers:

* Gradle 2.5 build management
* all Ant targets are reflected as Gradle tasks those name is prefixed with "a_", for instance: the Ant target "main" is available as Gradle task named "a_main"

Note: The file hierarchy is not touched at all on purpose! So the project setup is not really "clean", as I wanted the modifications less invasive!

Usage
=====

First you must build the complete project by invoking
```sh
./gradlew build
```
This will download *all* (transitive) dependencies required by java-mapi-wrapper and the Ant build script.

After that you can execute the Ant targets defined in build.xml via Gradle:
```sh
./gradlew a_main
```