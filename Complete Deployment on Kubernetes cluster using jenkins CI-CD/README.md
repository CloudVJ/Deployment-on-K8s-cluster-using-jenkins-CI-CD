<div align="center">

## Complete Deployment on Kubernetes cluster using jenkins CI-CD

![197373162-1f510766-4437-41ba-b6f8-deead93c7693](https://user-images.githubusercontent.com/58173938/197495878-0be968d0-2c33-4c26-b6fb-5a20b825c646.png)

</div>

We will see how jenkins transfer the files, also will see another job of ansible is to run the 
playbook principle so what are the files are going to run here is a `service.yaml` 
file and also a `deployment.yaml` file and kubernetes fetch the latest image 
from the docker registry and based on that it will start building a container 
also we have a service file so that container will be accessible to us using 
the terminal along with the node port we are going to expose 

I posted some of the troubleshoot scenerios which i have gone through on the [reddit](https://www.reddit.com/user/Mohanse7)

### Select the ansible public ip address and do ssh to the server via putty

![1-copy the ansible public ip address for ssh to the server](https://user-images.githubusercontent.com/58173938/197496057-5928e3fd-6a9d-42fb-bc6e-e38248031e1b.png)

### Select the webapp-server(k8s cluster) and do ssh to the server via putty

![2- copy the webapp-server(k8s cluster) for ssh to the server](https://user-images.githubusercontent.com/58173938/197496329-a5e59924-728c-4af2-aad1-ae2d57e42ab6.png)
 
### Now we have logged into the 2 servers right one is ansible and left one is webapp-server(k8s cluster)

![3- now we have logged into the 2 servers right one is ansible and left one is webapp-server(k8s cluster)](https://user-images.githubusercontent.com/58173938/197496413-248dee66-e90c-4703-ac65-844f083a1847.png)

### Set the root password in the webapp(k8s cluster) server

![4- set the root password in the webapp(k8s cluster) server](https://user-images.githubusercontent.com/58173938/197496499-8eef533a-718b-41a3-948c-16be6f431a01.png)

### Open sshconfig file we do this to allow network permissions

![5- open sshconfig file we do this to allow network permissions](https://user-images.githubusercontent.com/58173938/197496657-4604368b-b03d-4ca2-9b7d-002447aa496b.png)

