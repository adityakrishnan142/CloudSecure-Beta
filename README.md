# Cloud Microsegmentation Demo Simulation

Welcome to the Microsegmentation Demo Simulation App! This project is designed to highlight the power of Illumio's Cloudsecure by demonstrating its ability to secure and microsegment a vulnerable application environment effectively.

## Overview

The primary goal of this project is to demonstrate how Illumio Cloudsecure can be leveraged to implement microsegmentation within a complex cloud environment.

Microsegmentation is a critical aspect of modern network security, and Illumio provides robust solutions for Microsegmentation. This demo simulation serves as a realistic, intentionally vulnerable application that users can use alongside Illumio Cloudsecure to witness firsthand how microsegmentation enhances security.

The AWS CloudFormation template (cloudformation-template.yml) included in this project creates various AWS resources, including:

- **Virtual Private Cloud(VPC)**
- **Subnets**
- **Internet Gateway**
- **NAT Gateway**
- **EC2 Instances**

In our scenario, we have defined 3 subnets (prod, dev and staging) in a single VPC. Within each subnet, we have created 3-tier applications using EC2 instances. This will be created using the provided Cloudformation template along with the flows. 

![image](https://github.com/adityakrishnan142/CloudSecure-Beta/assets/56053567/2d740069-300b-40e2-a42a-05288da565a3)

Please go through the beta runbook provided to you to get a detailed overview of cloudsecure and its capabilities. 

To run this CFT template - 

1. Please make sure you are logged into your AWS account in **US-East-1** region
2. Click on the launch stack button below to open the AWS cloudformation console and create a new stack

[![image](https://github.com/adityakrishnan142/CloudSecure-Beta/assets/56053567/92b6adb3-d96d-44fa-aae7-f0bd524a17c5)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=Illumio-Beta-Demo-Simulation&templateURL=https://cft-illumio-simulation.s3.amazonaws.com/Illumio-Beta-Demo-Simulation.yaml)



