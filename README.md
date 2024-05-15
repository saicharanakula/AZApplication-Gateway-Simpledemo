# Deploy Simpleweb app through Azure app gateway

Azure Application Gateway is a web traffic load balancer that enables you to manage traffic to your web applications. Unlike traditional load balancers, which operate at the transport level (OSI Layer 4), Application Gateway can make routing decisions based on additional attributes of an HTTP request, such as URL path or host headers (OSI Layer 7).

**Key Features of Azure Application Gateway:**
Load Balancing: Distributes traffic across multiple servers to ensure high availability and reliability of applications.

SSL Termination: Offloads the SSL decryption work from web servers to the Application Gateway, improving the performance of the backend servers.

Web Application Firewall (WAF): Protects web applications from common threats and vulnerabilities such as SQL injection, cross-site scripting (XSS), and other OWASP top 10 threats.

URL-based Routing: Routes traffic based on URL paths, enabling efficient distribution of traffic to backend servers that handle specific content.

Multi-Site Hosting: Host multiple websites on the same Application Gateway by routing based on the hostname of the incoming request.

Session Affinity: Ensures that requests from a particular user session are directed to the same backend server, often using cookies.

Autoscaling: Automatically scales the number of Application Gateway instances based on traffic load, ensuring high availability and responsiveness during traffic spikes.

Custom Health Probes: Configurable health probes to monitor the status of your backend servers and ensure that traffic is only sent to healthy instances.

**Common Use Cases:**

Web Application Hosting: Efficiently balance the load and enhance security for web applications.

Microservices Architecture: Route requests to different backend services based on the URL path.

Secure Application Delivery: Use SSL termination and WAF to secure web applications.

Multi-Tenant Applications: Host multiple applications or domains on the same infrastructure with URL-based routing and hostname differentiation.

**Integration with Other Azure Services:**

Azure Traffic Manager: For global traffic distribution and failover.

Azure Active Directory: For secure authentication and authorization.

Azure Monitor: For logging, metrics, and diagnostics of Application Gateway.

**Configuration:**

Frontend IP Configuration: Defines the IP addresses and ports that the Application Gateway listens to.

Listeners: Configures the listening rules and conditions for incoming traffic.

Backend Pools: Contains the backend servers that serve the requests.

Routing Rules: Defines how traffic should be routed based on the rules set (e.g., URL-based routing).

