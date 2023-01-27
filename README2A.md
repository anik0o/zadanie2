# Zadanie nr 2 
## CZĘŚĆ NIEOBOWIĄZKOWA

CZĘŚĆ PIERWSZA

-polecenie w celu sprawdzenia usługi ElastiCashe

`aws elasticache describe-cache-clusters`


![image](https://user-images.githubusercontent.com/94603034/215181963-f3d641d7-48d8-4be7-93de-e28c89117024.png)


-polecenie w celu sprawdzenia usługi RDS -  z wprowadzeniem id mojej instancji bazy danych (multifib-postgres)

`aws rds describe-db-instances --db-instance-identifier multifib-postgres`

![image](https://user-images.githubusercontent.com/94603034/215189718-4179b3d5-30b4-4c06-8f83-95612df0b54b.png)


-polecenie w celu sprawdzenia usługi VPC - z wprowadzeniem mojego VPC ID (vpc-04697e01548a48148)

`aws ec2 describe-vpcs --vpc-ids vpc-04697e01548a48148`

![image](https://user-images.githubusercontent.com/94603034/215190226-cb6668da-7f12-4099-83e0-594f6f25ca44.png)



