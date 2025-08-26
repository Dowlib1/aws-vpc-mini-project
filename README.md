# AWS VPC Mini Project

## Project Reflection

- Successfully completed the project tasks related to setting up VPC infrastructure and configuring network components.
- Gained practical experience in navigating AWS management console and configuring VPC resources.
- Encountered challenges such as CIDR block size limitations and learned how to troubleshoot and resolve them effectively.
- Developed a deeper understanding of network architecture and cloud networking concepts through hands-on experimentation.
- Recognized the importance of network security measures, such as NAT gateways and VPC endpoints, in ensuring secure communication within cloud environments.
- Overall, the project offered valuable perspectives on the fundamentals of cloud networking and practical experience in deploying VPC infrastructure on AWS.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Step-by-Step Guide](#step-by-step-guide)
    - [Search for VPC](#search-for-vpc)
    - [Create VPC](#create-vpc)
    - [Configure Subnets](#configure-subnets)
    - [Set up Internet Gateway](#set-up-internet-gateway)
    - [Create Route Tables](#create-route-tables)
    - [VPC Peering](#vpc-peering)
3. [Best Practices](#best-practices)
4. [Conclusion](#conclusion)

---

## Introduction

This mini-project provides hands-on experience deploying and configuring AWS VPCs, subnets, gateways, route tables, and peering connections. It aims to help you understand cloud networking fundamentals and security best practices.

---

## Step-by-Step Guide

### Search for VPC

- In the AWS Console, search for "VPC" in the search bar.

![Search for VPC](images/vpc.png)
![VPC Dashboard](images/vpc1.png)

---

### Create VPC

- Click "Create VPC".

![Create VPC](images/vpc2.png)
![VPC Configuration](images/vpcc.png)

---

### Configure Subnets

- Select subnets and choose "Create".

![Create Subnet](images/vpcsub.png)
- Configure the subnet parameters.

![Subnet Configuration](images/vpsjoin.png)
![Additional Subnet Options](images/vpcd.png)

---

### Set up Internet Gateway

- Locate and select "Internet Gateway".

![Internet Gateway](images/vpcigw.png)
![Internet Gateway Details](images/vpcig.png)
- Choose "Create" or "Attach" as needed.

![Choose Action](images/vpcyi.png)
- Attach the Internet Gateway to your VPC.

![Attach IGW](images/vpcat.png)
![Confirm Attach](images/vpcatt.png)
- Repeat for the second subnet.

![Second Subnet](images/vpcim.png)

---

### Create Route Tables

- Create a route table.

![Create Route Table](images/vpcrt.png)
![Route Table Details](images/vpcttr.png)
- Edit and associate your subnet with the route table.

![Associate Subnet](images/vpccp.png)
![Subnet Association](images/vpcal.png)
![Route Table Association](images/vpch.png)
![Route Table Edit](images/vpcja.png)
![Final Route Table](images/vpcf.png)
![Route Table Confirmation](images/vpcfd.png)
![Route Table Review](images/vpcja.png)

---

### VPC Peering

**Steps to Create Peering Connection between Two VPCs:**

1. Deploy two VPCs (can be in different regions).

![Create Two VPCs](images/vpc22.png)
![VPC Regions](images/vpcxc.png)
![VPC Initialization](images/vpcinit.png)
![VPC Output](images/vpcout.png)

2. Create VPC Peering Connection.

![VPC Peering](images/vpc1u.png)

- Provide a name for the peering connection.
- Select the requester VPC.
- Choose "My account" for the account.
- Ensure both VPCs are in the same region.
- Select the accepter VPC.
- Click "Create Peering Connection".

![Peering Connection](images/vpcwq.png)
![Peering Acceptance](images/vpcacc.png)
![Peering Management](images/vpcmj.png)

3. Accept the peering request.

![Accept Peering Request](images/vpcrou.png)
![Peering Free](images/vpcfree.png)

4. Edit route tables to enable communication between VPCs.

- Go to the main route table ID of the accepter VPC.

![Accepter VPC Route Table](images/vpcwe.png)
- Edit routes and add the CIDR of the requester VPC.

![Edit Route](images/vpcfeg.png)
![Add Route](images/vpc300.png)
![Save Route](images/vpcsav.png)
![Route Table Verification](images/vpcv.png)

- Copy IPv4 CIDR from the requester VPC details.

![Copy CIDR](images/vpck.png)
![Paste CIDR](images/vpcope.png)
- Select VPC peering as the target, then choose the peering connection.

![Select Peering](images/vpcci.png)
![Peering Confirmation](images/vcppp.png)

- Do the same for the requester VPC.

![Requester Route Table](images/vpclo.png)
![Requester Route Table Verification](images/vpcyi.png)

- Add routes as before.

![Requester Route Table](images/vpc1.png)
![Requester Route Table](images/vpc2.png)

- The connection has been successfully established. Now, resources in both VPCs can communicate.

![Success Confirmation](images/vpc1.png)
![Peering Success](images/vpc2.png)

---

## Best Practices

- Always plan your CIDR blocks to avoid overlaps and maximize address space.
- Use NAT gateways and VPC endpoints for secure access to AWS services.
- Regularly review your route tables for unintended routes.
- Follow AWS security best practices for subnet isolation and public/private resource configuration.

---

## Conclusion

This project enabled hands-on learning of AWS VPCs, including their configuration, networking, security, and peering.  
You now have practical knowledge of deploying and managing cloud networks, troubleshooting, and applying security measures in AWS.

---
