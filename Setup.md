
Create a new CentOS machine called "IoT" with a floating IP.

As root, run the following:

yum install epel-release -y

yum install nodejs -y

yum update -y

Copy over the flows from git in /root/.node-red/flows_iot.json

node-red
