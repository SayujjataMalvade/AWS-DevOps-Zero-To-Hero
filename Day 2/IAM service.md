# What is IAM?

**Identity and Access Management (IAM)** is a service provided by **AWS** that allows you to:

- Create **IAM Users**, **Groups**, and **IAM Roles**.
- Authorize users and assign permissions based on project requirements, such as **read** or **write** permissions.
- Ensure only authorized individuals can manage project resources, aligning with AWS **security best practices**.

### Key Features of IAM
- **Global Service:** IAM operates globally, meaning it is not tied to a specific AWS region.
- **IAM Users:** Can belong to multiple IAM groups.
- **IAM Roles:** Are specific to particular AWS services.

### Components of IAM

1. **User Policies:**  
   When creating a user, you need to assign them access to AWS resources. Policies are used to define and grant these permissions.

2. **Groups:**  
   In an organization, a user may be part of multiple projects, requiring them to belong to multiple groups. IAM enables users to be part of multiple groups as needed.

IAM ensures secure and efficient access management for AWS resources.

# Root User

The **Root User** is a superuser in AWS with the highest level of authority. Key features of the Root User include:

- Full control over AWS resources.
- Ability to **create**, **delete**, and **deploy** applications on AWS resources.
- Can create and delete other IAM users.
- **Restriction:** No IAM user has the privilege to delete the Root User.

The Root User is essential for managing critical aspects of an AWS account but should be used sparingly to ensure security.

