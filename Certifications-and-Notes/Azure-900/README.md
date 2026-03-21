# My-summary-for-Azure900


## Cloud Computing - Summary
Cloud computing means renting computing resources over the internet instead of buying and managing physical hardware. This helps reduce capital expenditure (CAPEX) and operational expenditure (OPEX). For example, instead of buying an expensive server, you can use a virtual machine in the cloud and pay only for what you use.



## Cloud Service Models
Infrastructure as a Service (IaaS):
You get control over virtual machines, storage, and networking. You are responsible for managing the operating system and applications. The cloud provider handles the physical infrastructure. IaaS is ideal for scenarios where you want to move your existing systems to the cloud with minimal changes.



## Platform as a Service (PaaS):
The cloud provider gives you a ready-to-use platform with development tools and runtime environments. You just deploy your application without worrying about servers or operating systems. It’s great for developers who want to build and run apps quickly.



## Software as a Service (SaaS):
This provides ready-made applications directly to users. You don’t manage anything except how you use the software. Examples include Gmail and Microsoft 365.

Shared Responsibility Model
This model defines what the customer and the cloud provider are responsible for. In on-premises systems, the customer manages everything. In cloud models like IaaS, PaaS, and SaaS, more responsibility shifts to the provider. For example, in SaaS, the provider handles almost everything including security, servers, and updates. This helps customers focus more on using the service rather than maintaining it.

#Cloud Deployment Models


## Public Cloud:
Resources are shared among multiple users. A third-party provider like Microsoft Azure or AWS owns and manages the infrastructure. You pay only for what you use. It’s flexible and cost-effective.



## Private Cloud:
The cloud infrastructure is used by a single organization. It provides more control and better security. It can be hosted in your own data center or by a service provider.



## Hybrid Cloud:
This combines both public and private clouds. Organizations can keep sensitive data in the private cloud and use the public cloud for scaling and flexibility. It offers the best of both worlds.

# Benefits of Cloud Computing
High Availability and Fault Tolerance:
Applications are built to remain accessible even during failures. This is achieved through redundancy like using multiple virtual machines or database replication.

## Scalability:
You can increase or decrease resources based on demand. Vertical scaling means upgrading existing infrastructure, while horizontal scaling means adding more units like virtual machines.

## Elasticity:
The cloud can automatically scale your resources up or down depending on traffic or workload. This means you don’t have to manage capacity manually.

## Cost Effectiveness:
Cloud services are pay-as-you-go. You can estimate and optimize your costs using tools like the Azure Pricing Calculator or the Total Cost of Ownership (TCO) calculator.

Azure Resource Hierarchy
Azure has a structured way of organizing resources:

The top level is the Azure account.

Management Groups help organize multiple subscriptions.

Subscriptions are containers for billing and usage.

Inside subscriptions, you create Resource Groups to group related services.

Resources like Virtual Machines, Databases, or Storage accounts live inside Resource Groups.

Policies and permissions set at higher levels like management groups or subscriptions apply automatically to the levels below them.

# Azure Portal Overview
The Azure Portal is a web-based dashboard to manage Azure services. You can sign up for a free account and start using the portal to deploy services.

The portal includes a built-in tool called Cloud Shell, which supports both Bash and PowerShell for command-line tasks. You can also create virtual machines by selecting region, availability zone, VM size, authentication method (like SSH key), and OS disk type.

# Azure Infrastructure
Microsoft Azure runs in a global network of physical data centers. These are organized into Availability Zones, which are separate physical locations within a region. A region is a group of zones, like "Central India" or "West Europe". Regions are paired to support disaster recovery and high availability.

