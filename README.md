# CF Mount EC2-S3 Template
AWS CloudFormation stack template for Infrastructure as Code (IaC) to automate the provisioning of AWS resources
To provision an AWS S3 bucket for shared storage across three AWS EC2 instances within the same VPC, ensuring each instance resides in a separate availability zone, we will integrate EC2 and S3 using instance profiles, IAM roles, and policies. We'll use a CloudFormation template stack to provision the necessary resources, fetching input parameters from Parameter Store for secure storage of credentials. Additionally, Docker will be installed on each EC2 instance using user data script.
Services Used:
	AWS CloudFormation: For Infrastructure as Code (IaC) to automate the provisioning of AWS resources.
	Amazon EC2: To launch and manage virtual servers in the AWS cloud.
	Amazon VPC (Virtual Private Cloud): To create a virtual network including subnet, route table and IGW for AWS resources.
	Amazon S3 (Simple Storage Service): To create the shared storage bucket.
	AWS IAM (Identity and Access Management): To define roles and permissions for EC2 instances to access S3.
	AWS Systems Manager Parameter Store: To securely store AWS credentials for EC2 instances.
