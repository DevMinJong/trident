# trident

Trident-Java is a lightweight SDK that includes libraries for working with TRON system contracts and smart contracts.

Trident-Java makes it easy to build TRON applications with java.

Trident-Java document: https://developers.tron.network/docs/trident-java

Due to safety concerns, trident-java will no longer upload packaged files to maven. Please clone the code from GitHub and do the packaging. 

Trident-java is compiled with java version 13.0.2+8 and gradle 5.6.4.

## How to use

### Gradle Setting

Add repo setting:

```groovy
repositories {
    mavenCentral()
}
```

Then add required packages as dependencies. Please add dependencies locally.

```groovy
dependencies {
    // protobuf & grpc
    implementation 'com.google.protobuf:protobuf-java:3.11.0'

    implementation fileTree(dir:'../core')
    implementation fileTree(dir:'../utils')
    implementation fileTree(dir:'../abi')

    implementation 'com.google.guava:guava:28.0-jre'
}
```

### Maven Settings

```xml
<dependency>
  <groupId>org.tron.trident</groupId>
  <artifactId>abi</artifactId>
  <version>0.1.1</version>
  <type>pom</type>
</dependency>
<dependency>
  <groupId>org.tron.trident</groupId>
  <artifactId>utils</artifactId>
  <version>0.1.1</version>
  <type>pom</type>
</dependency>
<dependency>
  <groupId>org.tron.trident</groupId>
  <artifactId>core</artifactId>
  <version>0.1.1</version>
  <type>pom</type>
</dependency>
```

