# What Is Scalability? 🚀

Scalability describes a system’s elasticity. While we often use it to refer to a system’s ability to grow according to user traffic, it is not exclusive to this definition. We can scale down, scale up, and scale out accordingly.

## What Is Horizontal Scaling? ⬇️⬆️

Horizontal scaling (aka scaling out) refers to adding additional nodes or machines to your infrastructure to cope with new demands.

<img align="left" display="flex" alt="coding" width="50%" src="https://i.postimg.cc/XYqS9J62/image.png">
<br clear="left">

## What Is Vertical Scaling? ⬆️

Vertical scaling (aka scaling up) describes adding additional resources to a system so that it meets current user demand.

<img align="left" display="flex" alt="coding" width="50%" src="https://i.postimg.cc/fy3ZDRWq/image.png">
<br clear="left">


## Horizontal Vs. Vertical Scaling: At a Glance 🔄

|                                |                                                                                                                         |                                                                                                |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
|                                | **Horizontal scaling**                                                                                                  | **Vertical scaling**                                                                           |
| **Description**                | Increase or decrease the number of nodes in a cluster or system to handle an increase or decrease in workload           | Increase or decrease the power of a system to handle increased or reduced workload             |
| **Example**                    | Add or reduce the number of virtual machines (VM) in a cluster of VMs                                                   | Add or reduce the CPU or memory capacity of the existing VM                                    |
| **Execution**                  | Scale in/out                                                                                                            | Scale up/down                                                                                  |
| **Workload distribution**      | Workload is distributed across multiple nodes.<br><br>Parts of the workload reside on these different nodes             | A single node handles the entire workload.                                                     |
| **Concurrency**                | Distributes multiple jobs across multiple machines over the network, at a go. This reduces the workload on each machine | Relies on multi-threading on the existing machine to handle multiple requests at the same time |
| **Required architecture**      | Distributed                                                                                                             | Any                                                                                            |
| **Implementation**             | Takes more time, expertise, and effort                                                                                  | Takes less time, expertise, and effort                                                         |
| **Complexity and maintenance** | Higher                                                                                                                  | Lower                                                                                          |
| **Configuration**              | This requires modifying a sequential piece of logic in order to run workloads concurrently on multiple machines         | No need to change the logic. The same code can run on a higher-spec device                     |
| **Downtime**                   | No                                                                                                                      | Yes                                                                                            |
| **Load balancing**             | Necessary to actively distribute workload across the multiple nodes                                                     | Not required in the single node                                                                |
| **Failure resilience**         | Low because other machines in the cluster offer backup                                                                  | High since it’s a single source of failure                                                     |
| **Costs**                      | High costs initially; optimal over time                                                                                 | Low-cost initially; less cost-effective over time                                              |
| **Networking**                 | Quick inter-machine communication                                                                                       | Slower machine-to-machine communication                                                        |
| **Performance**                | Higher                                                                                                                  | Lower                                                                                          |
| **Limitation**                 | Add as many machines as you can                                                                                         | Limited to the resource capacity the single machine can handle                                 |

## Horizontal Scaling Vs. Vertical Scaling: An In-Depth Look 📊

<img align="left" display="flex" alt="coding" width="50%" src="https://i.postimg.cc/85BRbM2M/image.png">
<br clear="left">

### Advantages of Horizontal Scaling 🌐

- **Scaling is easier from a hardware perspective** – All horizontal scaling requires you to do is add additional machines to your current pool. It eliminates the need to analyze which system specifications you need to upgrade.
- **Fewer periods of downtime** – Because you’re adding a machine, you don’t have to switch the old machine off while scaling. If done effectively, there may never be a need for downtime and clients are less likely to be impacted.
- **Increased resilience and fault tolerance** – Relying on a single node for all your data and operations puts you at a high risk of losing it all when it fails. Distributing it among several nodes saves you from losing it all.
- **Increased performance** – If you are using horizontal scaling to manage your network traffic, it allows for more endpoints for connections, considering that the load will be delegated among multiple machines.

### Disadvantages of Horizontal Scaling ⚖️

