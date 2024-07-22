# Micrometer Tracing Facade

[![Build Status](https://circleci.com/gh/micrometer-metrics/tracing.svg?style=shield)](https://circleci.com/gh/micrometer-metrics/tracing)
[![Apache 2.0](https://img.shields.io/github/license/micrometer-metrics/tracing.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Maven Central](https://img.shields.io/maven-central/v/io.micrometer/micrometer-tracing.svg)](https://search.maven.org/artifact/io.micrometer/micrometer-tracing)
[![Javadocs](https://www.javadoc.io/badge/io.micrometer/micrometer-tracing.svg)](https://www.javadoc.io/doc/io.micrometer/micrometer-tracing)
[![Revved up by Develocity](https://img.shields.io/badge/Revved%20up%20by-Develocity-06A0CE?logo=Gradle&labelColor=02303A)](https://ge.micrometer.io/)

* == application tracing facade

## Join the discussion

* [Micrometer Slack](https://slack.micrometer.io)
  * Problems:
    * Problem1: NOT active
      * Note: Asked [here](https://github.com/micrometer-metrics/micrometer/issues/4411#issuecomment-2243490216)

## Snapshot builds

* published to `repo.spring.io` / every successful build | `main` branch & maintenance branches
* Use

    ```groovy
    repositories {
        maven { url 'https://repo.spring.io/snapshot' }
    }
    
    dependencies {
        implementation 'io.micrometer:micrometer-tracing:latest.integration'
    }
    ```

## Milestone releases

* uses
  * testing purposes
    * NOT for production use 
* https://repo.spring.io/milestone
  * if you want to use milestone releases -> include it as a maven repository | your build configuration


## Documentation

* "/docs"
* [URL](https://docs.micrometer.io/tracing/reference/)

## Contributing

See our [Contributing Guide](CONTRIBUTING.md) for information about contributing to Micrometer Tracing.

## Code formatting

The [spring-javaformat plugin](https://github.com/spring-io/spring-javaformat) is configured to check and apply consistent formatting in the codebase through the build.
The `checkFormat` task checks the formatting as part of the `check` task.
Apply formatting with the `format` task.
You should rely on the formatting the `format` task applies instead of your IDE's configured formatting.

-------------------------------------
_Licensed under [Apache Software License 2.0](https://www.apache.org/licenses/LICENSE-2.0)_

_Sponsored by [VMware](https://tanzu.vmware.com)_
