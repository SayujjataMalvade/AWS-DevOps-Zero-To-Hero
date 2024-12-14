# Route 53

## DNS Service Provided by AWS

DNS (Domain Name System) is a service used to translate human-readable domain names into IP addresses, essentially acting as the "phonebook" of the internet. AWS offers DNS services through **Route 53**.

### How DNS Works

1. **User Query:** When you type a domain name (e.g., [www.example.com](https://www.example.com/)) into your browser for the first time, the query is sent to a **DNS resolver**.
   - If the IP address is found in the **cache**, the website is accessed directly.
   - If not, the query moves to the **Root DNS** server.

2. **Root DNS:** The Root DNS server directs the query to the **TLD (Top-Level Domain)** DNS server based on the domain extension (e.g., `.com`, `.org`, `.edu`).

3. **TLD DNS:** The TLD DNS server points to the **authoritative DNS server** hosting the domain, such as AWS Route 53.

4. **Route 53:** The Route 53 DNS server provides the IP address for the domain, which is then stored in the cache for future queries. This allows the user to access the website.

   - On subsequent requests, if the IP address is cached, these intermediate steps are bypassed.

---

## Route 53 Routing Policies

Route 53 offers multiple routing policies to control how traffic is routed:

1. **Simple Routing Policy:** Routes all traffic to a single resource.
2. **Failover Routing Policy:** Automatically redirects traffic to a healthy resource in case of failure.
3. **Geo-location Routing Policy:** Routes traffic based on the geographic location of the user.
4. **Geo-proximity Routing Policy:** Routes traffic based on geographic proximity with optional biasing for specific regions.

Choose a routing policy depending on the requirements of your project.

---

## Health Checks in Route 53

Route 53 includes health checks to monitor and manage the availability of resources. Key features include:

- **Threshold Values:** Define thresholds for health checks to evaluate server status.
- **Traffic Management:** Based on server responses, Route 53 redirects traffic only to healthy servers.

Health checks ensure high availability and reliability by routing traffic to functioning servers while avoiding unhealthy ones.
