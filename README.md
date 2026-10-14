# MavenDemo

A minimal Java 21 Maven project for testing a Jenkins Maven build.

## Requirements
- JDK 21
- Maven 3.8+ (or a compatible newer version)

## Build
Run from the directory containing `pom.xml`:

```bash
mvn clean package
```

## Run
```bash
mvn exec:java
```

Expected output:
```text
Hello from Maven!
Jenkins Maven build is successful!
```

## Jenkins Freestyle job
1. Configure the repository under Source Code Management > Git.
2. Add a Maven build step with goals: `clean package`.
