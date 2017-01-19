
# Basics

maven standard folder layout `src/main/java`, `src/test/java`
automatic dependencies download
run unit test by default `mvn package`, `gradle build`

# Demo

- create MainClass
- launch with IDE
add pom, build
add build.gradle, build, show Gradle GUI

launch from command line, add MANIFEST
- gradle: add application, launch with `gradle run`

Start using dependencies - 

# Maven 

XML is just for mapping to Java classes
POM, super POM, parent

every step is plugin, specify plugin version!

3 lifecycles with phazes. Type `mvn what-is-lifecycle`

# Gradle

- often releases
- wrapper to keep reproducability

plugin define tasks, tasks can be added, extened, hooked

---

http://www.gradle.org/ vs https://maven.apache.org/
Latest 3.3 vs 3.3.9
Wikipedia is outdated https://en.wikipedia.org/wiki/Gradle vs https://en.wikipedia.org/wiki/Apache_Maven

Maven started in 2004 to address Ant drawbacks, starting from scratches.
Gradle started in 2014 as tool to build Groovy project, and adopting Maven default, supported ant, Ivy, then Android, then non JVM languages like C/C++
Gradle was started under SpringSource, SpringSource was promoting Groovy, then offloaded it. 
Now Groovy is under Apache https://github.com/apache/groovy http://www.groovy-lang.org/


When Google adopted Gradle for Android, that was a big break-though for Gradle (and also hit to Eclipse, when new Android Studio became IDEA CE-based)

Spring-framework is using Gradle, but Spring Boot is using Maven

If you want to do Spring development without no xml at all, then the Maven `pom.xml` is the last mile. Unless you go experimenting with Maven Polyglot.
The problem of Maven Polyglot: "too many languages" and "Who needs this?"
 
Polyglot: Gradle Kotlin script `.gradle.kts`

wrapper is now also in Maven, check Spring Boot Initializer start.spring.io



## Recommendations

### What to use?
If you use Maven, don't hurry to switch to Gradle.
If you still use Ant - you are dying, Gradle was before showing how it is easy to use Gradle over ant, but now deprecating and removing. (Would usage may be 1-5%).
So what to use?
If you have Android development, you may want to have common build tool - Gradle.
If you are having many many modules (with nexus server) Maven is better, but gradle is catching up in 3.x
Use Maven for Spring Boot (until Pivotal change default on it site)

Maven is declarative, straight forward to read. Gradle is more like development.

### What to learn?
First Maven, then mostly Gradle. You can stay with Maven that is more stable, you may go with Gradle that is evolving quicker () and used with Android.

Links
- https://technologyconversations.com/2014/06/18/build-tools/ (Maven 2004, Gradle 2012)
 - https://gradle.org/maven_vs_gradle/
- https://docs.gradle.org/ (latest release notes)
- http://softwareyoga.com/10-reasons-why-we-chose-maven-over-gradle/

