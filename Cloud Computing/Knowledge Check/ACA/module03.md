## Module 03 Knowledge Check

**1. Which statement reflects a design principle of the security pillar of the Well-Architected Framework?**

* **Correct:**  Apply security at all layers of an architecture.
    * **Explanation:** Defense in depth is a core concept of security. The Well-Architected Framework emphasizes
      layering security controls throughout your architecture, not just at the perimeter.

**2. Which statements about responsibility are accurate based on the AWS shared responsibility model? (Select TWO.)**

* **Correct:** AWS is responsible for the physical security of data centers.
    * **Explanation:**  Physical security of data centers (physical access controls, environmental controls, etc.) falls
      under AWS's responsibility.
* **Correct:** Customers are responsible for managing their user data.
    * **Explanation:**  While AWS provides services to help secure data, ultimately, customers are responsible for
      implementing security controls to protect their data in use, at rest, and in transit.

**3. Which options are characteristics of the principle of least privilege? (Select TWO.)**

* **Correct:** Craft security policies that limit access to specific tasks.
    * **Explanation:**  The core idea is to give users/entities only the permissions they need to perform their specific
      job, and nothing more.
* **Correct:** Grant access only as needed.
    * **Explanation:**  Permissions should be granted on a "need-to-know" and "need-to-use" basis. If access is no
      longer required, it should be revoked.

**4. Which statement about AWS Identity and Access Management (IAM) is true?**

* **Correct:** With IAM, you can grant principals granular access to resources.
    * **Explanation:** IAM enables you to define very specific permissions (down to the API action level) for users,
      roles, and services within your AWS account.

**5. Which statements describe AWS Identity and Access Management (IAM) roles? (Select TWO.)**

* **Correct:** They provide temporary security credentials.
    * **Explanation:** When an entity assumes an IAM role, it receives temporary credentials that expire after a defined
      duration.
* **Correct:** Individuals, applications, and services can assume roles.
    * **Explanation:** Roles are not tied to specific users. They can be assumed by users, AWS services, or applications
      running on EC2 instances, for example.

**6. Which statement reflects a best practice for the root user on an AWS account?**

* **Correct:** Create an admin user and perform most admin tasks with this user instead of the root user.
    * **Explanation:** Best practice is to secure the root user with a strong password and MFA, then create an IAM user
      with administrative privileges for day-to-day tasks. This limits the risk of accidental or malicious activity
      using the root account.

**7. How does AWS Identity and Access Management (IAM) evaluate a policy?**

* **Correct:** It checks for explicit deny statements before it checks for explicit allow statements.
    * **Explanation:** IAM policies follow an "explicit deny overrides" approach. If a deny statement matches the
      request, access is denied, even if an allow statement also matches.

**8. Which statement about AWS Identity and Access Management (IAM) policies is accurate?**

* **Correct:** Identity-based policies are attached to a user, group, or role.
    * **Explanation:** Identity-based policies specify permissions granted to an identity (user, group, role).
      Resource-based policies, on the other hand, are attached to resources.

**9. Which AWS Identity and Access Management (IAM) policy element includes information about whether to allow or deny a
request?**

* **Correct:** Effect
    * **Explanation:** The "Effect" element in an IAM policy defines whether the policy allows or denies access. It
      takes either "Allow" or "Deny" as values.

**10. Which option accurately describes the statement element in an AWS Identity and Access Management (IAM) policy?**

* **Correct:** The statement element contains other elements that together define what is allowed or denied.
    * **Explanation:** The "Statement" element is the core building block of an IAM policy. It contains elements like "
      Effect," "Action," "Resource," "Condition," and "Principal" that work together to define the permissions being
      granted or denied. 
