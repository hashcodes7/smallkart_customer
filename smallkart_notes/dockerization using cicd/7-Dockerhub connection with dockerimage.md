## Here we will generate Dockerhub PAT, and put it in Github Secrets
(you will not need this step in case you are doing manual deployment)

next we need a personal access t0ken along with our username to push into docker repo
![[Pasted image 20260815134443.png]]

and now click personal t0ken and create one
![[Pasted image 20260815134543.png]]

![[Pasted image 20260815134615.png]]

This will give us the docker repo t0ken something like this
![[Pasted image 20260815155751.png]]

take this t0ken and put it in github secrets
- go to github repo -> security
![[Pasted image 20260815134954.png]]

- scroll down to secrets and variables and click github action 
- ![[Pasted image 20260815135247.png]]
- create secret like this
- ![[Pasted image 20260815135340.png|283]]
 ![[Pasted image 20260815135429.png]]

| Secret key           | Value                           |
| -------------------- | ------------------------------- |
| `DOCKERHUB_USERNAME` | `hashcodes7`                    |
| `DOCKERHUB_TOKEN`    | Your Docker Hub PAT (above pic) |
next we can use them in our cicd pipeline

once your cicd pipeline pushes code you willget it automatically like this 
![[Pasted image 20260815135902.png]]