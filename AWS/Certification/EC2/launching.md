# launching and ec2 (Minimum req)

## Steps

1. Select region 
 - latests services in N.Virginia

2. Services select EC2
 - Select Launch instance
 - Instances created using Amazon Machine Images(AMIs)
 - For learning select amazon linux 2, follow free tier
    - Settings:
    - Use Stop for termination
    - User data (run bootstrap scripts)
 - Add storage
    - Use either General purpose or provisioned
    - can be encrypted using KMS
 - Add Tags
 - Add security groups
    - Change name of security group name - can use DMZ (demilitarized zone)
    - Add HTTP source anywhere (For webserver)
    - SSH access do not use anywhere in production
 - Create new key pair  

3. Connecting to an instance
 - Open Terminal
 - Go to correct folder where the private key is
 - chmod 400 nameOfPrivateKey.pem
 - SSH into ec2 instance:
```shell
ssh ec2-user@(ADD PUBLIC IP ADDRESS HERE) -i nameOfPrivateKey.pem
```
- Elevate priveges
```shell
sudo su
```
- Update operating system
```shell
yum update -y
```
- install apache web server
```shell
yum istall httpd -y
```
- start apache 
```shell
systemctl start httpd
```
- Or start apache at boot time
```shell
systemctl enable httpd
```
- check it is running correctly
```shell
systemctl status httpd
```
- should show as active
- Next need to go to html page location
```shell
cd /var/www/html
```
- Create page you can use nano
```shell
nano index.html
```
- exit with ctrl X and then y to save after you have edited the page

- after you have finished terminate the instance



 

    
   
   


