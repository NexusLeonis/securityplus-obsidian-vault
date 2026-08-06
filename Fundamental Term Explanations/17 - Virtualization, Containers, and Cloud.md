# 17. Virtualization, Containers, and Cloud

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.1 - Cloud Infrastructures]] · [[2.3 - Virtualization Vulnerabilities]] · [[2.3 - Cloud-specific Vulnerabilities]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Virtual machine** | A software-based computer with its own operating system and virtual hardware. | A Linux VM runs on a Windows host. | VMs require patching, isolation, and access control. |
| **Hypervisor** | Software or firmware that creates and manages virtual machines. | VMware ESXi or Microsoft Hyper-V. | Hypervisor compromise can affect every hosted VM. |
| **Type 1 hypervisor** | A hypervisor that runs directly on physical hardware. | VMware ESXi on a server. | It normally supports enterprise virtualization. |
| **Type 2 hypervisor** | A hypervisor that runs as an application inside a normal operating system. | VirtualBox on a laptop. | The host operating system adds another security dependency. |
| **Host machine** | The physical system running virtual machines or containers. | A server running ten VMs. | Host compromise can affect all guests. |
| **Guest machine** | A virtual machine running on a host. | A virtual Windows server. | Guests need normal operating-system security controls. |
| **VM escape** | An attack that breaks out of a VM and reaches the host or other VMs. | Malicious code exploits a hypervisor flaw. | Isolation failure can expose multiple workloads. |
| **Container** | An isolated application environment that shares the host operating-system kernel. | A Docker container runs a web application. | Containers start quickly but share more underlying components than VMs. |
| **Container image** | A packaged template used to create containers. | A web-server image includes the application and dependencies. | Malicious or outdated images introduce vulnerabilities. |
| **Container registry** | A repository that stores and distributes container images. | Docker Hub or a private registry. | Organizations must control image trust and access. |
| **Orchestration** | Automated management of many containers or workloads. | Kubernetes deploys and scales containers. | Compromising orchestration systems can affect entire environments. |
| **Cloud computing** | Using computing resources delivered by a provider over a network. | Hosting servers in AWS, Azure, or Google Cloud. | Security responsibilities divide between customer and provider. |
| **Shared responsibility model** | The provider secures some cloud components while the customer secures others. | AWS secures data centers; the customer secures accounts and data. | Many cloud incidents result from misunderstood responsibilities. |
| **IaaS** | Cloud service providing virtual servers, storage, and networking. | Renting virtual machines in AWS. | The customer usually secures operating systems, applications, and data. |
| **PaaS** | Cloud service providing a managed platform for building and running applications. | Deploying code without managing the underlying server. | The provider manages more infrastructure than with IaaS. |
| **SaaS** | Complete software delivered over the Internet. | Microsoft 365 or Salesforce. | Customers still manage users, permissions, configuration, and data. |
| **Public cloud** | Cloud services shared across customers but logically isolated. | A company uses Microsoft Azure. | Misconfiguration can expose resources publicly. |
| **Private cloud** | Cloud-style infrastructure dedicated to one organization. | An internal OpenStack environment. | The organization controls more of the infrastructure and security. |
| **Hybrid cloud** | An environment combining private or on-premises systems with public cloud resources. | Local databases connect to cloud applications. | Security teams must protect connections and policies across environments. |
| **Multi-cloud** | Using services from more than one cloud provider. | AWS for applications and Azure for identity. | Different platforms create inconsistent controls and visibility. |
| **Availability zone** | A separate data-center location inside one cloud region. | Two VMs run in different zones. | Spreading systems across zones improves resilience. |
| **Region** | A geographic area containing cloud data centers. | US East or Europe West. | Region choice affects latency, resilience, and data-location requirements. |
| **Elasticity** | Automatically increasing or decreasing resources as demand changes. | Cloud servers scale up during a sales event. | Attackers may cause unexpected scaling costs. |
| **High availability** | Designing systems to remain available when components fail. | Two servers run behind a load balancer. | Redundancy reduces single points of failure. |
| **Serverless** | A cloud model where the provider runs application code without the customer managing servers. | A function runs when a file uploads. | Customers still secure code, permissions, triggers, and data. |
| **API** | A defined way for software systems to request data or actions from one another. | A mobile app asks a server for account information. | Weak authentication or input validation can expose APIs. |

---
[[00 - Overview|← Overview]]
