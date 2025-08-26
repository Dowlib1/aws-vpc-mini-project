# aws-vpc-mini-project
hands-on project on vpc
##search for 'VPC' on the aws conle search bar
![iam](images/vpc.png)

![iam](images/vpc1.png)
##create vpc
![iam](images/vpc2.png)
##
![iam](images/vpcc.png)
## Select subnets and choose create
![iam](images/vcpsub.png)
##Configure the subnet like this
![iam](images/vpcjoin.png)

![iam](images/vpcd.png)
###Locate and select internet gateway
![iam](images/vpcigw.png)

![iam](images/vpcig.png)
## Choose action
![iam](images/vpci.png)
###Attach igw to vpc
![iam](images/vpcat.png)
##confirm attach
![iam](images/vpcatt.png)
Repeat for the secong subnet
![iam](images/vpcim.png)
##Create aroute table

![iam](images/vpcrt.png)
##
![iam](images/vpcttr.png)
##Edit associate subnet
![iam](images/vpccp.png)

![iam](images/vpcal.png)

![iam](images/vpch.png)

![iam](images/vpcj.png)

![iam](images/vpcf.png)

![iam](images/vpcfd.png)

![iam](images/vpcja.png)

![iam](images/vpcse.png)

![iam](images/vpcwq.png)

![iam](images/vpcty.png)

![iam](images/vpcop.png)

![iam](images/vpcobo.png)

![iam](images/vpcyu.png)

![iam](images/vpccz.png)

![iam](images/vpcgo.png)

![iam](images/vpcfh.png)

![iam](images/vpc22.png)

![iam](images/vpcxc.png)
##Step -6 Creating two VPC in two region.
![iam](images/vpcinit.png)

![iam](images/vpcout.png)

![iam](images/vpc1u.png)
3. Now, provide a name for the VPC peering connection.

a) select the requester VPC.

b) Choose the account "My account" since the VPCs are in our own AWS account.

c) Ensure to use the same region, "This Region (ap-southeast-1)," as the VPCs were created in the same region.

d) Next, select the accepter VPC.

e) proceed by clicking on the "Create Peering Connection" button.
![iam](images/vpcwq.png)


![iam](images/vpcacc.png)

![iam](images/vpcmj.png)

![iam](images/vpcrou.png)
b) Click on Accept request.
![iam](images/vpcfree.png)
5. Now, click on Main route table ID of the accepter VPC.
![iam](images/vpcwe.png)
6. Choose the route table.
a) then navigate to the "Routes" section.
b) Click on "Edit route."
![iam](images/vpfeg.png)
c) Click on add route.
![iam](images/vpc300.png)

![iam](images/vpcsav.png)

![iam](images/vpcv.png)
7. Go to the VPC page

a) select the requester VPC.

b) In the details tab, you'll find the IPv4 CIDR. (in this case - 192.168.0.0/16)

c) Copy this CIDR and paste it in the "Destination" field when adding a route.




![iam](images/vpck.png)

![iam](images/vpcope.png)
d) In the target, choose VPC peering and then choose the peering connection you have created. Click on save
changes
![iam](images/vpcci.png)

![iam](images/vpcpp.png)
9. Now, click on Main route table ID of the requester VPC.
![iam](images/vpclo.png)

![iam](images/vpcyi.png)

![iam](images/vpc.png)
9. Now, click on Main route table ID of the requester VPC.
![iam](images/vpc1.png)
10. Choose the route table, then navigate to the "Routes" section. Click on "Edit route."
![iam](images/vpc2.png)

![iam](images/vpc.png)
 Click on add route.

a) Paste the CIDR in the "Destination" field.

b) In the target, choose VPC peering

c) Then choose the peering connection you have created.

Alt text

The connection has been successfully established. Now, resources in the accepter VPC can connect to resources
in the requester VPC, and vice versa.
![iam](images/vpc1.png)

![iam](images/vpc2.png)







