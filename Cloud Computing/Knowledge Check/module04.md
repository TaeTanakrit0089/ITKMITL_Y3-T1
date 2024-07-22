## Module 04 Knowledge Check

Here are the answers and explanations to the AWS S3 questions:

**1. Amazon S3**

* **Explanation:** Amazon S3 is a highly scalable object storage service perfect for storing large amounts of
  unstructured, semi-structured, and structured data. It's also very cost-effective, especially for data that isn't
  accessed frequently.

* **Why other options are incorrect:**
    * **AWS Storage Gateway** is used to connect on-premises data to the cloud, not as primary storage.
    * **Amazon RDS** is a managed relational database service, not suitable for storing unstructured data.
    * **Amazon EBS** is block storage used with EC2 instances, ideal for frequently accessed data.

**2. An internet-accessible storage location for video files that an external website can access**

* **Explanation:** Amazon S3 is widely used for hosting static website content, including videos, due to its
  scalability, durability, and cost-effectiveness.

* **Why other options are incorrect:**
    * **Ledger data... frequently:** Requires a database solution with transactional capabilities for frequent updates
      and access.
    * **Hourly storage...temporary files:**  Better handled by ephemeral storage or services like Amazon EFS.
    * **Data warehouse for business intelligence:** Usually requires data warehousing services like Amazon Redshift.

**3. HTML files and image files, Video and sound files, Client-side scripts**

* **Explanation:** Amazon S3 is perfect for hosting these static website components:
    * **HTML files and image files:** The foundation of any website.
    * **Video and sound files:** Large media files easily served by S3.
    * **Client-side scripts:** JavaScript files that run in the user's browser.

* **Why other options are incorrect:**
    * **Server-side scripts:** S3 doesn't execute server-side code (like PHP, Python, etc.). You'd need a service like
      AWS Lambda or EC2 for that.
    * **Database engine:** S3 is not a database; use services like RDS or DynamoDB.
    * **Dynamic HTML files:** S3 serves static content; dynamic content requires server-side processing.

**4. Enabling server-side encryption on the S3 bucket before uploading sensitive data, Using client-side encryption to
protect data in transit before it is sent to Amazon S3**

* **Explanation:** These are essential security practices:
    * **Server-side encryption:** Encrypts data at rest within S3.
    * **Client-side encryption:**  Adds an extra layer by encrypting data before it even reaches AWS.

* **Why other options are incorrect:**
    * **Enabling server-side encryption...after uploading...** Data is vulnerable until encryption is enabled.
    * **Uploading unencrypted files...encrypts the files by default**  While S3 offers default encryption, it's best
      practice to explicitly manage it for sensitive data.
    * **Using SFTP...** While more secure than FTP, it's better to use HTTPS or AWS CLI with appropriate security
      configurations.

**5. Recover deleted files, Maintain different versions of files**

* **Explanation:** S3 provides data protection features:
    * **Recover deleted files:**  Versioning allows restoring previous file versions, acting as a safety net against
      accidental deletions.
    * **Maintain different versions of files:**  Versioning keeps a history of changes, useful for tracking revisions or
      reverting to previous states.

* **Why other options are incorrect:**
    * **Compare file contents between files:**  Not a built-in S3 feature; requires external tools or scripts.
    * **Lock a file...one person...edit it:** Not supported by S3; you'd need to implement a separate locking mechanism.
    * **Attach comments to files:**  Not a built-in S3 feature; consider using metadata or an external document
      management system.

**7. Which option takes advantage of edge locations in Amazon CloudFront to transfer files over long distances to an S3
bucket?**

* **Correct Answer: Amazon S3 Transfer Acceleration**

* **Explanation:**  Amazon S3 Transfer Acceleration leverages CloudFront's global edge network. When you use it, uploads
  are routed to a nearby edge location and then transferred over Amazon's optimized network to the S3 bucket,
  significantly speeding up the process, especially over long distances.

8. **Amazon S3 Transfer Acceleration** - While multipart uploads can improve speed and reliability, **S3 Transfer
   Acceleration** is designed precisely for scenarios with unreliable internet connections by routing traffic through
   edge locations. This combination makes it the most cost-effective for the video producer's situation.

9. **S3 Standard-Infrequent Access (S3 Standard-IA)** - S3 Standard-IA is the ideal choice for backup and easily
   recreatable data because it offers low cost, high durability, and low latency retrieval.

10. **S3 Glacier Deep Archive** - For data that needs to be retained for long periods with minimal access, S3 Glacier
    Deep Archive offers the lowest cost storage on AWS. 
