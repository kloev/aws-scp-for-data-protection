# Service Control Policies for Data Protection in AWS
This repository aims to give recommendations for AWS SCP that help protect your data in your AWS Organization. 

## DenyAllOutsideEUFrankfurt
This policy denies all listed services to be deployed outside of eu-central-1. This is eesential for being conform with the german GDPR. 

## SCPforOULeavingOrgProtection
Denies users to leave the organization. 

## DenyUsersToStopCloudtrail
Denies users to stop cloudtrail logging. 

## NoAWSAccess
Only use this rule for suspended accounts.

## DenyConfigRuleChanges
Denies User to change config rules. Config Rules are essential to monitor your security best practices. 

## DenyForbiddenServices
Use this rule for OUs and its children that are not allowed to access specific services. Define the policy based on your own compliance rules. 

## PreventS3FromUnencryptedUpload


## S3EnforceSpecificEncryption

## Sources
[AWS Blog Post: Codify your best practices using service control policies](https://aws.amazon.com/de/blogs/mt/codify-your-best-practices-using-service-control-policies-part-2/)

[Medium article: AWS Governance — Service Control Policies](https://medium.com/@seshu/aws-governance-service-control-policies-6d23b144ec72)

[AWS Organizations User Guide: SCP examples](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps_examples.html)