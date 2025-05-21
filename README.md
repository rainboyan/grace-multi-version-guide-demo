[![Main branch build status](https://github.com/rainboyan/grace-multi-version-guide-demo/workflows/Grace%20CI/badge.svg?style=flat)](https://github.com/rainboyan/grace-multi-version-guide-demo/actions?query=workflow%3A%Grace+CI%22)

# Grace Multi-version Guide Demo

This is a demo for publishing guide to GitHub Pages.

## Grace Version

- Grace **2023.0.0**

## Usage

Apply `grace-doc` plugin to your `build.gradle`,

```groovy
apply plugin: "org.graceframework.grace-doc"

repositories {
    mavenCentral()
    maven {
        url "https://s01.oss.sonatype.org/content/repositories/snapshots/"
        mavenContent {
            snapshotsOnly()
        }
    }
}

dependencies {
    implementation "org.graceframework:grace-boot"
}
```

## Links

- [Grace Framework](https://github.com/graceframework/grace-framework)
- [Grace Plugins](https://github.com/grace-plugins)
