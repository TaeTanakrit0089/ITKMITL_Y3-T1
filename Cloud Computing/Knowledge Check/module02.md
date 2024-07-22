## Module 02: Knowledge Check
**1. Which is the best definition of cloud architecture?**

* **Correct:** Applying cloud characteristics to a solution that uses cloud services and features to meet technical and business requirements.

  * **Explanation:**  Cloud architecture goes beyond simply using cloud infrastructure. It's about leveraging cloud-native principles (like scalability, elasticity, pay-as-you-go) to design and build systems that are efficient, adaptable, and meet specific needs.

**2. AWS Well-Architected Framework - Missing Pillars**

* **Correct:**
  * **Reliability:** The ability of a system to recover from infrastructure or service disruptions, dynamically acquiring resources to meet demand and mitigating disruptions.
  * **Cost optimization:**  Avoiding unnecessary costs.  This involves using resources efficiently, selecting the right pricing models, and optimizing continually over time.

**3. Operational Excellence Pillar Actions**

* **Correct:**
  * **Apply software engineering principles and methodology to infrastructure as code.**  This promotes consistency, repeatability, and automation in managing infrastructure.
  * **Review and improve processes and procedures on a continuous cycle.**  Operational excellence is about constant improvement, identifying areas for optimization, and refining processes.

**4. AWS Best Practices for Frontend/Backend Design**

* **Correct:**  Design the web tier to communicate with the application tier through the Elastic Load Balancing (ELB) service.

  * **Explanation:**  ELB distributes incoming traffic across multiple application servers, enhancing availability and fault tolerance. This is a core AWS best practice for scalable web applications.

**5. AWS Best Practices for Handling Server Failures**

* **Correct:** Amazon CloudWatch detects a system failure. It initiates automation to provision a new server.

  * **Explanation:**  This aligns with AWS principles of automation and minimizing downtime. CloudWatch can monitor for server failures and trigger automated responses like launching a new instance.

**6. Cost Efficiency for On-Premises to Cloud Migration**

* **Correct:** Provision the servers that are needed and stop services when they are not being used.

  * **Explanation:** One of the biggest advantages of the cloud is its pay-as-you-go model.  By only running resources when necessary, you optimize costs.

**7. AWS Best Practices for Read-Only Data with Global Users**

* **Correct:** Use a bucket in the AWS Region that is closest to the company headquarters. All users access the data through Amazon CloudFront.

  * **Explanation:** This combines cost efficiency (data stored in one region) with global performance (CloudFront's CDN caches content closer to users worldwide).

**8. Securely Granting Temporary Access to a Large S3 Object**

* **Correct:** Create a presigned URL to the object that expires in 24 hours, and give it to the consultant.

  * **Explanation:** This is the most secure and time-limited approach. The consultant gets temporary access without needing permanent credentials, and the link automatically expires.

**9. Main Considerations for Choosing AWS Regions**

* **Correct:**
  * **Latency reduction for end users:** Choose regions closest to your users for optimal performance.
  * **Compliance with laws and regulations:** Data residency and compliance requirements often dictate specific regions.

**10. Main Considerations for Choosing Availability Zones**

* **Correct:**
  * **Application resiliency during system failures:**  AZs are physically separated within a region, providing fault tolerance.
  * **Protection against localized natural disasters:** AZs protect against events impacting a single data center within a region. 
