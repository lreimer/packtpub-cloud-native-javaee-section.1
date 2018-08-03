# Cloud-native Application Development with Java EE

## Video 1.4: Getting started with Java EE 8 microservices

- Build and dependency setup for Maven
- Build and dependency setup for Gradle
- Basic project setup and structure
- Implement simple webservice with REST endpoint
- Local deployment with Payara 5

## Video 1.5: Containerizing Java EE 8 microservices

- Building Docker images for Java EE 8 with Payara Micro 5
- Running containerized Java EE 8 microservices locally
- Using multi-stage Docker builds for Java EE 8 microservices
- Tuning the JVM to run a containerized environment 

``` 
ENTRYPOINT ["java", "-server", "-XX:+UnlockExperimentalVMOptions", "-XX:+UseCGroupMemoryLimitForHeap", "-XX:MaxRAMFraction=3", "-XX:ThreadStackSize=256", "-XX:MaxMetaspaceSize=128m", "-XX:+UseG1GC", "-XX:ParallelGCThreads=2", "-XX:CICompilerCount=2", "-XX:+UseStringDeduplication", "-jar", "/opt/payara/payara-micro.jar"]
CMD ["--deploymentDir", "/opt/payara/deployments"]
```
