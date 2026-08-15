A dockerFile which tells your system about how it should make the image, which jdk, which Linux os and everything it should use.

just quickly create it using touch command inside your codespaces itself
```
touch Dockerfile
```
![[Pasted image 20260815120337.png]]

once done you will see a dockerfile built right in your project sidebar.

open that empty file and paste all this command there
``` dockerfile
FROM eclipse-temurin:17-jre

WORKDIR /app

COPY target/bigkart-0.0.1-SNAPSHOT.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
```
save and close this file.

to check what each command does check this file [[4.1 (Optional) Understanding DockerFile Commands]]