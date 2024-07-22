## Module 07: Knowledge Check

1. **Question Title:** True or False? Amazon Simple Storage Service (Amazon S3) is an object storage suitable for the
   storage of flat files like Microsoft Word documents, photos, etc.

   **Correct Answer:** True

   **Explanation:** This statement is true. Amazon S3 is an object storage service that's widely used for storing
   various types of data, including:

    - **Flat files:** This includes files like Word documents, PDFs, images, and videos.
    - **Other data:** S3 is also suitable for storing backups, logs, application data, and more.

   S3 offers high availability, scalability, and durability, making it a popular choice for storing a variety of data
   types.


2. **Question Title:** Amazon S3 replicates all objects ______. (Select the best answer)

   **Correct Answer:** in multiple Availability Zones within the same Region

   **Explanation:**

    - Amazon S3 replicates objects by default across multiple Availability Zones within the same Region. This provides
      high availability and fault tolerance, ensuring data is protected even if one Availability Zone experiences an
      outage.

    - **on multiple volumes within an Availability Zone:**  This is not a replication strategy for S3. S3 uses a
      distributed storage model where objects are spread across multiple servers.
    - **across multiple Regions for higher durability:** While S3 offers cross-Region replication as an option for even
      higher durability, it's not the default behavior.
    - **on multiple S3 buckets:** Replicating objects within the same bucket doesn't ensure high availability; the
      objects are still stored in the same physical location.
3. **Question Title:** Which of the following can be used as a storage class for an S3 object lifecycle policy? (Choose
   three)

   **Correct Answer:**
    - S3 - Standard Access
    - S3 - Infrequent Access
    - Simple Storage Service Glacier

   **Explanation:**

    - **S3 - Standard Access:**  This is the default storage class for S3 objects and is suitable for frequently
      accessed data.
    - **S3 - Infrequent Access:** This class is optimized for data that is accessed less frequently (e.g., backups,
      archives). It offers lower storage costs than Standard Access.
    - **Simple Storage Service Glacier:**  This is a very low-cost storage class designed for data that is accessed
      rarely (e.g., long-term backups, historical data). Retrieval of data from Glacier can take several hours.

   The other options are incorrect:

    - **AWS Storage Gateway:**  This is a service that provides a hybrid storage solution, enabling you to connect
      on-premises storage to AWS. It's not a storage class for S3 objects.
    - **S3 - Reduced Redundancy Storage:** This class offered lower storage costs but with reduced data durability. It
      was deprecated in 2020.
    - **Amazon Dynamo DB:** This is a NoSQL database service and not a storage class for S3.

   S3 lifecycle policies allow you to manage the storage class of objects over time, moving them to different storage
   classes based on their access patterns or age, optimizing costs and storage strategies.


4. **Question Title:** The name of an S3 bucket must be unique ______. (Select the best answer)

   **Correct Answer:** worldwide across all AWS accounts

   **Explanation:**

    - S3 bucket names must be unique globally across all AWS accounts. This ensures that there are no naming conflicts
      when accessing objects in different accounts.

    - **within a Region:** Bucket names are not unique within a Region; they need to be unique globally.
    - **across all your AWS accounts:**  Bucket names are not unique within a single account; they need to be unique
      worldwide.
    - **within your AWS account:**  Bucket names must be unique across all AWS accounts, not just within a single
      account.


5. **Question Title:** You can use Amazon Elastic File System (Amazon EFS) to: (Select the best answer)

   **Correct Answer:** implement storage for Amazon EC2 instances that multiple virtual machines can access at the same
   time.

   **Explanation:**

    - **Amazon EFS** is designed to provide a shared file system that can be accessed by multiple EC2 instances
      simultaneously. It offers a way to mount a network file system to your instances, making it ideal for scenarios
      where multiple machines need to share data.

    - The other options are incorrect:

        - **provide simple, scalable, elastic file storage for use only within AWS:** While EFS is simple, scalable, and
          elastic, it's not limited to use within AWS. You can access EFS from both AWS and on-premises systems.
        - **host a robust CDN to deliver entire web sites with dynamic, static, and streaming content:** This is a use
          case for Amazon CloudFront, a Content Delivery Network (CDN) service. EFS is not designed for this purpose.
        - **generate user-specific content:** EFS is a file storage service, not a content generation service. It's used
          to store and share data, not to create new content.

