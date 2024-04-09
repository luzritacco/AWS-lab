<h1 align="center"> AWS CLOUD LAB</h1>


Exploring AWS Cloud Labs is a fantastic way to immerse oneself in the cloud environment, providing invaluable resources for those new to cybersecurity. Building this  lab offer hands-on experience, which is crucial for developing the skills needed to excel in the field. Moreover creating  this lab, I will learn invaluable experience that is often not possible through traditional education methods.

<h1 align="center">BILLING ALARM</h1>

To optimize billing and cost management and prevent unexpected charges, setting up billing alarms is a proactive step. For AWS users, Amazon CloudWatch allows the creation of billing alarms to monitor estimated charges. By enabling billing alerts in the AWS Billing console, users can set alarms that trigger when account billing exceeds a specified limit.
To optimize your billing and cost management and avoid unexpected charges, consider implementing the following strategies:

- **Set Up Billing Alerts**: Configure alerts to notify you when you’re spending reaches a certain limit.
- **Review Regular Reports**: Schedule and review regular reports for a detailed understanding of your costs.
- **Implement Budgets**: Create budgets for different projects or departments to keep spending in check.
- **Utilize Cost Management Tools**: Use cloud provider or third-party cost management tools for insights and optimization recommendations.
- **Monitor Resource Usage**: Keep an eye on your resource usage to ensure you're not paying for unused or underutilized services.
- **Optimize Subscriptions**: Regularly review and adjust your subscriptions or service plans to match your actual usage patterns.
- **Automate Cost-Saving Measures**: Implement automation for shutting down unused resources or scaling services based on demand.

By following these steps, you can maintain better control over your expenses and reduce the likelihood of incurring unexpected charges. 


