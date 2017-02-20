
The Internet of Things (IoT) consists of IP (network) connected devices that perform repetitive actions and communication with other network devices. In this workshop, you'll be setting up some IoT devices to perform various actions.

First off, your team is going to need a name and a Twitter account. Pick a name and create a Twitter account at www.twitter.com. Your IoT devices will be posting messages to this Twitter account so you can keep track of what they are doing.

* Send a Tweet with the tag "#SanDiegoIoT" once your account is created!

One easy way to setup IoT devices is with node-red (www.nodered.org), a visual for wiring the Internet of Things. Through this visual interface, an IoT device and be setup to run a complete workflow. Each group will be assigned a pool of IoT devices to use.

At the following etherpad, type in your team name next to an OpenStack user account name. This is just to keep track of who is using which OpenStack account. The password for the account is on the whiteboard.

https://etherpad.openstack.org/p/san-diego-iot

Use the login above (teamXX) to log into the cloud console at:

http://cloud.openstacksandiego.org

Start up your first IoT instance!

* Project->Compute->Instance->"Launch Instance"
* Instance Name = "IoT"
* Count = 1
* Source = "iot-node-red"
* Flavor = "m1.small"
* Take note of the IP address of your new IoT instance

You'll need to open the firewall to get access to the IoT device. The IoT device console runs on TCP port 1880.

* Project->Compute->Access & Security->"Manage Rules"
* +Add Rule
* Defaults: Custom TCP/Ingress/Port (no need to change these)
* Port: 1880
* Add

Pull up the IoT console and let's setup the IoT device! Replace XXX with your IP address.

* Open a web browser to http://147.75.64.XXX:1880/

You should now see the IoT console.

There are a number of sensors already online and ready to go. These include some temperature, voltage, and a camera. Double click on the README to get the details on each workflow and things to setup in each workflow.

* Sensor Sample - read and alert on temperature and voltage changes.
* Twitter Alerting - automatically post on Twitter
* Camera - grab images from a camera and post them to Twitter
* Web Service - make services available on the Internet and have another device use the service
* Database - save and retrieve data to/from a database


