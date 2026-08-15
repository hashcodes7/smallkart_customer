### Coz company pc i will use codespaces
![[Pasted image 20260815030310.png|586]]

### set up codespaces jdk 
![[Pasted image 20260815115105.png]]

### inside there use this confg so codespaces has jdk17 + docker both
``` json
{
  "name": "Java 17 & Docker Environment",
  "image": "mcr.microsoft.com/devcontainers/base:ubuntu",
  "features": {
    "ghcr.io/devcontainers/features/java:1": {
      "version": "17",
      "installMaven": "true",
      "installGradle": "true"
    },
    "ghcr.io/devcontainers/features/docker-in-docker:2": {
      "version": "latest",
      "enableMoby": "true"
    }
  },
  "customizations": {
    "vscode": {
      "extensions": [
        "vscjava.vscode-java-pack",
        "ms-azuretools.vscode-docker"
      ]
    }
  }
}
```

### Then start your codespaces
![[Pasted image 20260815030501.png|279]]

### here you will be presented with a vscode like interface
![[Pasted image 20260815030555.png]]

we did this because we want to run docker, maven java etc commands which might not get installed in cognizant laptop
