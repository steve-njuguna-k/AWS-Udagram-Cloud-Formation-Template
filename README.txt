Deploy a high-availability web app using CloudFormation

In this project, you’ll deploy web servers for a highly available web app using CloudFormation. You will write the code that creates and deploys the infrastructure and application for an Instagram-like app from the ground up.

Project URL:
------------
DNS URL - http://udagr-webap-4sw8xcsr3kqc-283533686.us-east-1.elb.amazonaws.com/

The files included are: 
-----------------------
create.sh - Shell script for creating a new CF Template
update.sh - Shell script for updating an existing CF Template
delete.sh - Shell script for deleting a CF Template

Infrastracture Diagram.jpg - Infrastracture Diagram for Udagram

udagram-network.yml - Template for deploying Udagram Network on AWS
udagram-network-parameters.json - Network Parameters for Udagram

udagram-server.yml - Template for deploying Udagram Servers on AWS
udagram-server-parameters.json - Server Parameters for Udagram

How To Run
----------
To create the network: .\create.sh UdagramNetwork udagram-network.yml udagram-network-parameters.json
To create the servers: .\create.sh UdagramServer udagram-server.yml udagram-server-parameters.json

To update the network: .\update.sh UdagramNetwork udagram-network.yml udagram-network-parameters.json
To update the servers: .\update.sh UdagramServer udagram-server.yml udagram-server-parameters.json

To create the network: .\delete.sh UdagramNetwork
To create the servers: .\delete.sh UdagramServer