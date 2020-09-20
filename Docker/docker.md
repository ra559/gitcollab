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
 * Windows: 
    * Download from here: https://hub.docker.com/editions/community/docker-ce-desktop-windows/
    
  * Mac: 
    * Download from here: https://hub.docker.com/editions/community/docker-ce-desktop-mac/
    
  * Linux: 
    * CentOs 
        * sudo yum install -y yum-utils
        * sudo yum-config-manager \
          --add-repo \
          https://download.docker.com/linux/centos/docker-ce.repo
          
    * Debian 
        * sudo apt-get update
         * sudo apt-get install \
              apt-transport-https \
              ca-certificates \
              curl \
              gnupg-agent \
              software-properties-common
    
    * Fedora
        * sudo dnf -y install dnf-plugins-core
        * sudo dnf config-manager \
              --add-repo \
              https://download.docker.com/linux/fedora/docker-ce.repo