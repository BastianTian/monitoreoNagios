# MonitoreoNagios
## Installation
1. First we are going to need running our Virtual Machines, for that we use in directory root were we have the Vagrantfile the next command, it will take an average of 1 hour and half to install all the dependencies

`vagrant up`

2. After run the Virtual Machines we are going to access to the Nagios virtual machine, for that we use the next command

## Using project
`vagrant ssh nagios`

3. After access to the Nagios virtual machine we assert that the nagios service is running using the next command

`service nagios status`

4. Then we are going to use our ip of the Nagios virtual machine and use it in our internet navigator, if you dont have the ip of the Nagios virtual machine you can use the next command to get the ip of the Nagios virtual machine

`ifconfig`

5. In the navigator we should have a page like this one
![image1!](imagesReadme/image1.png)

6. We'll have to set the initial configuration for nagios
![image2!](imagesReadme/image2.png)
![image3!](imagesReadme/image3.png)

7. After that we are going to login in the Nagios page
![image4!](imagesReadme/image4.png)

8. It will ask us to accept the terms of servie
9. The we will have a home dashboard for Nagios like the following one
![image5!](imagesReadme/image5.png)

 we are goin to click en the navigator bar in 'Dashboards', then we're goin to be able to see our nagios virtual machine statistics
![image6!](imagesReadme/image6.png)
## Monitoring the Clients virtual machines with our Nagios virtual machine

10. Firt we'll need add the virtual machine that we want to monitor, for that in the navigation bar we go to the configure section and then go to the deploy section
![image7!](imagesReadme/image7.png)

11. After that we are going to config and set the connection to the client virtual machine that we're adding
![image8!](imagesReadme/image8.png)
if we set right the connection to the client virtual machine the we'll have the next response
![image9!](imagesReadme/image9.png)
