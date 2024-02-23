# 1. Distributed web infrastructure


<p align="center"><img src="https://github.com/Arzumirzeb/holbertonschool-system_engineering-devops/blob/master/web_infrastructure_design/task_1.png"></p>

## Some specifics about this infrastructure:

A load balancer and an active-passive setup are both integral components in ensuring high availability and reliability for critical systems and applications. Let's delve into each concept and explore how they work together.

#### Load Balancer:
A load balancer serves as a traffic manager, distributing incoming requests across multiple servers or resources. Its primary goal is to optimize resource utilization, prevent any single server from becoming overwhelmed, and ensure that the workload is evenly distributed. Load balancers operate at various layers of the OSI model, including Layer 4 (transport layer) and Layer 7 (application layer), providing different levels of functionality and intelligence.

#### Active-Passive Setup:
An active-passive setup, also known as a failover or standby configuration, involves maintaining duplicate sets of resources, such as servers or databases. In this setup, one set of resources (the active or primary) handles all incoming requests and processes data, while the other set (the passive or standby) remains idle, ready to take over operations in case of a failure or outage. The passive resources continuously replicate data or state from the active resources to ensure synchronization and minimize downtime during failover events.

#### Integration of Load Balancer with Active-Passive Setup:
In an active-passive setup, the load balancer plays a crucial role in routing traffic to the active resources while monitoring their health and availability. If the active resources encounter a failure or become unresponsive, the load balancer detects this condition through health checks or monitoring probes and automatically redirects traffic to the passive resources, which assume the active role. This failover process is transparent to end-users, ensuring continuous service availability and minimal disruption.

####In a Primary-Replica (Master-Slave) cluster,
 the primary node handles all write requests, updating its data and then replicating changes to replica nodes. Replica nodes maintain a copy of the data but only handle read queries, relying on replication from the primary node. The primary node is powerful, handling writes and maintaining data integrity, while replica nodes are simpler, serving as backups and managing read-heavy workloads. This setup ensures high availability, scalability, and fault tolerance for database systems.


## what the issues are with this infrastructure:
In a Primary-Replica cluster, the primary node is a potential single point of failure. Firewall protection is crucial for security, preventing unauthorized access and attacks. HTTPS ensures secure communication, protecting data from interception. Monitoring tools are essential for detecting issues early, ensuring stability, security, and performance.
