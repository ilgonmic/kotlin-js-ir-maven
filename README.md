# kotlin-js-ir-maven
Pretty easy sample to setup Kotlin/JS IR in Maven

The main problem of using IR in maven that IR uses `klib` as artifacts instead of JAR, because all libraries are published with transitive dependencies with "default" type (which is jar)
But Gradle has Variant Aware Resolution, Maven has not such feature.

So here it is plugin which register custom artifact types. And then it can be used during compilation

## How to build
1. `cd custom-maven-plugin`
2. `mvn install`
3. `cd ..`
3. `mvn compile`