- **Increased complexity of maintenance and operation** – Multiple servers are harder to maintain than a single server is. Additionally, you will need to add software for load balancing and possibly virtualization. Backing up your machines may also become a little more complex. You will need to ensure that nodes synchronize and communicate effectively.
- **Increased Initial costs** – Adding new servers is far more expensive than upgrading old ones.

### Advantages of Vertical Scaling 📈

- **Cost-effective** – Upgrading a pre-existing server costs less than purchasing a new one. Additionally, you are less likely to add new backup and virtualization software when scaling vertically. Maintenance costs may potentially remain the same too.
- **Less complex process communication** – When a single node handles all the layers of your services, it will not have to synchronize and communicate with other machines to work. This may result in faster responses.
- **Less complicated maintenance** – Not only is maintenance cheaper but it is less complex because of the number of nodes you will need to manage.
- **Less need for software changes** – You are less likely to change how the software on a server works or how it is implemented.

### Disadvantages of Vertical Scaling ⚖️

- **Higher possibility for downtime** – Unless you have a backup server that can handle operations and requests, you will need some considerable downtime to upgrade your machine.
- **Single point of failure** – Having all your operations on a single server increases the risk of losing all your data if a hardware or software failure was to occur.
- **Upgrade limitations** – There is a limitation to how much you can upgrade a machine. Every machine has its threshold for RAM, storage, and processing power.

## Which Should You Choose? 🤔

Both horizontal and vertical scaling have their own benefits and limitations. Since there isn’t a one-size-fits-all solution for organizations, you need to scale according to your needs and resources. Here are a few factors to consider along with which type of scaling suits the situation best:

- **Cost** – Initial hardware costs for horizontal upgrades are higher. If you are working on a tight budget and need to add more resources to your infrastructure quickly and cheaply, then vertical scaling may be the best option for you.
- **Future-proofing** – Adding additional updated machines through horizontal scaling will increase the overall performance threshold of your organization. There is a limit to how much you can vertically scale a single node and it may not be able to handle the demands of the future.
- **Topographic distribution** – If you plan to have nationwide or global clients, it is unreasonable to expect them all to access your services from a single machine in a single location. In a situation like this, you’ll need to horizontally scale your resources to maintain your service level agreement (SLA).
- **Reliability** – Horizontal scaling may offer you a more reliable system. It increases redundancy and ensures that you are not relying on a single machine. If one machine fails, another may be able to pick up the slack temporarily.
- **Upgradability and flexibility** – If you are running your application’s tiers on individual machines, they are easier to decouple and upgrade without any downtime.
- **Performance and complexity** – Performance will depend on how your services work and how they are interconnected. Simple straightforward applications won’t benefit much from being run on multiple machines. In fact, it may degrade its quality. Sometimes it’s better to leave the application as is and upgrade the hardware to meet demand. Horizontal scaling may require you to rewrite the code or add a virtual machine that unifies all the servers.

## Horizontal Vs. Vertical Scaling: Use Cases 🔍

Here are examples of when it is best to use either scaling approach to optimize your workloads.

### Use vertical scaling when:

- You’ve verified with your engineers and other stakeholders that increasing a machine's capabilities, such CPUs and memory capacity, will deliver the price-performance level your workloads require
- If you’re just starting out; you don’t know how consistent the traffic is or how many users you’ll get
- Want to use your existing system internally and a cloud provider services for the bulk of customer-facing solutions
- You know redundancy is not feasible or required to operate optimally
- Upgrades are few and far between, so there is little downtime to worry about
- You have a legacy app that doesn’t require distributed or high scalability

### Use horizontal scaling when:

- Providing high-quality service requires high performance
- Backup machines are necessary to reduce single points of failure
- You want more flexibility to configure your machines in different ways to increase efficiency, such as the price-performance ratio
- You need to run your application or services across different geographical locations at low latency
- Updating, upgrading, and optimizing your system regularly is imperative — all without increasing downtime
- You are sure that your usage, users, or traffic are consistently high or will be growing exponentially soon
- You have the people and resources to buy, install, and maintain additional hardware and software
- You are using a micro-services architecture or containerized applications, which achieve better performance on a distributed system
