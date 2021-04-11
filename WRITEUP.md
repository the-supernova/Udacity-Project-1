# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
------
For the project deployment, out of the choices between Virtual Machine and App Service, I chose to deploy the application through App Services keeping in mind the following analysis:-

**Cost**:

Azure App Services are more convenient to opt owing to their flexible service plans. App Services tend to be much cheaper as compared to Virtual Machines. On the other hand, Virtual Machines can be deallocated in order to cut some costs.

**Scalability**:

Both VMs and App Services can be scalable. Multiple VMs can be grouped to provide high availability, scalability and redundancy via Virtual Machine Scale Sets and Load Balancers. Whereas in App Services, we have Auto Scaling service built-in.

**Availability**:

In terms of availability, VMs generally have more availability than App Services, but require extra setup and configuration to be fault tolerant and avoid downtimes during maintenance and upgrades.

**Workflow**:

Virtual Machines provide infrastructure as a service(IaaS) by allowing users full access and control of the VM, but they can be more time consuming for the user to customize and maintain the software that runs on VM. App Services, on the other hand, are classified as platform as a service(PaaS), it allows user to integrate the app without managing the underlying infrastructure.

Considering all the points covered above, choosing App Service would be a justified choice since it is better for lightweight services and it allows the user to focus on the application while Azure takes care of the infrastructure. Azure App Services also provide a variety of deployment options that can be easily integrated into production workflow and satisfy different user needs with their flexible plans.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

In the case of integrating new features to the application, it would need to be updated for more compute capability to prevent rising costs, also we need to take into consideration the hardware limitations of App Services. This would lead us to opt for a VM service. This would also allow us to customize the image according to the working of application, custom monitoring and logging, to enable high performance compute services.