# Deploy container to Amazon ECS (Elastic Container Services) using Fargate

Easy and fun lab! 

I followed the Amazon ECS developer guides here: 
- Creating a container image: https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-container-image.html
- Creating ECS fargate using a container image: https://docs.aws.amazon.com/AmazonECS/latest/developerguide/getting-started-fargate.html 

Lab task overview:
- Create a docker image from scratch (from Dockerfile): see `Dockerfile`
- Push image to Amazon ECR (Elastic Contailer Registry)
- Create an ECS Task definition: see `ecs_task_definition.json`
   - Required creating a new Task Execution IAM role: See `AmazonECSTaskExecutionRolePolicy`
   - Task Execution Role documentation: https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html 
- Create an ECS Service (or task directly) to run task definition.
- Test


## Results
dan@R2-D2:~/labs/create-container-image-ecs$ curl http://hello.mfdg.xyz/
Hello World! (Dans World is the Best!)

