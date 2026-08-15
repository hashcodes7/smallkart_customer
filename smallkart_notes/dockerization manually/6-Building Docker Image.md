lets say you created docker account and a repo, using [[5-creating dockerhub account & Repo]]
your full repo reference is `hashcodes7/smallkart_customer:latest`

Running this command in terminal makes a docker image from docker file. 
```
docker build -t hashcodes7/smallkart_customer:latest .
```

- docker build - builds an image
- -t bigkart - name of the image we waant
- repo reference `hashcodes7/smallkart_customer:latest` we put so Docker Hub knows where to push it. its optional while building image.
- . full stop in end means- take the full project and make this image

the output looks like this
![[Pasted image 20260815160335.png]]

the docker image is created and is stored inside a hidden place in system

to see how we test docker image in a codespace before we actually push on docker hub check 
[[6.1 (optional) testing docker image locally before deploying]]

to directly move to deplyment go to [[7-Logging in to DockerHub]]

