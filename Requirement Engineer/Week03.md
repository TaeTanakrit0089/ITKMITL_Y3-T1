## FURPS+

**FURPS+** คือแบบจำลองสำหรับการจำแนกคุณลักษณะด้านคุณภาพซอฟต์แวร์ (หรือที่เรียกว่าข้อกำหนดที่ไม่ใช่ฟังก์ชัน) ตัวย่อมาจาก:

* **F**unctionality (ฟังก์ชันการทำงาน): คุณสมบัติ ความสามารถ ความปลอดภัย
* **U**sability (ความสามารถในการใช้งาน): ปัจจัยมนุษย์ ความสวยงาม ความสอดคล้องกัน ความช่วยเหลือ เอกสาร
* **R**eliability (ความน่าเชื่อถือ): ความถี่/ผลกระทบของความล้มเหลว ความสามารถในการกู้คืน ความสามารถในการคาดการณ์
* **P**erformance (ประสิทธิภาพ): ความเร็ว ประสิทธิภาพ การใช้ทรัพยากร ปริมาณงาน ความสามารถในการปรับขนาด
* **S**upportability (ความสามารถในการสนับสนุน): ความสามารถในการทดสอบ ความสามารถในการปรับตัว ความสามารถในการบำรุงรักษา
  ความเข้ากันได้ ความสามารถในการกำหนดค่า
* **+** ("พลัส"): คุณลักษณะอื่นๆ เช่น:
    * **Implementation** (การใช้งาน): ภาษาและเครื่องมือ การปฏิบัติตามมาตรฐาน
    * **Interface** (อินเทอร์เฟซ): ข้อจำกัดที่กำหนดโดยการเชื่อมต่อกับระบบภายนอก
    * **Operations** (การดำเนินงาน): การดูแลระบบ การจัดการ
    * **Packaging** (บรรจุภัณฑ์): ตัวอย่างเช่น สื่อบันทึกข้อมูล หากเกี่ยวข้อง
    * **Legal** (กฎหมาย): การออกใบอนุญาต การปฏิบัติตามกฎของโอเพ่นซอร์ส ฯลฯ

**ตัวอย่าง:**

| คุณลักษณะด้านคุณภาพ         | คำอธิบาย                                                     |
|-----------------------------|--------------------------------------------------------------|
| **ฟังก์ชันการทำงาน**        | แอปพลิเคชันต้องอนุญาตให้ผู้ใช้สร้างและแก้ไขเอกสารได้         |
| **ความสามารถในการใช้งาน**   | แอปพลิเคชันต้องเรียนรู้และใช้งานง่าย แม้แต่กับผู้ใช้ครั้งแรก |
| **ความน่าเชื่อถือ**         | แอปพลิเคชันต้องพร้อมใช้งาน 99.9% ของเวลา                     |
| **ประสิทธิภาพ**             | แอปพลิเคชันต้องตอบสนองต่อการกระทำของผู้ใช้ภายใน 2 วินาที     |
| **ความสามารถในการสนับสนุน** | แอปพลิเคชันต้องบำรุงรักษาและอัปเกรดง่าย                      | 

## Case Tool

CASE Tool ย่อมาจาก **Computer-Aided Software Engineering Tool** คือ เครื่องมือที่ใช้คอมพิวเตอร์ช่วยในการพัฒนาซอฟต์แวร์
โดยมีจุดประสงค์เพื่อเพิ่มประสิทธิภาพและประสิทธิผลของกระบวนการพัฒนาซอฟต์แวร์ในทุกขั้นตอน ตั้งแต่การวิเคราะห์ระบบ
การออกแบบ ไปจนถึงการทดสอบและการบำรุงรักษา

# Module 2: Introduction to RMUC (Requirement Management Use-Cases)



## Objectives:

* Define requirements management.
* Describe aspects of requirement quality.
* Identify factors that contribute to project success and project failure.
* Describe how requirements management increases the chances for project success.
* List team members (roles) in requirement management.

---

## Definitions

* **Requirement:** A condition or capability to which the system must conform.
* **Requirements management:** การจัดการความต้องการ เป็นกระบวนการที่ประกอบไปด้วย
  * Finding (ค้นหา)
  * Eliciting (ดึงออกมา)
  * Organizing (การจัดการ)
  * Documenting (การทำเอกสาร)
  * Managing Requirements ()
  * Establishing and maintaining agreement between customer/user and the project team on the changing requirements.

---

## Requirements Exist at Many Levels

```
Stakeholder Needs
                ^
                | Transformation
                v
System Requirements
```

---

## Qualities of a Software Requirement

* Verifiable (สามารถตรวจสอบได้)
* Ranked for importance and stability ()
* Modifiable
* Traceable
* Understandable
* Correct
* Complete
* Consistent
* Unambiguous

---

## Qualities of a Requirement: Verifiable

* A requirement is verifiable if there exists a finite, cost-effective process to check if the product meets the requirement.

**Examples:**

