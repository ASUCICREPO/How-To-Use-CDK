# How-To-Use-AWS-CDK

1. npm install -g aws-cdk@2.136.1
2. create virtual env - myLib.
3. pip3 install -r requirements.txt
4. aws configure
5. cd aws-cdk-demo
6. To init AWS-cdk use: 
    1. cdk init app --language python
7. To run:
    1. cdk synth
    2. cdk deploy
 You are now ready to use CDK - Dont forget to delete SQS and Cloudformation template - "AwsCdkDemoStack-CIC"


# How-To-Use-Terraform-CDK

1. Install cdktf using - brew install cdktf
2. cd terraform-cdk-demo
3. To init: cdktf init
4. To run: 
    1. cdktf synth
    2. cd cdktf.out/stacks/aws-cdk-demo
    3. terraform init
    4. terraform apply

