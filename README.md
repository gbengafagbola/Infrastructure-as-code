http://udagr-webap-akcgwi4s9v8v-26657472.us-east-1.elb.amazonaws.com/

## Infrastructure as Code - Designing Implementing/provisioning the required infrastructure for an Application

This folder provides contains the following folders:

1. Diagram: - which is a visual aid to understand the CloudFormation script.
2. Script: - interpret the instructions and create a matching CloudFormation script.

### Dependencies
##### 1. AWS account
You would require to have an AWS account to build the cloud infrastructure.

##### 2. Editor
You can get VS Code editor, which is gret for indentation outline [here](https://code.visualstudio.com/download).

##### 3. An account on www.lucidchart.com
A user-account on [www.lucidchart.com](www.lucidchart.com) is required to be able to draw the web app architecture diagrams for AWS or any popular cloud platform if the need arise.


### How to run?
You can run thescript in two easy steps:
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh udagramNetworkBuild network.yml network-parameters.json
# Create servers
# Change the AMI ID and key-pair name in the servers.yml
# Check the region in the update.sh file
./update.sh udagramProjectUpdate servers.yml servers-parameters.json
```