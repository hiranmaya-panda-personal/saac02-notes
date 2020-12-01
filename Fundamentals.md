## Public vs Private Services
It's a networking difference - i.e. services that be connected but not necessarily have the permission to make changes!

AWS has:
* AWS Public zone (say S3 Bucket) - can be connected to through public internet.
* AWS Private zone (say EC2 instances) - isolated by default. Only services within the same private space can interact with and/or specialised private networks that you create links with(such as On-Premises).

Private zones can be further divided using VPC.

Some AWS private zone's services can be configured to make them accessible via public internet.
When AWS private zone's services are configured in such a manner, it means that the service in question is projected across to the AWS Public space & you can access it via the public internet.

## Global infrastructure 

