#### Security, Identity & Compliance
###### Identity and Access Management (IAM)
###### Deep dive into Key Management Service (KMS). There would be quite a few questions on this.
* Understand IAM Policies, Key Policies, Grants to grant access
* Understand the difference between CMK with generated and imported key material esp. in rotating keys
* KMS usage with VPC Endpoint which ensures the communication between the VPC and KMS is conducted entirely within the AWS network.
#### Networking & Content Delivery
###### Virtual Private Connect – VPC
* Security Groups, NACLs: NACLs need to open ephemeral ports for response traffic.
* VPC Peering
 To enable communication betwee
 n VPCs within the same or different regions.
 Route tables need to be configured on either VPC for them to be able to communicate.
 does not allow cross-region security group reference.
 ###### CloudFront
* Viewer Protocol Policy and Origin Protocol Policy to enforce HTTPS – can be configured to require that viewers use HTTPS to request the files so that connections are encrypted when CloudFront communicates with viewers.
* CloudFront Origin Shield
* field-level encryption
* custom headers **X-Origin-Verify**
 ###### Route 53
 * Route 53 DNSSEC: secures DNS traffic, and helps protect a domain from DNS spoofing man-in-the-middle attacks. 
 * Resolver query logging: logs the queries that originate in specified VPCs, on-premises resources that use inbound resolver or ones using outbound resolver as well as the responses to those DNS queries
 ######  Gateway Load Balancer – GWLB
 * helps deploy, scale, and manage virtual appliances, such as firewalls, IDS/IPS systems, and deep packet inspection systems.
 ###### Elastic Load Balancer
 * End to End encryption
 * can be done NLB with TCP listener as pass through and terminating SSL on the EC2 instances
 * can be done with ALB with SSL termination and using HTTPS between ALB and EC2 instances
