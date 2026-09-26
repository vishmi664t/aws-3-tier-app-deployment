# Three-Tier Web Application Deployment on AWS

## Project Overview
This project demonstrates a complete three-tier web application architecture deployed on AWS, covering networking, compute, and database layers. Built as part of my hands-on AWS learning, following AWS's official three-tier architecture workshop as a base and implementing it end-to-end on my own AWS account.

## Architecture
- **Web Tier**: EC2 instances running NGINX and a React.js frontend, in public subnets
- **App Tier**: EC2 instances running a Node.js backend, in private subnets
- **Database Tier**: Amazon Aurora (MySQL-compatible) RDS in private subnets with Multi-AZ setup

## What I Configured
- Custom VPC with 6 subnets across 2 Availability Zones (public web, private app, private database)
- Internet Gateway and NAT Gateways for secure inbound/outbound traffic
- Route tables and security groups for each tier, following least-privilege access
- IAM roles for EC2 instances to securely access S3 and Systems Manager
- Internal and internet-facing Application Load Balancers
- Auto Scaling Groups for high availability on web and app tiers
- Aurora RDS database with a sample transactions table

## Tech Stack
AWS (EC2, VPC, RDS, S3, IAM, ALB, Auto Scaling), NGINX, Node.js, React.js, MySQL

## Note
This project is based on AWS's official three-tier architecture workshop, implemented and configured hands-on as part of my DevOps and cloud learning.


