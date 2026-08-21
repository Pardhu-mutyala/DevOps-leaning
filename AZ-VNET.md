----------------------------------------------VIRTUAL NETWORK (VNET) -----------------------------------------------

Why Azure come up with VNET concept in AZure?

Take an example of Two devops engineers in different regions, wants to two create two VMs, created in two differents regions but availble in same zone.
if one machine is got affected by an hacker can access everythinhg all other VMs  on that machine.

By using VNETs we can create your own network and protect your data by using some rules init.

In your VNET we can deploy different type of services like Web apps, business logic application and DBs, customers like outsiders does't have permissions for DBs through SSH.

we can split the network into subnets and secure the services based on the requirements.

NSG(Network security group) --> Adding security to you network based on the requirements.

 ASG(Application security group):- It enhances the capabilities of NSG.
 In real world we use both ASG+NSG

 