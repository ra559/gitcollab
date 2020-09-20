![Markdown Logo](DockerLogo.png)
# What is Docker ? 

Docker is an open platform for developing, shipping, and running applications. Meaning that developers or system adminstrators are able to: 

* Increase responsive deployment and scaling 
* Develop applications and its supporting components utilizing containers.
* Separate applications from infrastructure so they can deliver software quickly. 
* Deploy an application into the production enviroment where the application can be a container or service. 
  
 ## Note: 
 Nothing beats reading the manual. So if you want to, Docker documentation can be found here: https://docs.docker.com/get-started/overview/
 
 ## Installing Docker 
 Before you install Docker Engine for the first time on a new host machine, you need to set up the Docker repository. 
 
 ### Installation using download
 * Windows: 
 ```
    Download from here: https://hub.docker.com/editions/community/docker-ce-desktop-windows/
```  
  * Mac: 
```
   Download from here: https://hub.docker.com/editions/community/docker-ce-desktop-mac/
```

 ### Installation using repository
  * Linux: 
```
     CentOs
 
        1. sudo yum install -y yum-utils

        2. sudo yum-config-manager \
          --add-repo \
          https://download.docker.com/linux/centos/docker-ce.repo

     Debian & Raspbian 

        1. sudo apt-get update 

        2. sudo apt-get install \
              apt-transport-https \
              ca-certificates \
              curl \
              gnupg-agent \
              software-properties-common
    
     Fedora
        1. sudo dnf -y install dnf-plugins-core
        2. sudo dnf config-manager \
              --add-repo \
              https://download.docker.com/linux/fedora/docker-ce.repo
    
   * Ubuntu
   
      * sudo apt-get update
      * sudo apt-get install \
           apt-transport-https \
           ca-certificates \
           curl \
           gnupg-agent \
           software-properties-common