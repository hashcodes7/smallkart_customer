### first get the permission to use mvnw command
``` bash
chmod +x mvnw
```
run these to check your maven and java versions
``` bash
java -version
mvn -version
./mvnw -version
```

expected result : just quick look through yours and dont compare line by line 
``` bash
openjdk version "17.0.20" 2026-07-21 LTS
OpenJDK Runtime Environment Microsoft-14670383 (build 17.0.20+8-LTS)
OpenJDK 64-Bit Server VM Microsoft-14670383 (build 17.0.20+8-LTS, mixed mode, sharing)
bash: mvn: command not found
Apache Maven 3.9.16 (2bdd9fddda4b155ebf8000e807eb73fd829a51d5)
Maven home: /home/vscode/.m2/wrapper/dists/apache-maven-3.9.16/56ba1f9f
Java version: 17.0.20, vendor: Microsoft, runtime: /usr/local/sdkman/candidates/java/17.0.20-ms
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "6.8.0-1052-azure", arch: "amd64", family: "unix"
```


once all is verified run this command to build jar file
``` bash
./mvnw clean package -DskipTests
```

### output
once jar is built you will see the jar file in target folder something like this 
![[Pasted image 20260815115948.png|242]]