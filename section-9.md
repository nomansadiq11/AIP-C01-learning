# Security, Identity and Compaliance

## Principle of least permissions

- provide only permission people need todo, nore more than

## Data Masking and Annomization

- mask the data, this is built in option in aws glue and other soruce
- you can also encrypt the data
- if you don't need password and credit card number just delete it or don't import it

## IAM Identity Center

- You can integrate with Microsoft AD or third party AD
- you can defin polices in Identity center and attachecd to accounts and users

## AWS Control Towers

- you can create the account and you can define the policy
- you can manage your accounts and implement the compaliance
- can you implement preventive guradrial like only use us-east-1 region
- you can also define detective guardrial like detect untagged resouces


## Amazon Macie

- Macie will discover the PII data and alert you
- it use to find the sensitive data

## AWS Secret Managers

- in AWS this you can integrate most of the services
- you can also replciate in multi region

## AWS Cognito

- These are users sit outside the AWS
- you can integrate external users with application

## AWS WAF

- this use to proectect your applciation
- its on layer 7
- you can define the  ACL rules
- WAF doens't support NLB becuase its on layer 7

## AWS VPC

- its virtual private cloud,
- you can create your own network
- you have mutkple VPC for each region
- you can create subnet in each az
- you need define the routetable to see the traffic toruting
- IG will use to for expor application public
- NAT gateway use to allow download from internet but not accessible from internet

## AWS NCALs and Securigy group

- A firewall which control traffice to and from
- this can be attached to subnet level
- rules only includes IPs
- security groups
    - you can attached this to EC2 machine
    - you can control traffice to and from
- NACLs are stateless


## VPC Flowlogs

- we can capture information all the traffic to your VPC
- this is help you to troubleshott your network connectivity
- Flow logs can be send to streaming services

## VPC Peering

- let say you have two VPC you want to connect together

## VPC endpoint

- you can create endpoint and connect aws services privalty

## Site-toSite VPN

- we can connect on premise to cloud usng VPN

## Direct COnnect

- you can connect your data center privaly, which will take time to todo this

## AWS PrivateLink

- you can connect with another VPC using privatelink without connecting vpc peering
- let say 3rd party need to connect with private link, party have to create the network load balance and you can creae ENI and then top of that you can create private link and connected both VPC
