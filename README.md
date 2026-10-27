# SWTModular
![Maven Central Version](https://img.shields.io/maven-central/v/io.github.sundenjaeger/SWTModular)

> [!NOTE]
> Windows x86_64 only. Based on SWT version 3.135.0. Intended for use with jlink where all dependencies must be proper JPMS modules.

Modularized version of Eclipse SWT for Windows (win32 x86_64). Adds a `module-info` to the original SWT jar for JPMS and `jlink` compatibility.

# Usage

### Maven

```xml
<dependency>
    <groupId>io.github.sundenjaeger</groupId>
    <artifactId>SWTModular</artifactId>
    <version>1.0.2</version>
</dependency>
```

### Gradle

```groovy
implementation("io.github.sundenjaeger:SWTModular:1.0.2")
```

# Running

SWT requires native access to be explicitly enabled. Add the following JVM argument when running your application:
```
--enable-native-access=org.eclipse.swt.win32.win32.x86_64
```

# Building Locally

```
mvn install
```