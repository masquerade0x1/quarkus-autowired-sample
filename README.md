```
$ mvn quarkus:dev
[INFO] Scanning for projects...
[INFO] 
[INFO] ---------------------< org.acme:code-with-quarkus >---------------------
[INFO] Building code-with-quarkus 1.0.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- quarkus-maven-plugin:2.10.1.Final:dev (default-cli) @ code-with-quarkus ---
[INFO] Invoking org.apache.maven.plugins:maven-resources-plugin:2.6:resources) @ code-with-quarkus
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 2 resources
[INFO] Invoking io.quarkus.platform:quarkus-maven-plugin:2.10.1.Final:generate-code) @ code-with-quarkus
[INFO] Invoking org.apache.maven.plugins:maven-compiler-plugin:3.8.1:compile) @ code-with-quarkus
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /home/username/playground/quarkus-autowired-sample/target/classes
[INFO] Invoking org.apache.maven.plugins:maven-resources-plugin:2.6:testResources) @ code-with-quarkus
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/username/playground/quarkus-autowired-sample/src/test/resources
[INFO] Invoking io.quarkus.platform:quarkus-maven-plugin:2.10.1.Final:generate-code-tests) @ code-with-quarkus
[INFO] Invoking org.apache.maven.plugins:maven-compiler-plugin:3.8.1:testCompile) @ code-with-quarkus
[INFO] Changes detected - recompiling the module!
Listening for transport dt_socket at address: 5005
2022-07-06 21:45:25,657 INFO  [io.qua.dep.dev.IsolatedDevModeMain] (main) Attempting to start live reload endpoint to recover from previous Quarkus startup failure
2022-07-06 21:45:25,751 INFO  [org.jbo.threads] (main) JBoss Threads version 3.4.2.Final
2022-07-06 21:45:25,902 ERROR [io.qua.dep.dev.IsolatedDevModeMain] (main) Failed to start quarkus: java.lang.RuntimeException: io.quarkus.builder.BuildException: Build failure: Build failed due to errors
        [error]: Build step io.quarkus.arc.deployment.ArcProcessor#validate threw an exception: javax.enterprise.inject.spi.DeploymentException: javax.enterprise.inject.UnsatisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]

















Caused by: javax.enterprise.inject.UnsatisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]                                 

















Caused by: io.quarkus.builder.BuildException: Build failure: Build failed due to errors                                                                                     
atisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]                                                                       

















Caused by: javax.enterprise.inject.UnsatisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]                                 












Caused by: javax.enterprise.inject.spi.DeploymentException: javax.enterprise.inject.UnsatisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]                                                                                                                                                            

















Caused by: javax.enterprise.inject.UnsatisfiedResolutionException: Unsatisfied dependency for type org.acme.Utils and qualifiers [@Default]                                 


        at io.quarkus.arc.processor.Beans.resolveInjectionPoint(Beans.java:411)
        at io.quarkus.arc.processor.BeanInfo.init(BeanInfo.java:532)
        at io.quarkus.arc.processor.BeanDeployment.init(BeanDeployment.java:263)
        ..re13 mo


```