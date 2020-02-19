# awsms-intra-setup
Code for AWS infrastructure setup:

Sequence of running stacks:

1. awsms-poc-vpc.yml - it will create vpc, subnets, NAT gateways, Internet gateway, Route tables, Routes, VPC Endpoints

2. awsms-poc-ecs-cluster.yml - it will create ECS Cluster and Roles.

3. awsms-poc-alb.yml - it will create ALB, Target Group, Security group for Load Balancer, Listener

4. awsms-poc-ecs-service.yml - it will create ECS service, Tasks, Task Defination, Log Group

5. awsms-poc-code-pipeline.yml - it will create codepipeline - after this if build got failed then we need to edit codebuild stage and need to login to Github Repo
