Containers are a virtualization environment. Just like running multiple VMs on a single physical host, you can run multiple containers on a single physical or virtual host. 
Containers are designed to be created, scaled out and stopped dynamically. 
Containers help respond to changes on demand and restart quickly after crash.
Ex - Docker. Azure supports Docker.


**VMs vs Containers** - 
VMs can only run one OS at a time. so different resources that require diff OS require more VMs to be created.
VMs are like real computer. so they take more time to start up.
VMs virtualize the hardware while containers virtualize the OS
Container bundles a app and its dependencies and deploys it as a unit to the container host. The container host provides a standardized runtime environment.  
Can run multiple containers in a single host with complete isolation.
Containers can be orchestrated with container cluster orchestration. 


**Azure Container Instances** - 
PaaS offering of Azure. Fastest and simplest way to run a container in Azure. Upload container and the service runs them. 

**Azure Container Apps** - 
PaaS offering. Container apps include built in load balancing and scaling. Basically allows for operations around a containerized app. while container instance just runs the container. 

**Azur Kubernetes Service** - 
Container Orchestration Service. This manages lifecycle of the containers. 

![[Pasted image 20260923004801.png]]


Containers are often used to create solutions that use microservice architecture. 