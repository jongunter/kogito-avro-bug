# kogito-avro-bug Project
This repo is a demo of an issue I've been experiencing between the Maven Avro plugin and Quarkus.

## Description of issue
When creating a BPMN process in Kogito, code generation fails with certain settings in the Avro Mavn plugin. 
The error is super cryptic: `java.lang.IllegalArgumentException: Cannot find method lambda$process$0[] on class...`

## Branches
- `main` - broken example
- `working` - working process with message node but no Avro Maven Plugin
- `working1` - working process with Avro Maven plugin but no message node
- `working2` - working process with message node but no Avro maven plugin
- `working3` - working process with message node and Avro maven plugin, but plugin output directory set differnetly

## Running the application

You can run your application in dev mode that enables live coding using:
```shell script
./mvnw compile quarkus:dev
```
