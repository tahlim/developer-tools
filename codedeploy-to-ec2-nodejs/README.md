# codedeploy-to-ec2-nodejs
Deploy the Nodejs application to EC2 Instance using CodeDeploy
```
1. launch Ubuntu instance with User-Data:-

Production 1 , Production 2 , Production 3

2. Create IAM roles for both CodeDeploy and EC2 instance:-
We are going to create a Role for EC2 with this name "ec2_to_codedeploy"

AWSCodeDeployFullAccess
AmazonS3FullAccess
AdministratorAccess

We are going to create a Role for CodeDeploy with this name "codedeploy_to ec2"

AWSCodeDeployRole

and then attache this role "ec2_to_codedeploy" to instance Production 1 , Production 2 , Production 3

3. Create Application in CodeDeploy:-

4. Create Deployment group in Application:-

and then attache this role "codedeploy_to ec2" in Deployment group

5. Create CodePipeline using GitHub & CodeDeploy:-

6. Modify the Code & Check if Pipeline works:-
```
