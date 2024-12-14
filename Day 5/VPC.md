# Virtual Private Cloud (VPC)

A Virtual Private Cloud in AWS is a logically isolated network where resources like virtual servers (EC2 instances) can be created and managed. 

## Key Components of a VPC

- **Network Range:** Defines the IP address range for the VPC.
- **Subnets:** Subdivisions of the network range.
- **Route Table:** Specifies the traffic flow paths.
- **Internet Gateway (IGW):** Enables internet connectivity.
- **NAT Gateway:** Allows private resources to access the internet securely.

Every AWS region includes a **default VPC**, which comes pre-configured with subnets, an internet gateway, and a route table.

---

## Subnet

A **subnet** is used to divide the VPC's network into smaller segments. Subnets facilitate better organization and isolation of resources. For instance, in an organization, different teams like:

- Sales Team
- Developer Team
- Cloud Team
- DevOps Team

Each team has distinct tasks, so subnets can be allocated to them for coordination while keeping the network within the organization consistent and secure.

---

## Route Table

A **route table** defines the path for network traffic within the VPC and beyond. It determines where the traffic should flow and specifies routes for destinations, such as:

- Internet Gateway for external internet access.
- NAT Gateway for private resources to access the internet.
- Peering connections or other subnets for internal communication.

---

## Security Group

A **security group** is a core component of security that operates at the **ENI (Elastic Network Interface) level**, meaning it applies to individual EC2 instances. It is:

- **Stateful:** If an inbound rule is created, the corresponding outbound rule is automatically applied.
- Configured with rules that specify the protocols, port numbers, and IP ranges allowed to access the EC2 instance.
- Used to restrict or allow traffic based on IP and port-level configurations.

---

## Network Access Control List (NACL)

A **NACL** operates at the **subnet level** and provides an additional layer of security. Key points include:

- Works with the five security layers in the cloud: ENI, Subnet, Load Balancer, WAF, and Firewall.
- **Stateless:** Inbound and outbound rules must be explicitly defined, and the rules are evaluated based on a priority list.
- Useful for defining fine-grained control over traffic entering or leaving a subnet.
