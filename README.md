# Docker
## What is Docker?

<p>Before understand docker you need to understand hypervisor. What the heck? Hypervisor! I know hypervisor dude! Ok but this is for who don't know hypervisor. Imagine, You have a computer.You are using windows os. Your computer configuration is core i3, ram 4gb and harddisk space is 1tb. Now you want to use Linux for your OS lab assignment. How you solove this problem. You should use virtualbox or kvm or vagrant. In your vitualbox you install ubuntu 14.04 and you give 20gb space from 1tb your single hardware and you also share 2 gb ram or 1gb ram. see now virtualbox taking your single hardware resources. now you thought that you should use kali linux. so you need another virtualbox. again select resources from your single hardware resources.   </p>

## SO hypervisor is a program which is managing lots of os(windows, linux, mac) in your virtualbox and hypervisor uses your single hardware resources. 

![hypervisor](https://user-images.githubusercontent.com/33630256/55679144-f0cbde80-5927-11e9-92b3-39480d54a949.png)


### Now Docker?
![docker](https://user-images.githubusercontent.com/33630256/55680270-62f8ef00-5939-11e9-9e4e-46e325a0a580.png)

If you are using ubuntu then command ls / . You wll see bin dev lib64 sys and so on. Docker creates tunnel with our os. Using our os resources. Imagine we have a node js application and another php application. So we need to run this application in two seperate server in serperate conatiners. In docker we have containers. In containers we save node, php, django application and 
running separately. That's the difference between hypervisor and Docker. 

## How to set up docker in Linux?
<p>how to install docker ubuntu 18.04 </p>

`sudo apt update`

`sudo apt install apt-transport-https ca-certificates curl software-properties-common`

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"`

`sudo apt update`

`apt-cache policy docker-ce`

`sudo apt install docker-ce`

`sudo systemctl status docker`

## Executing the Docker Command Without Sudo 

`sudo usermod -aG docker ${USER}`

`su - ${USER}`

`id -nG`

In username you use a name from id -nG command gives you.

`sudo usermod -aG docker username`

`docker`

`docker info`

`docker version`

Docker has a images. In Images you have lots of containers. suppose you want to use apache. Then use this command 

`docker container run -d -p 8081:80 --name myapache httpd`

check this on your computer localhost:8081 typing

here -d means detach 
-p port 
myapache is a container name 
httpd - image

Now You want to use nginx server. So you need another containers. Use this command 

`docker container -d -p 8080:81 --name mynginx nginx`

this nginx running on 81.
check this on your computer localhost:8080 typing

run this command to see your current running containers:

`docker ps`

Stop docker cotainer 

`docker container stop mysqldb`

remove particular docker image 

` docker container rm mysqldb -f`

remove all containers

`docker rm $(docker ps -aq) -f`

`docker container ls`



Nodejs Dockerize 

`mkdir node_project`
`cd node_project`
`code .`
`open the terminal vs code`
`npm init`
`npm install express --save`

https://nodejs.org/de/docs/guides/nodejs-docker-webapp/
