# Altschool Cloud Engineering Second Semester Project-Exam
## Documentation
This documentation explains the provisioning of two Ubuntu-based servers, named “Master” and “Slave”, using Vagrant. This script automated the deployment of a LAMP stack and cloned a PHP application from Github using both the master and slave nodes.
Below are the processes in more details.
##  Provisioning of two Ubuntu-based servers, named “Master” and “Slave”, using Vagrant
I created a directory for this poject, then 'vagrant init' to initialize a vagant file into it and to configure the vagrant file. After that, I was able to 'vagrant up' my master and slave nodes. See the image below; 
![exam image 1](https://github.com/NifemiLoveth/altschool_cloud_exam/assets/152023802/73abe77f-8911-430c-8ccf-25fcd9f00912)

## Creation of bash script to deploy lamp stack
On the master node, I created a bash script to automate the deployment of a LAMP (Linux, Apache, MySQL, PHP) stack. This script  clone a PHP application from GitHub, installed all necessary packages, and configure Apache web server and MySQL. Through it, I was able to view the cloned Github laravel page. See it below;
![laravel screenshot](https://github.com/NifemiLoveth/altschool_cloud_exam/assets/152023802/505fd55e-fcd5-463f-b3fd-e8ec94a3e48a)

## Installation of Ansible and SSH connection of master to slave
On the master node, i installed Ansible and all its necessary packages. I also generated ssh keys so i can ssh directly into my slave node. After that, i ran the ping command to ensure that the connection was a success.
![exam image](https://github.com/NifemiLoveth/altschool_cloud_exam/assets/152023802/f09c80c3-4e6f-44ca-8ed9-1b728718e31c)

## Creation of ansible playbook to execute bash script on Slave node
Thereafter, I created a playbook to execute the bash scipt on the slave node and set up a cron job to check the server's uptime every 12am and also verified that the PHP application is accessible through the VM's IP address. See evidence below;
![play success](https://github.com/NifemiLoveth/altschool_cloud_exam/assets/152023802/af2f9829-3185-4dbc-a6b9-922d12d971d3)

## Test on Slave Ip
I put in my slave node's IP address into a chrome browser and the laravel page was displayed which indicates a successful project. Image is below.
![exam screenshot 3](https://github.com/NifemiLoveth/altschool_cloud_exam/assets/152023802/0ffc3e75-7dea-45e8-a562-a21c57d0c9cb)

# Thank you for reading!
