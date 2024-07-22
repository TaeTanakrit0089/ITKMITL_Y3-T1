## Module 04: Knowledge Check

1. **Question Title:** In the shared responsibility model, AWS is responsible for providing what? (Select the best
   answer.)

   **Correct Answer:** Security of the cloud

   **Explanation:** In the shared responsibility model, AWS is responsible for the "security of the cloud." This means
   they are responsible for securing the underlying infrastructure, including the hardware, networking, and data
   centers.

    - **Security to the cloud** and **Security for the cloud** are not standard terms used in the shared responsibility
      model.
    - **Security in the cloud** refers to the security measures that customers are responsible for within their
      applications and data.

   The shared responsibility model emphasizes that while AWS secures the cloud itself, customers are responsible for
   securing their applications, data, and user access within the cloud environment.


2. **Question Title:** In the shared responsibility model, which of the following are examples of "security in the
   cloud"? (Choose two.)

   **Correct Answer:** Security group configurations, Encryption of data at rest and data in transit

   **Explanation:**

    - **Security group configurations:** Security groups act as virtual firewalls that control inbound and outbound
      network traffic for resources in the cloud. These configurations are part of "security in the cloud" as they are
      customer-managed.
    - **Encryption of data at rest and data in transit:**  Encryption helps protect data confidentiality, both when
      stored (at rest) and when transmitted (in transit). This is a core responsibility of the customer within the
      shared responsibility model.

   The other options are examples of "security of the cloud," which AWS is responsible for:

    - **Compliance with compute security standards and regulations:** AWS is responsible for adhering to security
      standards and regulations for its infrastructure and services.
    - **Physical security of the facilities in which the services operate:** This is the responsibility of AWS to secure
      its data centers and physical infrastructure.
    - **Protecting the global infrastructure:** This is a broad responsibility of AWS to maintain the security of its
      cloud infrastructure.
3. **Question Title:** Which of the following is the responsibility of AWS under the AWS shared responsibility model? (
   Select the best answer.)

   **Correct Answer:** Maintaining physical hardware

   **Explanation:** AWS is responsible for maintaining the physical hardware that makes up its cloud infrastructure.
   This includes the servers, storage devices, networking equipment, and data centers.

    - **Configuring third-party applications** is typically the customer's responsibility.
    - **Security application access and data** is also primarily the responsibility of the customer.
    - **Managing custom Amazon Machine Images (AMIs)** is a customer responsibility, although AWS offers tools and
      services to facilitate this.

   The shared responsibility model divides security responsibilities between AWS (the cloud provider) and the customer.
   AWS takes care of the physical security of the cloud infrastructure, while customers are responsible for securing
   their applications, data, and user access.
4. **Question Title:** When creating an AWS Identity and Access Management (IAM) policy, what are the two types of
   access that can be granted to a user? (Choose two.)

   **Correct Answer:**  Programmatic access, AWS Management Console access

   **Explanation:**

    - **Programmatic access:** This allows users to interact with AWS services through code, scripts, or automated
      tools (like the AWS CLI or SDKs).
    - **AWS Management Console access:**  This provides users with access to the web-based interface for managing AWS
      services.

   The other options are not standard access types in IAM:

    - **Institutional access:** This is not a recognized term in IAM.
    - **Authorized access:**  While access is always authorized in IAM, this is not a distinct access type.
    - **Administrative root access:**  This is a special type of access for the root account, not typically granted to
      individual users.
5. **Question Title:** True or False? AWS Organizations enables you to consolidate multiple AWS accounts so that you
   centrally manage them.

   **Correct Answer:** True

   **Explanation:** This statement is true. AWS Organizations is a service specifically designed to help organizations
   manage multiple AWS accounts centrally. It allows you to:

    - **Consolidate accounts:**  Create a hierarchy of accounts, grouping them into organizational units (OUs) for
      easier management.
    - **Centralize governance:**  Establish policies, controls, and compliance requirements for the entire organization,
      applying them across all accounts.
    - **Improve security:**  Streamline security management and enforce consistent security controls across multiple
      accounts.

   AWS Organizations is a valuable tool for organizations that need to manage and govern their AWS environment across
   multiple accounts.


