# Prisma Cloud AWS Permission Sample 

The following github shows policies required by Prisma Cloud for Prisma Cloud Assessment on AWS Accounts. As part of the assessment, the following security settings are enabled:
1. Misconfigurations (CSPM)
2. Identity Security
3. Agentless Workload Scanning
4. Threat Detection


During AWS account onboarding to Prisma Cloud, the role and policies can be created by the Cloud Formation Template (CFT) generated from the onboarding wizard in Prisma Cloud. As part of the CFT, the following items will be done:
1. Create IAM Role with trusted relationship to Prisma Cloud AWS Account
2. Create customer managed policy as the following:
    - prisma_cloud_1
    - prisma_cloud_2
    - prisma_cloud_3
    - prisma_cloud_4
    - prisma_cloud_5
3. Attach the customer managed policies above and SecurityAudit (AWS managed policy) to the IAM role
In any situation where manual onboarding is required, please work with Prisma Cloud team on the updated list of permission. 

Note: This is not an official guide from Palo Alto Networks, and can only be used as a reference. The required permission will change from time to time due to additional services added by AWS. 