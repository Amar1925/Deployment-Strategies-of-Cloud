# Deployment-Strategies-of-Cloud
## Introduction
First let us understand what Cloud is and what cloud computing is then we will come to the issue of deployment strategies of cloud. Cloud is the computing resources which are provided to us like storage, RAM, CPU, networking etc. over the internet.
While cloud computing is using these on demand resources over the internet  for deploying applications or any other task without hardware being physically present with us. This ensures accesibility, scalability, observability, reliability, authenticity, security etc.
Here we will be talking about two types of cloud:
 ### 1. Public Cloud: 
This is a cloud computing model where computing resources like servers, storage, and applications are owned and operated by third-party cloud providers like AWS, GCC(google cloud), Microsoft Azure and are shared among multiple users over the internet.
- This means that a single computing resource can be shared with many users at a particular time which is sometimes undesirable. Nowadays many companies and organisations are using public cloud to host their applications like Netflix, Gmail, Dropbox etc.
Some Advantages of Public Cloud are:
- High Scalability – Instantly increase or decrease resources according to need.
- Reliability – Cloud providers like AWS offer high uptime (99.99%) and they have a contract for the same.
- Global Reach – We can access resources from anywhere using just an internet connection and logging in to cloud providers site.
- Low Cost – We dont have to pay for hardware set up like servers and computing resources like CPU, RAM, Storage etc. as the cloud provider does it for us. 
### 2. Private Cloud:
 This is a cloud computing model where resources are exclusively used and owned by a single organization. It provides greater control, security, and customization, making it ideal for businesses with strict data security and compliance requirements. Examples include Openstack, VMware.
The single organisation hosting the private cloud has full control over it and its hardware resources which gives it <ins> TCO or total cost of ownership over its product </ins>
- Private Cloud is better over public cloud if you want full control over your resources and dont have much budget constraint as it gives TCO as said above while public cloud provides lower set up costs but can have unpredictable costs over time which are undesirable.
Advantages:
- TCO – The company has full control over their resources and hardware which is an ideal situation instead of 3rd party controlling it
- High security – Company has full access and ownership over resources so automatically the security also increases
- Increased Performance – There is no resource sharing with other users so performance is increased.

### Various Deployment Strategies of Cloud:

### 1. Public Cloud Only:
A public cloud is a computing environment where cloud resources are owned and managed by third-party providers such as AWS, Microsoft Azure, and Google Cloud. Users can access these resources on-demand, typically through a pay-as-you-go model.

- **Deployment**:Services are hosted entirely on a public cloud platform such as AWS, Azure, or Google Cloud.

- Users access resources via the internet, utilizing shared cloud infrastructure managed by the provider.

- **Cost Analysis**:Lower upfront costs as infrastructure is managed by the cloud provider.

- Variable operational costs based on usage (compute, storage, networking).

### Advantages

- Scalability and elasticity, allowing businesses to scale up or down as needed.
- No maintenance overhead since the provider manages hardware and software updates.
- Pay-per-use pricing, which reduces capital expenditure.

### Disadvantages

- Limited control over infrastructure as cloud providers enforce certain policies.
- Potential security and compliance concerns, as data is stored on third-party servers.

Examples include: 

- Hosting a website on AWS EC2 instance or hosting web application on ec2 using the public IP provided by amazon.

- Using Google Cloud Storage for storing backup data.

### 2. Private Cloud Only:
A private cloud is a cloud infrastructure that is exclusively used by a single organization and the organisation has the full ownership over it and the hardware resources associated with it. It can be hosted on-premises or in a third-party data center but is not shared with other customers.

- **Deployment**: Infrastructure is hosted on-premises or in a dedicated data center.

- Managed entirely by an enterprise IT team or a managed service provider.

- **Cost Analysis**: High capital expenditure (CapEx) for purchasing hardware and setting up infrastructure.

- Operational costs (OpEx) for maintenance, staffing, and electricity.

### Advantages

- Full control over security and compliance, ensuring regulatory adherence.
- Customization and dedicated resources tailored to specific organizational needs.

### Disadvantages

- High initial investment required for setting up the infrastructure.
- Limited scalability compared to public clouds.

### Example Services

- Running OpenStack on in-house servers.

- Hosting an enterprise database in a private data center.

### 3. Public on Private Cloud (Hybrid Cloud)
Cloud bursting is a hybrid model where an organization primarily runs applications in a private cloud but dynamically shifts workloads to a public cloud when demand spikes.

- **Deployment**: Deploying certain services on your private cloud and others on a public cloud.
- This allows us to leverage the strengths of both environments.
- Often involves connecting your private cloud to a public cloud through a VPN or dedicated connection.


- **Cost**:Combines the costs of private and public cloud.
- Requires careful cost optimization to balance the two environments.

### Advantages:

- Flexibility: Choose the best environment for each service.
- Scalability: Use public cloud for burst workloads.
- Security: Keep sensitive data in the private cloud.
- Disaster recovery.

### Disadvantages:
- Complexity: Managing two separate environments.
- Integration challenges: Ensuring seamless communication between clouds.
- Increased network complexity.

### Examples:
- E-commerce: Hosting the website on a public cloud and the database on a private cloud.
- Development and testing: Using the public cloud for development and testing, and the private cloud for production.
- Data backup and archival.

### 4. Private on Public Cloud (Dedicated Cloud on Public Infra)

In this model, a private cloud infrastructure is hosted within a public cloud provider’s environment, offering a dedicated yet managed solution
- **Deployment** : Portions of the private cloud environment are deployed inside a public cloud. For example, using VMWare inside of AWS.
- This is often used for migrating existing workloads to the cloud, without refactoring.

### Cost: 
- The cost of the public cloud resources, plus the cost of the private cloud software liscensing.
- Can be expensive.

### Advantages:
- Allows for lift and shift migration, which reduces migration complexity.
- Can use existing private cloud tools, inside the public cloud.

### Disadvantages:
- Increased cost.
- Increased complexity.
- Performance can be degraded.

### Examples:
- Running VMWare workloads inside of AWS, Azure VMWare solution, or Google VMWare engine.

