# awsms-intra-setup

Code for AWS infrastructure setup:

Sequence of running stacks:

1. awsms-poc-vpc.yml - To create VPC, Subnets, NAT Gateways, Internet Gateway, Route Tables, Routes, VPC Endpoints

2. awsms-poc-ecs-cluster.yml - To create ECS Cluster and Roles.

3. awsms-poc-ecr-code-build.yml - To create Repository and CodeBuild.

4. awsms-poc-alb.yml - To create ALB, Target Group, Security group for Load Balancer, Listener

5. awsms-poc-ecs-service.yml - To create ECS service, Tasks, Task Defination, Log Group

6. awsms-poc-code-pipeline.yml - To create codepipeline - after this if build got failed then we need to edit codebuild stage and need to login to Github Repo
