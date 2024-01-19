login, account, services, lightsail (manage virtual private servers) 

#### EC2 (virtual servers in the cloud)
- Launch Instance
- Select Amazon Linux AMI as the image
- Type is t2.micro
- Generate a pair of keys
- Leave network and storage as default
- Name and Tags: myFirstEC2
- Launch Instance

#### S3 (scalable storage in the cloud)
- Create a bucket (data container)
- Set a name and region
- Leave the public access blocked
- Create it

#### Restart the EC2 instance
- Resources
- Instances (running)
- Instance state and reboot

#### Allos public access to the S3 bucket
- Services -> S3
- Select our bucket -> permissions
- Block public access -> edit
- Uncheck the "block all public access" checkbox and confirm

#### Delete AWS resources

###### Delete the EC2 instance
- Services -> EC2 -> Instances (running)
- Select it
- Instance state -> Terminate instance

###### Delete the S3 bucket
- Services -> S3
- Select it
- Delete