6. **Question Title:** Which of the following are best practices to secure your account using AWS Identity and Access
   Management (IAM)? (Choose two.)

   **Correct Answer:** Manage access to AWS resources, Define fine-grained access rights

   **Explanation:**

    - **Manage access to AWS resources:**  This is a fundamental principle of IAM. It involves granting the least amount
      of privilege necessary for each user to perform their tasks, minimizing the risk of unauthorized access.
    - **Define fine-grained access rights:** This involves setting specific permissions for users and groups, allowing
      them to access only the resources they need to do their jobs. This approach promotes security by reducing the
      potential for accidental or malicious misuse of resources.

   The other options are not best practices:

    - **Provide users with default administrative privileges:** Granting default administrative privileges is a major
      security risk as it gives users broad access to sensitive resources and operations.
    - **Leave unused and unnecessary users and credentials in place:**  This is a security vulnerability as inactive
      accounts can be a target for compromise. Regularly reviewing and disabling unused accounts and credentials is
      essential.
    - **Avoid using IAM groups to grant the same access permissions to multiple users:**  Using IAM groups effectively
      can streamline permission management, but it's crucial to define groups carefully and ensure they only include
      users with similar roles and responsibilities.

   In short, proper IAM management involves defining clear access policies, limiting privileges, and regularly auditing
   accounts and permissions.


7. **Question Title:** Which of the following should be done by the AWS account root user? (Select the best answer.)

   **Correct Answer:** Change the AWS support plan

   **Explanation:**

   The AWS account root user has the highest level of privileges and can perform actions that affect the entire AWS
   account. Changing the AWS support plan is a high-level administrative action that only the root user can perform.

   The other options are not typically done by the root user:

    - **Secure access for applications:** This is typically handled by IAM policies and roles.
    - **Integrate with other AWS services:**  This is usually done through code, scripts, or the AWS Management Console.
    - **Change granular permissions:** Granular permissions are managed through IAM policies and roles, not directly by
      the root user.

   It's highly recommended to avoid using the root account for everyday tasks and instead create and manage IAM users
   with specific permissions. The root account should only be used for essential actions and for creating the first IAM
   users.
8. **Question Title:** After initial login, what does AWS recommend as the best practice for the AWS account root
   user? (Select the best answer.)

   **Correct Answer:** Delete the AWS account root user
9. **Question Title:** How would a system administrator add an additional layer of login security to a user's AWS
   Management Console? (Select the best answer.)

   **Correct Answer:** Enable multi-factor authentication

   **Explanation:** Enabling multi-factor authentication (MFA) is the most effective way to add an extra layer of
   security to logins. MFA requires users to provide more than just a password, such as a one-time code from a mobile
   app or a physical security key, to verify their identity.

    - **Use Amazon Cloud Directory:**  This service is for managing user directories, not specifically for enhancing
      login security.
    - **Audit AWS Identity and Access Management (IAM) roles:** Auditing IAM roles is important for security, but it's
      not a method for directly enhancing login security.
    - **Enable AWS CloudTrail:** CloudTrail is a service that logs events in your AWS account, but it doesn't directly
      impact login security.


10. **Question Title:** True or False? AWS Key Management Service (AWS KMS) enables you to assess, audit, and evaluate
    the configurations of your AWS resources.

    **Correct Answer:** False
      
    **Explanation:**  AWS Key Management Service (AWS KMS) is primarily focused on managing encryption keys. While it
    provides auditing capabilities for key usage and access, it's not designed to assess, audit, and evaluate the
    configurations of all your AWS resources.

    - For assessing and auditing configurations, you'd typically use services like AWS Config and AWS CloudTrail.
    - AWS Config continuously monitors and assesses the configurations of your resources against rules you define.
    - AWS CloudTrail logs events related to your AWS account, which can be used for auditing and security analysis. 









