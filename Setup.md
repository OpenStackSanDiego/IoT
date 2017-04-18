
Create a new CentOS machine called "IoT" with a floating IP.

As root, run the following:

yum install epel-release -y

yum install nodejs -y

yum install screen -y

yum update -y

Copy over the flows from git in /root/.node-red/flows_iot.json

screen

npm install node-red-node-random

npm install node-red-node-mongodb

node-red

ctrl-a ctrl-d
