## Azure Application Gateway :
 
The Application Gateway is the one of the load balancer in Azure that allows you to manage the traffic to the web application.It operates at <mark>OSI 7 layer (Application layer)</mark>. It supports HTTP / HTTPS protocols. A virtual machine or backend servers can be associated with Application Gateway backend pool.
The Application Gateway routing the traffic based on additional attributes of the HTTP request (URL path or host headers).

**Example :**  If \signup is in the incoming URL , we can route the traffic to a specific set of servers(signup -- backend pool). If \login is in the incoming URL , we can route the traffic to a another pool(login -- backend pool).

We can upload the custom error pages and route the multiple website using by Application Gateway.
Application Gateway supports <mark>autoscaling , TLS offloading , web application firewall (WAF) , cookie-based session affinity , URL path-based routing , multisite hosting.</mark>

The <mark>subnet is required</mark> for creates the Application Gateway.The Application Gateway is deployed in it's subnet.The Application Gateway occupies the whole IP addresses of the subnet for scaling purpose (If we enable the scaling setting , the scaling VM's or servers are deployed in that subnet).It is a dedicated subnet for Application Gateway.

###### Performance Enhancement :

Tha Application Gateway is available under a <mark>Standard_v2 Sku</mark>.
The V2 Sku offers ,
- Auto Scaling
- Zone redundancy
- Static IP

The WAF V2 Sku includes Web Application Firewall.



![AppGW](https://github.com/user-attachments/assets/3e22a709-7ed2-4ece-b132-52278d68135a)