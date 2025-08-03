Virtual Machine Scale Set - VMSS

old we have physical servers and deploy the application on the ser vers as we need.
whe Virtualisation comes, we installa hypervisor it logically divide the server with some logically portions to increase the usage the efficiency of resource usages.

Azure manges the Data centres to deploy yhr resource when they get the request.

Ex:- if some one from the our teams needs an VM to deploy for the client then you logged in the Azure portal and then we create a VM as the client requirements.

Creation of Virtual machine in Azure cloud by using AZure (GUI) portal 

1. Navigate to Azure portal --> portal.azure.com
2. serch for Virtal machine the search bar on the top section
![alt text](image.png)
see the above pictue and see the options we need to give

we need to provide fields which having * marks

  . Resource group -- > It accumualtes all of your resource when you want to create for a particular operations are anything. It binds all the resource in one group togethere like a family.

  .region -->  we need to select the regions provided by the Azure. Select the region where the operation are near the place.
               eg:- if you client is from USA in atlanta, we need to select the region based upon that we need ti+o select the region

  .Zones --> these are like Data centres, you need to select based upon your requirements, it creates the vm on that data centres

  .image --> it is the main part in the billing process, based on the Image selection the cost of VM will be there

  .Size --> This is also another important facor for billing incurr. In we will select the vCpus and RAM based on your requirements.

  for linux machine we can login via SSH keys
  or we can use Password type login

Simple task to --> installing jenkis in the VM

jenkins is java dependency application

steps or cmds


suod apt-get update
sudo apt-get install openjsk-11-jre

check --> java --version

we need to install Jenkins by using the below command

curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins

we need 8080 port to open and create a Inbound role to open 8080 to access the traffic in NSG in virtual network settings

VMSS --> It is a Auto scale the VMs abased upon the traffic for the VM gets, not only that we can set any threshold based o0n that a new one will add if the load is down it is automatically down the VM.