# stream-java

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.getstream.client/stream-java/badge.svg?style=flat)](https://maven-badges.herokuapp.com/maven-central/io.getstream.client/stream-java)
![](https://github.com/GetStream/stream-java/workflows/Java%20CI/badge.svg)

[stream-java](https://github.com/GetStream/stream-java) is a Java feed client for [Stream](https://getstream.io/). At the moment, there is no pure Java client for chat but you can find REST docs [here](https://getstream.io/chat/docs_rest/) and an Android specific implementation in Kotlin can be seen [here](https://github.com/GetStream/stream-chat-android-client).

You can sign up for a Stream account at https://getstream.io/get_started.

---

### Installation

Add the following dependency to your `pom.xml`:

```xml
<dependency>
    <groupId>io.getstream.client</groupId>
    <artifactId>stream-java</artifactId>
    <version>3.2.4</version>
</dependency>
```

or in your `build.gradle`:

```gradle
implementation 'io.getstream.client:stream-java:3.2.4'
```

In case you want to download the artifact and put it manually into your project,
you can download it from [here](https://github.com/GetStream/stream-java/releases).

Snapshots of the development version are available in [Sonatype](https://oss.sonatype.org/content/repositories/snapshots/io/getstream/client/) snapshots repository.

---

### JDK / JVM version requirements

This API Client project requires Java SE 7.

---

### FAQ

1. Is Android supported?

Yes. Use `client` for your backend and use `CloudClient` for your mobile application.

2. Cannot construct an instance of `io.getstream.core.models.*`, a model object in android. What is the problem?

If you're using proguard, ensure having following: `-keep class io.getstream.core.models.** { *; }`

Additionally, we're using Jackson JSON processor and see [their definitions](https://github.com/FasterXML/jackson-docs/wiki/JacksonOnAndroid) too unless you're already using it.

---

### Full documentation

Documentation for this Java client are available at the [Stream website](https://getstream.io/docs/?language=java).

For examples have a look [here](https://github.com/GetStream/stream-java/tree/master/example/Example.java).

Docs are available on [GetStream.io](https://getstream.io/docs/?language=java).

JavaDoc is available [here](https://getstream.github.io/stream-java/).

---

### Building & Testing

Run `gradlew test` to execute integration tests

---

### Copyright and License Information

Copyright (c) 2016-2020 Stream.io Inc, and individual contributors. All rights reserved.

See the file "LICENSE" for information on the history of this software, terms & conditions for usage, and a DISCLAIMER OF ALL WARRANTIES.
