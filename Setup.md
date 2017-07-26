
Create a new CentOS machine called "IoT" with a floating IP and disable SELinux.

https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-centos-7

As root, run the following:

yum install epel-release -y

yum install nodejs -y

yum install screen -y

yum update -y

Exit out of root and continue as a regular user (centos)

screen

cd ~/.node-red

npm install node-red-node-random

npm install node-red-node-mongodb

npm install node-red-node-pi-sense-hat-simulator

wget https://raw.githubusercontent.com/OpenStackSanDiego/IoT/master/flows_iot.json

node-red flows_iot.json

ctrl-a ctrl-d
