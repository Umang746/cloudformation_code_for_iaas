# AWS CloudFormation Infrastructure as Code (IaaS) for AWS CloudFront

## Overview

This repository contains Infrastructure as Code (IaC) templates using AWS CloudFormation to deploy and manage infrastructure components for an AWS CloudFront setup.
## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Deployment](#deployment)


## Prerequisites

Before using these CloudFormation templates, ensure you have the following:

- AWS Account
- AWS CLI Installed
- AWS CLI Configured with the necessary credentials



## Getting Started

Clone the repository:
git clone https://github.com/Umang746/cloudformation_code_for_iaas.git
cd cloudformation_code_for_iaas

Modify Configuration:
Review and modify the CloudFormation templates in the templates/ directory based on your requirements.


## Configuration

cloudfront.yaml: Configures the AWS CloudFront distribution.
networking.yaml: Defines networking components such as VPC, subnets, etc.
other_templates.yaml: Additional templates for specific services or configurations.


## Deployment

Use the provided script to deploy the CloudFormation stack:
cd scripts
./deploy.sh