![Screenshot 2024-04-05 001211](https://github.com/luzritacco/AWS-lab/assets/151267325/aab66d16-3e97-42ef-9761-79edba36c6b3)

##
<h1 align="center">CREATE A NON-ROOT USER ACCOUNT </h1>

Setting up non-root user accounts with appropriate permissions is a critical step in maintaining a secure and organized lab environment. Here's a bullet point list to guide you through the process:

- **User Account Creation**: Create individual user accounts for each person who will be using the lab systems to ensure accountability and traceability of actions.
- **Permission Levels**: Assign permissions based on the principle of least privilege, giving users the minimum level of access necessary to perform their tasks.
- **User Groups**: Organize users into groups based on their role or function in the lab to streamline the management of permissions.
- **Access Control**: Implement access controls to sensitive data and systems, ensuring that only authorized users can access certain information or resources.
- **Password Policies**: Enforce strong password policies and consider multi-factor authentication to enhance security further.
  
By following these steps, you can help ensure that your lab remains secure, efficient, and compliant with relevant policies and regulations.
 ![Screenshot 2024-04-05 002146](https://github.com/luzritacco/AWS-lab/assets/151267325/908ca7fb-d120-484c-a4d2-093de773be0f)

![2024-04-09 03_19_32-Screenshot 2024-04-05 002438](https://github.com/luzritacco/AWS-lab/assets/151267325/a6a1afa5-ad93-4af2-aba1-2cf7702360ef)

##

<h1 align="center">VPC (VIRTUAL PRIVATE CLOUD) </h1>

A Virtual Private Cloud (VPC) is a critical step towards ensuring a secure and resilient online environment for your resources. A VPC is a virtual network dedicated to your AWS account, isolated from other virtual networks and providing scalable infrastructure to deploy applications and services securely.

Here are key steps to configure a secure VPC:
- **Define Network Objectives**: Before diving into configurations, outline the objectives for your VPC. Consider aspects such as the number of subnets, connectivity requirements, whether public or private, and the region distribution.
-  **Subnet Strategy**: Create subnets in multiple Availability Zones to ensure high availability and fault tolerance. This approach not only provides resilience against outages but also optimizes performance.
-  **Security Groups and Network ACLs**: Implement security groups to control inbound and outbound traffic to your EC2 instances. Network Access Control Lists (ACLs) can provide an additional layer of security, regulating traffic at the subnet level.
-  **Identity and Access Management (IAM)**: Use IAM to manage access to AWS resources within your VPC securely. By setting up IAM roles and policies, you can ensure that only authorized personnel have access to specific resources.
-  **Data Protection**: Employ encryption methods for data at rest and in transit within your VPC to protect sensitive information from unauthorized access.
-  **Monitoring and Logging**: Utilize tools like VPC Flow Logs to monitor network traffic and detect unusual activity. Regular monitoring can help in identifying potential security threats early.

  
By following these steps, you can establish a VPC that not only meets your operational requirements but also aligns with stringent security standards. Remember, a well-configured VPC is the cornerstone of a secure cloud ecosystem, enabling you to leverage the full potential of cloud computing with confidence.


![Screenshot 2024-04-05 003323](https://github.com/luzritacco/AWS-lab/assets/151267325/0fbba438-25de-427e-a9cb-3cdbadb488b4)


![Screenshot 2024-04-05 003633](https://github.com/luzritacco/AWS-lab/assets/151267325/c8342e4b-529f-4311-83d6-33750d57f80a)

![Screenshot 2024-04-05 004841](https://github.com/luzritacco/AWS-lab/assets/151267325/9e1d3cb3-611b-4800-b6ad-2c20f82589e8)

![Screenshot 2024-04-05 005326](https://github.com/luzritacco/AWS-lab/assets/151267325/1cc8f665-5dfd-4cb3-9a54-935158571012)

   ##
   
<h1 align="center">LAUNCH EC2 AMAZON ELASTIC INSTANCE ON KALI LINUX </h1>


Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers and allows for scalable deployment of applications by providing a web services interface through which a user can create and manage virtual machines, or instances.

For users of Kali Linux, a popular Linux distribution designed for digital forensics and penetration testing, launching an EC2 instance can be particularly useful. Whether it's for security testing, running simulations, or just leveraging the cloud for various tasks, the process is straightforward but requires attention to detail.

Here's a step-by-step guide to launching an Amazon EC2 instance on Kali Linux:

- **Create an AWS Account**: Before you can launch an EC2 instance, you need to have an active AWS account. If you don't have one, you can create it on the AWS website.
- **Select the Kali Linux Amazon Machine Image (AMI)**: Once logged into your AWS account, navigate to the EC2 dashboard and select "AMI Catalog" on the left side. Search for the official Kali Linux image and select it.
- **Instance Configuration**: After selecting the Kali Linux AMI, you will need to configure your instance. This includes selecting the instance type, which determines the hardware of the host computer used for your instance.
- **Security Settings**: Set up security groups and key pairs to ensure secure access to your instance. Security groups act as a virtual firewall that controls the traffic for one or more instances, while key pairs are used to securely log into your instance.
- **Storage Configuration**: Configure the storage settings for your instance. By default, the storage selected does not use magnetic storage, which may incur additional costs. You can change this to "standard" to prevent extra costs.
- **Launch the Instance**: After configuring all settings, you can launch your instance by clicking on "Launch Instance". You will then see a screen confirming that your instance is launching.
- **Connect to Your Instance**: After the instance is up and running, you can connect to it using SSH. The command to connect will typically look like this: `ssh -i "keys.pem" kali@ip-address`, where `keys.pem` is your private key file and `ip-address` is the public IP address of your instance.
- **Post-Connection Configuration**: Once connected, you may want to update the system and install necessary software. For a full Kali Linux toolset, you can utilize Kali’s metapackages.

By following these steps, you can successfully launch and connect to a Kali Linux EC2 instance, ready for whatever tasks you may need it for. Remember to always adhere to AWS's acceptable use policy, especially when conducting penetration testing or other security-related activities.
![Screenshot 2024-04-05 005400](https://github.com/luzritacco/AWS-lab/assets/151267325/61a3844a-e651-4f0e-8dbe-20d7dabc49d5)
![Screenshot 2024-04-05 005432](https://github.com/luzritacco/AWS-lab/assets/151267325/9f415de8-1544-4860-9567-3d0325955951)

Connect to instance 

![Screenshot 2024-04-05 013907](https://github.com/luzritacco/AWS-lab/assets/151267325/1942a24e-91b3-4578-b2c0-9d26caf809d0)

##
<h1 align="center">LAUNCH EC2 AMAZON ELASTIC -widows server  </h1>


Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud, allowing users to run applications on a virtual server known as an instance. For those looking to launch a Windows server on EC2, the process is straightforward and can be done in a few simple steps.

- **Step 1: Launch an Instance-** To launch a Windows instance, navigate to the Amazon EC2 console. From the dashboard, select 'Launch Instance' to start the process.
- **Step 2: Choose an Amazon Machine Image (AMI)**-Select a Windows-based AMI from the Quick Start list. Amazon provides a variety of AMIs pre-configured with different versions of Windows Server.
- **Step 3: Select an Instance Type**Choose an instance type that matches your performance and budget requirements. AWS offers a range of instance types designed for different use cases.
- **Step 4: Configure Instance Details**Set up the network and security group for your instance. You can select an existing security group or create a new one that specifies which ports are open and who can access the instance.
- **Step 5: Add Storage**You can add additional Elastic Block Store (EBS) volumes if you need more storage than what is provided by default with the AMI.
- **Step 6: Configure Security Group**A security group acts as a virtual firewall. You must configure it to control the traffic to and from your instance.
- **Step 7: Review and Launch**Review your instance configuration and make any necessary changes. When you're ready, click 'Launch' to start your Windows server.
- **Step 8: Connect to Your Instance**After the instance is running, connect to it using Remote Desktop Protocol (RDP). You'll need the public DNS name or IP address of the instance and the private key file associated with your security group.

By following these steps, you can successfully launch and connect to a Windows server on Amazon EC2. 

