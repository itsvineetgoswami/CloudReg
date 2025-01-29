# CloudReg
Cloud bases registration form
![refrence architecture](https://github.com/user-attachments/assets/6f62aa62-7d25-4fb6-b1a8-8fa4d0a18a70)

## Step 1: Create DynamoDB Table

```sh
Table Name: registration-table 
Partition key: email

```

## Step 2: Create IAM Role for Lambda Function
```sh
IAM Role Name: RegistrationFormRole

Permissions:
1. CloudWatch Full Access
2. DynamoDB Full Access

```

## Step 3: Create Lambda Function

```sh
Function Name: registration-form-function
Runtime: Python 3.9

```

## Step 4: Write Lambda Function

## Step 5: Create API Gateway and Enable CORS

## Step 6: Test the Project


### Enable CORS: 

```sh
Access-Control-Allow-Origin: '*'
Access-Control-Allow-Headers: Content-Type,X-Amz-Date,Authorization,X-Api-Key,X-Amz-Security-Token
Access-Control-Allow-Methods: POST

```

## Step 5: create a EC2 server

```sh
configure security group(ssh -22 for admin only)(80 - for normal traffic)
4. connect to ec2 machine
5. install httpd webserver in machine(used to run web app)
 sudo su
 yum update -y
 yum install httpd -y
 cd /var/www/html
 create website (create the files that are requires for your website )
 service httpd start
```
## Step 6: access website from browser using ec2 public ip or DNS
```
simply just copy the public ip of the instance and paste it in the browser

