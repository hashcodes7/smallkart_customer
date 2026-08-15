we have 2 spring projects so we are making 2 repositories , one for each. 

https://github.com/hashcodes7/smallkart_admin.git
https://github.com/hashcodes7/smallkart_customer.git

next we just run this command
``` bash
git init
```


then we connect it to our online github repo
``` bash
git remote add origin https://github.com/hashcodes7/smallkart_admin.git
```

verify
``` bash
git remote -v
```

expected result -
```
origin  https://github.com/hashcodes7/bigkart.git (fetch)
origin  https://github.com/hashcodes7/bigkart.git (push)
```

next we just go to left side source control and simply do commit and push

it will say
![[Pasted image 20260815025248.png]]

just select ok and create a remote branch
if authentication is asked just authenticate and it will be pushed.