# swaggar-ts-sprint-boot
A swaggar blue print that produces typescript DTOs and client library together with Java DTOs and a Spring boot server from a single swaggar definition

# Usage
* Clone this project as a sub module of your main project.
```batch
cd myproject
git clone https://github.com/sparmboy/swaggar-ts-spring-boot.git api-definition
```
* Edit the ```api-definition/pom.xml``` to specify your ```groupId``` and ```projectId```(Be sure not to add hyphens to the artifactId as it effects the generated java package names)
* Modify the [swaggar.json](src/main/resources/swaggar.json) and associated schemas for your API definition
* When complete, ensure the ```api-definition``` gets run as part of your main projects build
```batch
mvn clean install
```

This will generate the typescript and java libraries ready to use in your project.

Good luck. We're all counting on you...