* The system supports up to 1,000 simultaneous users. **(Verifiable)**
* The system shall respond to an arbitrary query in 500 msec. **(Verifiable)**
* The color shall be a pleasing shade of green. **(Not verifiable)**
* The system shall be available 24 X 7. **(Verifiable)**
* The system shall export view data in comma-separated format. **(Verifiable)**

---

## Qualities of a Requirement: Traceable

```
Stakeholder Requests
                ^
                | Traceability
                v
Features
                ^
                | Traceability
                v
Use Cases & Supplementary Requirements 
```

---

## Qualities of a Requirement: Unambiguous

* A requirement is unambiguous if it has only one interpretation.

**Example:**

"A shall do B to C" - This requirement should have a clear and single meaning.

---

## Exploring Ambiguity: An Observation

```
                Understandability
                        ^
                        |
                        |
       Ambiguity  <-------|-------->  Clarity
                        |
                        |
                        v
                Complexity 
```
The "sweet spot" lies where the requirement is clear, understandable and avoids ambiguity.

---

## Exercise 2.1: Explore Ambiguity

* Discuss language ambiguity in a sample sentence.
* Explore dictionary definitions.
* Analyze combination of words.
* Identify ways to minimize ambiguity.

**Example sentence:** "Mary had a little lamb." (Open to multiple interpretations)

---

## What is NOT in a Requirement?

* **Design:** How to accomplish the requirements. This is covered in the design model.
* **Verification:** How you know the requirements have been met. This is specified in the test model.
* **Project Data:** When the requirements are met.  This is detailed in the software development plan.

---

## Requirements Management Is Not Easy, Because…

* Requirements:
  * Are not always obvious.
  * Can come from many sources.
  * May not always be easy to express clearly.
  * Relate to one another and to other software engineering deliverables.
  * Have unique properties and/or property values.
  * **Change.**

* A large number of requirements is unmanageable without control.

---

## Keys to Effective Requirements Management

* Maintain a clear statement of the requirements with:
  * Good quality requirements.
  * Applicable attributes for each requirement type.
  * Traceability to other requirements and project artifacts.

**Goal:** Deliver quality products on time and on budget that meet the customer’s real needs.

---

## What Is a Quality Product?

**FURPS+ Model:**

* **Functionality:**
  * Feature set
  * Capabilities
  * Generality
  * Security
* **Usability:**
  * Human factors
  * Aesthetics
  * Consistency
  * Documentation
* **Reliability:**
  * Frequency/Severity of Failure
  * Recovery
  * Predictability
  * Accuracy
  * MTBF
* **Performance:**
  * Speed
  * Efficiency
  * Resource Usage
  * Throughput
  * Response Time
* **Supportability:**
  * Testability
  * Extensibility
  * Adaptability
  * Maintainability
  * Compatibility
  * Configurability
  * Serviceability
  * Installability
  * Localizability
  * Robustness

---

## On Time and On Budget

* **Resources:** How much can we afford?
* **Time:** How much time do we have?
* **Scope:** How much work can we do?

These three factors are interconnected and must be balanced.

---

## Meet the Customer’s Real Needs

* How do we know what the needs are?
* How do we determine priority?
* What is in the baseline?

Understanding these is crucial for defining project scope and meeting customer expectations.

---

## Agreement on What the System Should Do

```
Customer/User Community <-----> Requirements Surrogate (e.g., Business Analyst)
                ^                ^
                | Communication  | Communication
                v                v
        Requirements <----------------> System To Be Built 
                ^
                | Verification
                v
                Goal
```
Effective communication and a shared understanding of requirements are essential.

---

## What Factors Contribute to Project Success?

* User Involvement
* Executive Management Support
* Clear Statement of Business Objectives

**However, Statistics Show:**

* Only 26% of projects completed on time and on budget.
* 46% of projects overran original estimates.
* 28% of projects canceled before completion.

---

## Size Is Important

**Success Rate vs. Project Size:** Larger projects tend to have lower success rates.

---

## High Cost of Requirement Errors: The 1-10-100 Rule

* The cost of fixing errors increases exponentially the later they are found in the software development lifecycle.
* Finding and fixing errors during the requirements phase is significantly cheaper than fixing them during maintenance.

---

## How Can Projects Succeed?

* **Problem analysis:** Understand and gain stakeholder agreement on the problem.
* **Requirements elicitation:** Identify actors and use cases.
* **Requirements management:**
  * Specify requirements completely.
  * Manage expectations, changes, and errors.
  * Control scope creep.
  * Involve all team members.

---

## Involve the Whole Team in Requirements

* Developers, testers, writers:
  * Help develop and monitor requirements management practices.
  * Verify elicitation processes and document requirements.
  * Participate in reviews and the Change Control Board (CCB).
  * Review traceability outcomes and verify quality, testability, and completeness.

---

## Requirements Discipline: Workflow Details

(Refer to slide 24 for visual workflow diagram)

---

## Roles and Artifacts

(Refer to slide 25 for roles and artifacts table)

---

## Review:

1. What is a requirement?
2. What are some characteristics of well-written requirements?
3. What is requirements management?
4. What factors contribute to project success?
5. What team members are involved in requirements management and how?
6. How would you explain the 1-10-100 rule? 
