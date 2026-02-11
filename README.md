## Disclaimers
Customers are responsible for making their own independent assessment of the information in this document.

This document:

(a) is for informational purposes only,

(b) references AWS product offerings and practices, which are subject to change without notice,

(c) does not create any commitments or assurances from AWS and its affiliates, suppliers or licensors. AWS products or services are provided "as is" without warranties, representations, or conditions of any kind, whether express or implied. The responsibilities and liabilities of AWS to its customers are controlled by AWS agreements, and this document is not part of, nor does it modify, any agreement between AWS and its customers, and

(d) is not to be considered a recommendation or viewpoint of AWS.

Additionally, you are solely responsible for testing, security and optimizing all code and assets on GitHub repo, and all such code and assets should be considered:

(a) as-is and without warranties or representations of any kind,

(b) not suitable for production environments, or on production or other critical data, and

(c) to include shortcuts in order to support rapid prototyping such as, but not limited to, relaxed authentication and authorization and a lack of strict adherence to security best practices.

All work produced is open source. More information can be found in the GitHub repo.

## README: How to Use AWS CDK, Terraform CDK, and Hashicorp Terraform

This project demonstrates the usage of AWS CDK (Cloud Development Kit) in Python, Terraform CDK in Python, and Hashicorp Terraform to create a basic queue in AWS.

### Prerequisites 
Configure your AWS credentials:

`aws configure`

### AWS CDK

1. Install the AWS CDK globally:

   `npm install -g aws-cdk@2.136.1`
2. Create a virtual environment and install the required dependencies:

   `python3 -m venv myLib`
   
   `pip3 install -r requirements.txt`
4. Navigate to the `aws-cdk-demo` directory:

   `cd aws-cdk-demo`
5. Initialize the AWS CDK project:

   `cdk init app --language python`
6. To deploy the AWS CDK stack:

   `cdk synth`

   `cdk deploy`
   
   This will create an SQS queue and a CloudFormation template named "AwsCdkDemoStack-CIC".

### Terraform CDK

1. Install the Terraform CDK:
   
   `brew install cdktf`
2. Navigate to the `terraform-cdk-demo` directory:

   `cd terraform-cdk-demo`
3. Initialize the Terraform CDK project:

   `cdktf init`
4. To deploy the Terraform CDK stack:

   `cdktf synth`

   `cd cdktf.out/stacks/aws-cdk-demo``

   `terraform init`

   `terraform apply`

### Hashicorp Terraform

1. Navigate to the `terraform-hashicorp` directory:

   `cd terraform-hashicorp`
2. Initialize Terraform:

   `terraform init`
3. Validate the Terraform configuration:

   `terraform validate`
4. Apply the Terraform configuration:

   `terraform apply -auto-approve`
5. To delete the resources:

   `terraform destroy`

Remember to clean up the resources created by each approach to avoid incurring unnecessary costs.
