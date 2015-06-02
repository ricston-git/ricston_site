## About gradle

Gradle is a project build automation tool that uses a Groovy DSL. Gradle build scripts support Maven and Ivy repositories as well as plain file system for dependency management.

[Gradle](http://gradle.org/) is a build automation tool that uses a Groovy DSL. In Gradle one can use Maven or Ivy as a platform for dependency management.

Gradle allows you to describe the automation of a project build both declaratively _and_ imperatively as you have the full power of the Groovy programming language to describe Gradle [tasks](http://www.gradle.org/docs/current/userguide/userguide_single.html#tutorial_using_tasks).

Latest Version: [2.4](https://gradle.org/docs/current/release-notes) (5th May 2015)

The default name for the build script is `build.gradle`

**Expressing a project dependency**

    repositories {
        mavenCentral()
    }

    dependencies {
        testCompile 'junit:junit:4.12'
    }

**Defining a task**

Using a Groovy closure in defining a task count:

    task count << {
        4.times { print "$it " }
    }

Output of running `gradle -q count`:

    > gradle -q count
    0 1 2 3

**Links:**

*   [Download Gradle](http://www.gradle.org/downloads)
*   [Documentation](http://www.gradle.org/documentation)
*   [Forum](http://forums.gradle.org/gradle)
*   [Wiki](http://en.wikipedia.org/wiki/Gradle)