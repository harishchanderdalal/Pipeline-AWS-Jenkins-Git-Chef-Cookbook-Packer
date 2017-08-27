# WorkFlow
![vagrant aws chef jenkins](https://user-images.githubusercontent.com/22466745/29718668-2b304188-89d1-11e7-870e-dec94211b5f8.png)

# Level 1
- Local vagrant + aws plugins
#### https://github.com/harishchanderdalal/vagrantJenkins.git
```
    Launch Ec2 Instance with Jenkins
    URL - Ec2 Ip:8080
```
# Level 2
- How to Create Jenkins Pipeline Job for Spring Boot
```
1. Select New Item
2. Job Type PIPELINE

- Repositroy URL = https://github.com/harishchanderdalal/pocAgility.git
```
- Configure Pipline Job
![pipeline configure](https://user-images.githubusercontent.com/22466745/29747587-08329aee-8b1d-11e7-9229-816f938ed82f.png)

- Build Job
![spring build](https://user-images.githubusercontent.com/22466745/29747684-bb0281a0-8b1f-11e7-94ce-d51af69db713.png)

- Sping UI
- Jenkins IP:9000
![spring 9000](https://user-images.githubusercontent.com/22466745/29747690-fc11944c-8b1f-11e7-8c32-fa54b65cedce.png)

#### https://github.com/harishchanderdalal/spring-petclinic.git
```
    Spring Framework Build as Service and Launch
    URL - Ec2 IP:9000
```
# Level 3
- Install Chef Server on Ec2
#### https://github.com/harishchanderdalal/chef.git
```
    Configure Chef Server 
    Cookbook on Chef Server
```
# Level 4
- Packer AMI Creation
#### https://github.com/harishchanderdalal/packerChef.git
```
    Ec2 Use AMI will add that node under Chef Server
```
