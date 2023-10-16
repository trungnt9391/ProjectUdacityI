# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
Virtual Machine (VM):

Costs: VMs can be more cost-effective if you have a consistent workload and can leverage reserved instances. However, costs may vary depending on the VM size, storage, and bandwidth.
A1(1 cores, 1.75 GB RAM, 40 GB Temporary storage) - Monthly cost $23.36
Scalability: VMs can be scaled vertically (resizing the VM) or horizontally (adding more VM instances), but scaling may require manual intervention.
Availability: VMs can achieve high availability through strategies like Azure Availability Sets or Availability Zones, but it typically requires more manual configuration.
Workflow: Deploying on VMs often involves more management, including OS patching, security updates, and application maintenance.


Azure App Service:

Costs: App Service is a Platform as a Service (PaaS) offering, which can be more cost-effective for smaller to medium-sized applications. It abstracts infrastructure management.
B1( 1 cores(s), 1.75 GB RAM) x730 hours - Monthly cost: $54.75
Scalability: App Service offers easy horizontal scaling with automatic load balancing, enabling your app to handle varying workloads seamlessly.
Availability: App Service includes built-in features for redundancy and failover, making it highly available without significant manual configuration.
Workflow: App Service simplifies deployment and management. You focus on your code and not the underlying infrastructure.
2. Choose the Appropriate Solution (VM or App Service):
For deploying a CMS app, considering the features and nature of the application, Azure App Service is often a more appropriate choice for the following reasons:

Cost-effectiveness: If the CMS app is of moderate size and doesn't require specific VM-level configurations, App Service is often more cost-effective.
Simplicity and speed: App Service simplifies the deployment process and allows you to focus on application development rather than infrastructure management.
Scalability: App Service provides effortless horizontal scalability to handle traffic spikes or growing user numbers.
Availability: Azure App Service has built-in features for high availability and automatic backups.
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
The decision to change from Azure App Service to VMs would be driven by evolving app requirements that demand a higher degree of control, customization, or specialized infrastructure that App Service cannot readily provide. It's crucial to carefully evaluate the changing needs of your CMS app and choose the deployment option that best aligns with those evolving requirements while considering the trade-offs in complexity, management, and cost.
