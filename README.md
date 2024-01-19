# AWS CloudFormation Infrastructure as Code (IaC)

![AWS CloudFormation](https://img.shields.io/badge/AWS-CloudFormation-orange?style=for-the-badge&logo=amazon-aws)

This repository contains an Infrastructure as Code (IaC) template using AWS CloudFormation to deploy and manage AWS infrastructure. The provided CloudFormation template encompasses various aspects of infrastructure such as networking, EC2 instances, and other AWS services.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project utilizes AWS CloudFormation to define and provision AWS infrastructure in a declarative manner. The entire infrastructure code is encapsulated in a single CloudFormation template file.

## Prerequisites

Before using this CloudFormation template, ensure you have the following prerequisites:

- AWS Account
- AWS CLI Installed
- AWS CLI Configured with the necessary credentials

## File Structure

```plaintext
cloudformation_code_for_iaas/
│
├── aws_code.yml
├── README.md
└── ...
```
`aws_code.yml`: The CloudFormation template containing the entire infrastructure code.

## Getting Started


1. **Clone the repository:**

    ```bash
   git clone https://github.com/Umang746/cloudformation_code_for_iaas.git
   cd cloudformation_code_for_iaas

    ```

2. **Review the CloudFormation Template:**

   Open and review the aws_code.yml file to understand the defined infrastructure.

  ## Usage

1. **Deploy the Infrastructure:**

    ```bash
    aws cloudformation deploy --template-file aws_code.yml --stack-name YourStackName --parameter-overrides Param1=Value1 Param2=Value2


    ```

2. **Monitor Deployment:**

  Check the AWS CloudFormation console or use the AWS CLI to monitor the deployment status.

  ## Example

### Scenario: Deploying a Basic VPC and EC2 Instance

In this example, we'll deploy a simple AWS Virtual Private Cloud (VPC) and an EC2 instance using the provided CloudFormation template (`aws_code.yml`).

#### Steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/Umang746/cloudformation_code_for_iaas.git
    cd cloudformation_code_for_iaas
    ```

2. **Review the CloudFormation Template:**

    Open the `aws_code.yml` file and understand the defined resources, parameters, and outputs.

3. **Deploy the Infrastructure:**

    Execute the following AWS CLI command to deploy the CloudFormation stack. Replace the placeholders with your desired values.

    ```bash
    aws cloudformation deploy --template-file aws_code.yml --stack-name MyExampleStack --parameter-overrides VpcCidrBlock=10.0.0.0/16 SubnetCidrBlock=10.0.1.0/24 InstanceType=t2.micro
    ```

    - `VpcCidrBlock`: CIDR block for the VPC.
    - `SubnetCidrBlock`: CIDR block for the subnet.
    - `InstanceType`: EC2 instance type.

4. **Monitor Deployment:**

    Check the AWS CloudFormation console or use the AWS CLI to monitor the deployment status.

5. **Access Resources:**

    Once the deployment is complete, access the AWS Management Console to view the newly created VPC and EC2 instance.

6. **Cleanup (Optional):**

    If needed, tear down the deployed resources using the following AWS CLI command:

    ```bash
    aws cloudformation delete-stack --stack-name MyExampleStack
    ```

    Confirm the deletion when prompted.

This example demonstrates a basic scenario, and you can customize the parameters and resources in the CloudFormation template based on your specific infrastructure requirements.


  
