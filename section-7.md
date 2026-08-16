# More tools for building AI Applciations

## AWS Serverless Data Processing tool

- you don't have run create ec2 instances
- its automaticallay scale out
- its often used in multiple services to get the data
- lambda can be sitting in between services and do something you need like transform the data or something

## Why not just run server

- you have manage this full server like patch deployment services
- you have to pay full day if you are not using it
- you can also run lambda as cronjob
- you manay options of languages to create lambda functions
- there are many services which can trigger lambda function
- like say s3 can trigger lambda function after receiving the object in s3

## Using bedrock with Lambda

- lambda have alot of integration so in bedrock

## API gateway

- you can expose any AWS service to external work using API Gateway
- API gateway have three ways to expose it, glocal, regional, and private
- you can publish in multiple environments

## API Gateway and GenAI

- you can enforce limits in API gateway if response is very high
- you can implemtn you canssend max 10 request per seconds


## AWS App Config

- you can configure the variables and use it in your applciations
- this will helpful without changes your applciations

## AWS AppConfig with GenAI

- you can save model inside configuration and change it when you need it
- can be use bor A/B testing
- you don't need to rebuild the code

## AWS Steps Functions

- step functions collect all steps together and create system
- it has advance error handling
- retry machinic outside your applciation
- ability to wait between functions
- you can have 1 year execution time workflow
- we can also use in ML models
- steps functions can work on automating your data enough
- This is very important tool for data visualization

## Step Functions : Circut Breakers

- this prevent calling service3 wich is not working or timeout
- its also work in AI if the model is not reachable it should call different model
- you can use step function to use approvals for something deployment

## AWS CodeDeploy

- you need to have codedeploy agent on theec2 instances
- you should have appsepec.yaml in the root directory of the repo
- we can deploy following deployment stragitic
    - canar - blue/green, this means create new instances of ec2 instances
    - linear deployment, deploy traffic in some time make like 100% slowly

## MLFlow with GenAI

- its open source tool you can integrate with sagemaker

## AWS AppSync GraphQL with GenAI

- retrive data from multiple data from many source and have in graphql format

## AWS Outpots

- AWS will setup outposts rack in onpremse server you can manage all your servers on AWS cloud
- but you are responsible for physical security of the servers
- you will get local data processing, data will on own data centers

## AWS Outposts and GenAI

- you can run your model locally uisng this serverice

## AWS Wavlength

- wavelenght can deploy to edge so it will be zero latency
- wavelengt zone, this is usecase enable by 5G
- usecases: smart city, ml ,

## AWS wavelength and GenAi

- edge deployment
- secure routing between cloude and on premise
- if there is requirment for zero latency then we should have very high internet to get it done
- low work at edge

## SQS (simple queue service)

- produce send the message and consumer will consume it
- there could be multple producer and consumers
- data could be anything like videos, files
- each message is short live is 4 days max 14 days
- low latency and 1024 kb size
- message can have duplciat but you need to setup atleast once delivery


## AWS Amplify

- connect your all services to mobile using AWS Amlify

## AWS EventBridge

- All services send events to eventbridge
- 