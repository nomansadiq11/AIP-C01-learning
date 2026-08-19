# Analytics Services You should Know

## Athena

- This SQL query engine topic of S3
- it can support many formats like, parquet, json,
- data can be unstruct, struct or semi-structure

## EMR (Elastic MapReduce )

- managed Ec2 instances which have hadoop
- emr cluster
    - master node which manage the cluster core like track of the tasks health of the nodes
    - core nodes which work on your data and can also store data
    - task node which deosn't store data but work on your task
    - task node can be on spot instances
- EMR Usage
    - one of them is transient cluster, after work you can terminate the cluster
    - long running clusters, you can create cluster, and use sport instances and if you gonna running for long time you can reserve the instances

## Amazon QuickSight

- fast, easy clouswer powered business application
- you can build dashboards, it has many other sources
- it has many data sources you can connect and build dasshboard
- SPICE
    - its in memory data calucaltion but it has limitation be remeber taht
- this cannot be use for ETL
- you can also create VPC connectivty with quicksight
- by default QS can access data in same region but other region you need to enable inbound IPs in SG.
- you can also do peering VPC for cross region access
- there are other ways to cross region
- corss account access ther emiht be transit gateway can help

## Amazon Kinesis Data Straming

- you can send streaming data to streaming
- data be will stay for 365, you cannot delete it
- can you read data again
- Provisioned Mode
    - you will select the shared
    - you can scale and shared
    - you can monitor your througput
- Ondemand mode
    - you will pay per hour

## Amazon MSK

- this is apache kafka
- this is alernative the kenisis
