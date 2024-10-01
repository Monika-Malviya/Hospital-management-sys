**Database Overview**<br>
The HMS database is designed to manage various aspects of hospital operations, including patient information, doctor details, billing, appointments, and prescriptions.

**Tables and Their Purpose**<br>

**1. Patients**<br>
**Purpose**: Stores information about patients.<br>
**Key Fields**:<br>
**patient_id**: Unique identifier for each patient.<br>
**name**: Full name of the patient.<br>
**gender**: Gender of the patient.<br>
**contact_number**: Patient’s contact number.<br>
**address**: Residential address of the patient.<br>
**email**: Email address of the patient.<br>
**doctor_id**: References the doctor assigned to the patient.<br>

**2. Doctors**<br>
**Purpose**: Stores information about doctors.<br>
**Key Fields**:<br>
**doctor_id**: Unique identifier for each doctor.<br>
**name**: Full name of the doctor.<br>
**specialty**: Medical specialty of the doctor.<br>
**contact_number**: Doctor’s contact number.<br>
**email**: Email address of the doctor.<br>
**date_hired**: Date when the doctor was hired.<br>
**appointment_id**: References appointments associated with the doctor.<br>

**3. Billing**<br>
**Purpose**: Manages billing information for appointments.<br>
**Key Fields**:<br>
**billing_id**: Unique identifier for each billing record.<br>
**appointment_id**: References the appointment related to the billing.<br>
**amount**: Total amount billed.<br>
**billing_date**: Date when the billing was done.<br>
**patient_id**: References the patient associated with the billing.<br>

**4. Appointments**<br>
**Purpose**: Manages appointment details between patients and doctors.<br>
**Key Fields**:<br>
**appointment_id**: Unique identifier for each appointment.<br>
**patient_id**: References the patient for the appointment.<br>
**doctor_id**: References the doctor for the appointment.<br>
**appointment_date**: Date of the appointment.<br>
**appointment_time**: Time of the appointment.<br>
**billing_id**: References the billing record for the appointment.<br>

**5. Prescriptions**<br>
**Purpose**: Stores prescription details issued during appointments.<br>
**Key Fields**:<br>
**prescription_id**: Unique identifier for each prescription.<br>
**appointment_id**: References the appointment during which the prescription was issued.<br>
**medicine_name**: Name of the prescribed medicine.<br>
**dosage**: Dosage instructions for the medicine.<br>
**duration**: Duration for which the medicine should be taken.<br>

