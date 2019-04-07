# Docker
What is Docker?

<p>Before understand docker you need to understand hypervisor. What the heck? Hypervisor! I know hypervisor dude! Ok but this is for who don't know hypervisor. Imagine, You have a computer.You are using windows os. Your computer configuration is core i3, ram 4gb and harddisk space is 1tb. Now you want to use Linux for your OS lab assignment. How you solove this problem. You should use virtualbox or kvm or vagrant. In your vitualbox you install ubuntu 14.04 and you give 20gb space from 1tb your single hardware and you also share 2 gb ram or 1gb ram. see now virtualbox taking your single hardware resources. now you thought that you should use kali linux. so you need another virtualbox. again select resources from your single hardware resources.   </p>

## SO hypervisor is a program which is managing lots of os(windows, linux, mac) in your virtualbox and hypervisor uses your single hardware resources. 

![hypervisor](https://user-images.githubusercontent.com/33630256/55679144-f0cbde80-5927-11e9-92b3-39480d54a949.png)


### Now Docker?
![docker](https://user-images.githubusercontent.com/33630256/55680270-62f8ef00-5939-11e9-9e4e-46e325a0a580.png)

If you are using ubuntu then command ls / . You wll see bin dev lib64 sys and so on. Docker creates tunnel with our os. Using our os resources. Imagine we have a node js application and another php application. So we need to run this application in two seperate server in serperate conatiners. In docker we have containers. In containers we save node, php, django application and 
running separately. That's the difference between hypervisor and Docker. 

## How to set up docker in Linux?
<p>how to install docker ubuntu 18.04 </p>