6.**Question Title:** Amazon Elastic Block Store (Amazon EBS) is recommended when data ______ and ______. (Choose two)

**Correct Answer:**

- must be quickly accessible
- requiring long-term persistence

**Explanation:**

- **Amazon EBS** is a block storage service that provides persistent storage for EC2 instances. It's designed for data
  that needs to be quickly accessible and requires long-term persistence.

- The other options are incorrect:

    - **requires object-level storage:**  Object storage is typically handled by S3 (Simple Storage Service). EBS is for
      block storage, which is more suitable for storing data that needs to be accessed like a traditional hard drive.
    - **requires an encryption solution:** While EBS supports encryption, it's not the primary reason to choose EBS.
      Encryption is a security consideration that can be applied to various storage services.
    - **needs to be stored in a different Availability Zone than the one the EC2 instance is in:** EBS volumes are
      typically attached to EC2 instances within the same Availability Zone.

7. **Question Title:** True or False? By default, all data stored in Amazon S3 is viewable by the public.

   **Correct Answer:** False

   **Explanation:** This statement is false. By default, objects stored in Amazon S3 are **not** publicly viewable. They
   are private by default. To make objects publicly accessible, you must explicitly grant permissions for public access
   using S3 bucket policies or access control lists (ACLs).

    - It's important to be mindful of security when storing data in S3. Always use appropriate permissions and security
      measures to protect your data from unauthorized access.
8. **Question Title:** Regarding Amazon S3 Glacier, what is a Vault? (Select the best answer)

   **Correct Answer:** A container for storing archives

   **Explanation:**

    - In Amazon S3 Glacier, a **Vault** is a logical container where you store archives (data that is accessed
      infrequently). Think of it like a folder or a storage bin for your cold data.

   The other options are incorrect:

    - **The rules that determine who may (or may not) access archives:** This is referred to as an access policy in
      Glacier, not a Vault.
    - **An object (photos, videos, files, or documents):**  These are the actual data items that are stored as archives
      within a Vault.
    - **A policy that identifies who can access content stored in Glacier:** This is an access policy, which controls
      access to the data in a Vault.
9. **Question Title:** True or False? When you create a bucket in Amazon S3, it is associated with a specific AWS
   Region.

   **Correct Answer:** True

   **Explanation:** This statement is true. When you create an S3 bucket, you must choose a specific AWS Region where
   the bucket will be located. This means:

    - The bucket's data will be stored in the data centers within that Region.
    - Data access and transfer will primarily occur within that Region.
    - Region selection influences factors like data latency and availability.

   It's important to choose the Region that's most appropriate for your needs, considering factors like user proximity,
   data sovereignty, and latency requirements.

10. **Question Title:** Which of the following are features of Amazon Elastic Block Store (Amazon EBS)? (Choose two)

    **Correct Answer:** Amazon EBS volumes can be encrypted transparently to workloads on the attached instance.
    Data stored on Amazon EBS is automatically replicated within an Availability Zone.

    **Explanation:**
      
    - **Amazon EBS volumes can be encrypted transparently to workloads on the attached instance.**  EBS supports volume
      encryption using AWS KMS. This encryption is transparent to the EC2 instance, meaning the application running on
      the instance doesn't need to handle encryption/decryption.
    - **Data stored on Amazon EBS is automatically replicated within an Availability Zone.** EBS volumes are
      automatically replicated within an Availability Zone to provide fault tolerance. If one instance fails, another
      instance can take over the volume.

    The other options are incorrect:

    - **Data on an Amazon EBS volume is lost when the attached instance is stopped.** This is not true. EBS volumes are
      persistent storage, meaning the data remains even if the instance is stopped or terminated.
    - **Amazon EBS data is automatically backed up to tape:** EBS doesn't automatically back up data to tape. You would
      need to configure additional services like AWS Backup for backups. 











