
Create a new CentOS machine called "IoT" with a floating IP and disable SELinux.

https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-centos-7

As root, run the following:

yum install epel-release -y

yum install nodejs -y

yum install screen -y

yum update -y

Copy over the flows from git into /root/.node-red/

screen

npm install node-red-node-random

npm install node-red-node-mongodb

node-red

ctrl-a ctrl-d
