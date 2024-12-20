# Healthcare_System
## This project was part of my two final class projects for at srbiau:Database And Principles of Sofware Design,
### first for the Database,I decided to deploy the ER diagram of the following paper to sql code.

<a href="https://www.researchgate.net/publication/324182359_Article_ID_IJCIET_09_01_090_Cite_this_Article_Ahmad_Muhsin_Djawoto_Priyo_Susilo_and_Muafi_Hospital_Performance_Improvement_Through_The_Hospital_Information_System_Design" target="_blank">Article ID: IJCIET_09_01_090 Cite this Article: Ahmad Muhsin, Djawoto, Priyo Susilo and Muafi, Hospital Performance Improvement Through The Hospital Information System Design</a>
![image](https://github.com/srssina/Healthcare_Database_system/assets/95973648/11a78666-9b73-49c4-b6c5-96ce887c12b3)


# Link to SQL Code
You can view the full SQL code [here]((HCDB.sql)).

```sql
-- Sample SQL code shown below
-- patient table
Create table patient(
  PatientId int is Not null,
  Name varchar(128),
  Gender varchar(16),
  Age smallint,
  MRID int,
  primary key (patientID)
  foreign key (MRID) REFERENCES medicalrecord(MRID)
);

```
<h2>Also i decided to use this project as part as my <u>principles of sowftware design</u> course at srbiau;</h2>

### first we start our project as designing our needs and requiremets:

### 1. User Roles and Permissions
* Admin: Manages all users, assigns roles, handles system settings.
* Doctor: Accesses patient records, updates treatment plans, schedules appointments.
* Nurse: Views patient records, updates vitals, assists in treatment.
* Receptionist: Manages patient appointments, updates contact information.
* Patient: Views personal health records, schedules appointments.

### 2. Functional Requirements
* Patient Registration: New patients can register and existing patients can update their information.
* Appointment Scheduling: Doctors and patients can schedule, update, and cancel appointments.
* Electronic Health Records (EHR): Secure storage and retrieval of patient health data.
* Billing and Payments: Generates bills for services and processes payments.
* Pharmacy Management: Tracks inventory and manages medication dispensing.

### 3. Non-Functional Requirements
* Security: Ensure patient data is encrypted and access is role-based.
* Scalability: The system should handle a growing number of users and data.
* Usability: The interface should be intuitive for all user roles.
* Reliability: System uptime should be above 99.9%.

### as it follows, how can we introduce Ai handeling registeration of healthcare system,this a imaginary system totally based on ai,and totally depended on a patient's data,you can [access my article on medium](https://medium.com/@SinaRahimian/healthcare-registration-in-the-age-of-ai-a-data-flow-overview-938eaa0a134e) for full Description on How Ai can make a change in registeration system. 

### level zero DFD
![image](levelzeroDFD.png)

### level one DFD
![image](leveloneDFD.png)

### level two DFD
![image](leveltwoDFD.png)

### minimal new ER

![image](minimalnewER.png)

### event moduling

![image](SD.png)

### for the better understanding of each process in the Diagram there is a [data dictionary](Datadictionary.md),in which process broke down into combination of data.



