## Module 03: Knowledge Check

1. **Question Title:** Which component of the AWS Global Infrastructure does Amazon CloudFront use to ensure low-latency
   delivery? (Select the best answer.)

   **Correct Answer:** AWS edge locations

   **Explanation:** Amazon CloudFront uses a network of edge locations strategically placed around the globe to cache
   content closer to users. This minimizes the distance data needs to travel, resulting in faster delivery and reduced
   latency.

    - **AWS Regions** are larger geographical areas that contain multiple Availability Zones.
    - **AWS Availability Zones** are physically isolated locations within a single region.
    - **Amazon Virtual Private Cloud (Amazon VPC)** allows users to create isolated and secure virtual networks in the
      AWS
      cloud, not directly related to CloudFront's edge network.


2. **Question Title:** You can run applications and workloads from a Region closer to the end users to ______ latency.

   **Correct Answer:** decrease

   **Explanation:** Running applications and workloads from a Region closer to end users helps to **decrease** latency.
   Latency is the time it takes for data to travel between points, so reducing the physical distance between the server
   and the user minimizes the time it takes for data to be transmitted.
3. **Question Title:** True or False? Networking, storage, compute, and databases are examples of service categories
   that AWS offers.

   **Correct Answer:** True

   **Explanation:**  This statement is true. AWS provides a comprehensive suite of cloud services, covering essential
   categories like:

    - **Networking:** AWS offers services for managing virtual networks, routing traffic, connecting resources, and
      more.
    - **Storage:** AWS provides various storage services, including object storage (S3), block storage (EBS), and file
      storage (EFS).
    - **Compute:** AWS offers virtual servers (EC2), serverless computing (Lambda), and container services (ECS, EKS).
    - **Databases:** AWS provides a variety of database services, such as relational databases (RDS), NoSQL databases (
      DynamoDB), and data warehousing (Redshift).
4. **Question Title:** Which of the following are geographic areas that host two or more Availability Zones? (Select the
   best answer.)

   **Correct Answer:** AWS Regions

   **Explanation:**

    - **AWS Regions** are large geographical areas (like US East (N. Virginia), US West (Oregon), etc.) and typically
      contain multiple Availability Zones.
        - This is for high availability and fault tolerance.

    - **Availability Zones** are physically separate data centers within a Region, designed to be resilient to failures
      in a single location.
    - **Edge locations** are points of presence for content delivery (like CloudFront) but do not house core compute or
      storage services.
    - The term "AWS Origins" is not a standard AWS term.


5. **Question Title:** ______ means the infrastructure has built-in component redundancy and ______ means that resources
   dynamically adjust to increases or decreases in capacity requirements.

   **Correct Answer:**  Fault tolerant, Elastic and scalable

   **Explanation:**

    - **Fault tolerant:** This means the system is designed to withstand failures of individual components. Redundancy (
      having backups or multiple copies of components) is a key aspect of fault tolerance.
    - **Elastic and scalable:**  This means the system can automatically adjust its capacity to handle changes in
      demand. The system can scale up to handle increased load or scale down to reduce costs when demand decreases.

6. **Question Title:** True or False? Availability Zones within a Region are connected through low-latency links.

   **Correct Answer:** True

   **Explanation:** This statement is true. Availability Zones within the same AWS Region are designed to be highly
   connected with low-latency network links. This allows for fast communication between resources located in different
   Availability Zones within the same Region, which is crucial for:

    - **High Availability:**  If one Availability Zone experiences an outage, applications running in other Availability
      Zones can still communicate and function.
    - **Fault Tolerance:**  Low-latency links between Availability Zones enable the rapid failover of applications and
      data in case of a failure in one zone.

7. **Question Title:** Which of these statements about Availability Zones is not true? (Select the best answer.)

   **Correct Answer:** A data center can be used for more than one Availability Zone.

   **Explanation:**

    - **Availability Zones** are designed to be physically isolated within a Region. A single data center is typically
      dedicated to a single Availability Zone to ensure that failures in one zone do not impact others.

    - The other statements are true:
        - Availability Zones are designed for fault isolation.
        - Availability Zones are made up of one or more data centers.
        - Availability Zones are connected to each other using high-speed private links.


8. **Question Title:** What is true about Regions? (Choose two.)

   **Correct Answer:**
    - Each Region is located in a separate geographic area.
    - A Region is a physical location that has multiple Availability Zones.

9. **Question Title:** AWS highly recommends provisioning your compute resources across ______ Availability Zones. (
   Select the best answer.)

   **Correct Answer:** multiple

   **Explanation:** AWS strongly recommends distributing compute resources across multiple Availability Zones within a
   Region to achieve high availability and fault tolerance. If one zone experiences an outage, applications and services
   running in other zones can continue operating.

   The other options are incorrect:

    - **All:** It's not necessary or always practical to deploy across all Availability Zones in a Region.
    - **No:** This would create a single point of failure, making the application vulnerable to outages.
    - **Single:**  Deploying resources in a single Availability Zone is generally not considered a best practice for
      resilience.

10. **Question Title:** True or False? Edge locations are only located in the same general area as Regions.

    **Correct Answer:** False

    **Explanation:** This statement is false. Edge locations, used for services like CloudFront, are designed to be
    distributed globally to be closer to users, often in different locations than AWS Regions. Regions are larger, more
    centralized areas that house core compute and storage resources. Edge locations are a distinct network for content
    delivery and caching. 




