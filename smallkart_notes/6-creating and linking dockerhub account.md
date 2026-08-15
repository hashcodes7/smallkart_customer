- go to hub.docker.com
- make a account, set a username , choose free plan
- click create repository

![[Pasted image 20260815133804.png]]

after creating it will look like this
![[Pasted image 20260815134031.png]]

as it appears the repo is `hashcodes7/smallkart_customer`
so the docker image name should be `hashcodes7/smallkart_customer:latest`
it has to be compatible

next we need a personal access t0ken along with our username to push into docker repo
![[Pasted image 20260815134443.png]]

and now click personal t0ken and create one
![[Pasted image 20260815134543.png]]

![[Pasted image 20260815134615.png]]


This will give us the docker repo t0ken.

take this t0ken and put it in github secrets
- go to security
![[Pasted image 20260815134954.png]]

- scroll down to secrets and variables and click github action 
- ![[Pasted image 20260815135247.png]]
- create secret like this
- ![[Pasted image 20260815135340.png|283]]
 ![[Pasted image 20260815135429.png]]

### so we added 2 secrets

`DOCKERHUB_USERNAME

`hashcodes7

and:

`DOCKERHUB_T0KEN

`cant write that see img


next we can use them in our cicd pipeline


once your cicd pipeline pushes code you willget it automatically like this 
![[Pasted image 20260815135902.png]]



