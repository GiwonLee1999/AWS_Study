# Types of EC2/cloud computing

Application:
- App
- OS
- Computing: CPU + RAM
- Storage
- Network

IaaS: Infrastrucutre as a Service - Computing, storage, network
- Provide infrastructure
- OS must be installed and develop software
- Like borrowing a virtual computer
- eg:  AWS EC2
For example: 
You are hungry and you are renting a kitchen which contains: nothing and you need to bring your ingredients, recipes, tools. In results, you get your food.


PaaS: Platform as a Service - OS+ Runtime, Computing, storage, network
- Infra + OS + etc softwares to run programs
- Can operate right away with code
- eg: Firebase, Google App Engine
For example: 
You are hungry and you are renting a kitchen which contains:  ingredients, tools. You must bring your own recipe then you get your food.
Bring code*

SaaS: Software as a Service: Infra + OS + necessaryr softwares
- Provide entire service
- Utilize service
- eg: Gmail. DropBow, Slack, Google Docs
For example: 
You are hungry and you are renting a kitchen which contains:  everything. And you get your food.


Cloud computing deployment model:
public: cheap, flexible, ran entirely in cloud
protected(hybrid, mix): use as a backup
private: highly customizable, initially expensive, high fees to maintain, high security



# AWS structure
- Region: physical data centre
	- gloabal service: data& service are shared in the world
		- cloudFront, IAM, Route53, WAF
	- local service: particular regions based, data & service provided
		- most of services
		- S3
- edge location: multiple data centre distributed in the world, fast access to whoever is close to them

ARN: Amazon resource name - AWS resources and key ID

# AWS account - practical
- IAM: manually created user for authorized services, can call AWS API: - AccessKey (like ID), Secret Access Key (like password)
- Root user: main admin

Do not use root user as a main
Do not create unnecessary users
Use group or policy in most of cases
Use least authorized 
Activate MFA
Use roles than AccessKey
Use Credential Report if possible
