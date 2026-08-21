# Storage Services You Should Know

## EBS volumes

- these are network drives
- its lock to avaiblity zone but you can move to another az
- you can define how much size you want and IOPS you want
- it cannot be attached two machines
- we can attached two EBS volumes
- you can enable/disable delete on termination of ec2 instance
- its like usb drive to attached to a machine

## EFS

- Its network file system
- its can attached to many ec2 instances
- its expenseive then ebs
- its only compatible with linux base machines
- its pay pr use
- you can scale up and down base on your usecase
- there is classes where you can data like standard, infreqent and archieve