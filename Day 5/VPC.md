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
