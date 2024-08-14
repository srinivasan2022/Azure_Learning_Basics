## Load Balancer in Azure :

The term load balancing refers to the distribution of workloads across multiple computing resources. Load balancing aims to optimize resource use, maximize throughput, minimize response time, and avoid overloading any single resource. It can also improve availability by sharing a workload across redundant computing resources.

There are 4 types of load balancing services in Azure :
- 1.Azure Load Balancer
- 2.Azure Application Gateway
- 3.Azure Traffic Manager
- 4.Azure Front Door

#### Azure Load Balancer :
It Effectively and Evently distribute the incoming user request to backend pools.

It opeates at the <mark>OSI 4 layer</mark> .It Support <mark>TCP/UDP</mark> based protocols

##### There are 2 types of load balancer in Azure.
###### 1.Public load balancer -- can be accessed from anywhere.
###### 2.Private or internal load balancer -- Only within the network.

##### Service categorize in Azure load balancer : 
###### 1.Regional service : 
These load balancing service distribute the network traffic within the virtual network.
###### 2.Global service : 
These load balancing service distribute the network traffic regional , clouds or on-premises network.

###### Health Probes :
A Azure load balancer can send the request to active Vm. A active Vm's checked by health probes.A health probe can send the request to each Vm's and if the Vm is active the load balancer can send the request to the virtual machine.

 If the Vm's get down , the load balancer doesn't send the any request to the virtual machine.Azure load balancer support both inbound and outbound scenarios.The end user can get the quick response by using load balancer.

| Sku | Type | Tier |
|----------|----------|----------|
| Basic | Public / Internal | Regional |
| Standard | Public / Internal | Regional / Global |
| Gateway | Internal | Regional |

 ---

![LB](https://github.com/user-attachments/assets/fe9d851b-f96c-4420-970e-c98b9cd65672)