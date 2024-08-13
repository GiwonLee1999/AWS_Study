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

# Virtualization
- One machine distributes into multiple machines, VM

	- OS: Windows, linux, MacOS...
	- Privileged instruction: Commands with system - only OS can command
		- Regular programs do not need these special authorization
	- Until VM came out, only one OS was able to run

1 gen: Fully emulated: All the system factors are running inside the emulator
- Very slow due to using CPU, Hard disk, motherboard etc..

2en gen: Paravirtualization: Guest OS work with Hypervisor (virtual manager exists between OS and hardware)
- Enhanced speed.

3rd gen: Hardware Virtual Machine(HVM): Hardare supports virtual itself.
- Guest OS communicated directly with hardware === Very fast(near bare-metal)


# EC2: Cloud platform for computing power
Use when:
- Building a server
- Host application or use it: DB, ML, etc ...
- Graphic Rendering.

Pay per second.

Instance: Memory, CPU, graphics
EBS: Elastic Block Storage
AMI: EC2 instance image 

```linux
// user autorization
sudo -s

// install web server
yum install httpd -y

// start web server
service httpd start

// modify this directory or create
nano /var/www/html/index.html
```

Type of instance
e.g m5 ->c gen 5
e.g m5a xlarge
	gen  cpu 	size