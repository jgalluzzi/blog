# blog

Banging my head around AWS in the start of a new home lab. 

Just spent 20 minutes trying tp download a .deb via curl with bad info on how to do it from Bing AI.

I was trying
```
  curl https://github.com/arkime/arkime/releases/download/v5.2.0/arkime_5.2.0-1.ubuntu2204_amd64.deb
vs
  curl -O -k -L https://github.com/arkime/arkime/releases/download/v5.2.0/arkime_5.2.0-1.ubuntu2204_amd64.deb
```

<img width="383" alt="image" src="https://github.com/jgalluzzi/blog/assets/46066804/c1c65eaa-c4ce-4b2c-be6a-51631c7f0802">

<img width="889" alt="image" src="https://github.com/jgalluzzi/blog/assets/46066804/c169859e-3c25-4480-8891-201cb80b2d4a">


Now I'm on debian trying to get opensearch to install. Its fucked. It won't install or uninstall or start the service. 
Do I try elastichsearch instead?

![image](https://github.com/jgalluzzi/blog/assets/46066804/60fe911a-8d69-4379-8a7a-f42f4a5f9cb4)

Got Elasticsearch install after rebuilding for ubuntu 22 and armine installed. But now elasticsearch isn't working.

I spent the whole evening trying to get Arkmie to work. Backlog.

arkmie https://arkime.com/index#home

## The Redirect

I sought to redirect help.jgalluzzi.blog to this blog
I googled, I read.
Nginx was installed on a new EC2 instance, bodies on the floor of terminated instances and failed exercises.

How to restart nginx
nginx redirect web

I kept adjusting the nginx config to no avail

Later I found out I screwed up the security group and nothing was getting to the instance. Fuck. I hadn't properly associated the correct security group.
You need to add the security group and click save, not just select it. Cool.
<img width="293" alt="image" src="https://github.com/jgalluzzi/blog/assets/46066804/a1848e06-2982-49f8-a50a-f0f66c7f7e11">


