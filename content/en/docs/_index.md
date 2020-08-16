
---
title: "Documentation"
linkTitle: "Documentation"
weight: 20
menu:
  main:
    weight: 20
---

{{% alert title="Warning" color="warning" %}}
These pages are currently in beta, please be patient!
{{% /alert %}}

This documentation will covers the different libraries in existence and show how you can interact with them.

The first thing you should do is create a new project in a folder by doing `gradle init` (if you don't know how, refer to 
[this guide](https://gradle.org/install/)).

Then you add those lines in your build.gradle:

```groovy
repositories {
	mavenCentral()
	maven {
		url "https://jitpack.io"
	}
}
dependencies {
	implementation 'com.github.KaptainWutax:SEED:c540b5224dbb4dc80fe8a25bfcfcf9383f635a0c'
}
```


