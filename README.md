# International Students University System

## Overview

A website that lets international (foreign) students complete their university services online, while Student Affairs staff manage student data, fees, and documents.

## System Flow

1. Students come to the faculty to register.
2. Student data is uploaded on the system (by the staff).
3. Students sign in on the system.
4. The website shows buttons for the different services the student can use.
5. Students choose the service.
6. The system shows the service.
7. The student prints the paper.
8. The student signs the papers.
9. The student uploads the signed papers (payment receipt) to the system.

## Services

1. Medical Examination
2. Enrollment Fees
3. Book Fees
4. Residency Fees
5. Additional Fees that should be paid
6. Notification for any meeting with the staff (via Email)

## Users

- Foreign Students
- Student Affairs

---

## User Stories

### Foreign Student

**User Story 1**
As a `<Student>`
I want to `<sign in on the system with my account>`
So that `<I can securely access my own services>`

**User Story 2**
As a `<Student>`
I want to `<see buttons for all the available services after signing in>`
So that `<I can easily choose the service I need>`

**User Story 3**
As a `<Student>`
I want to `<choose the Medical Examination service and view its details>`
So that `<I know what is required and can complete it>`

**User Story 4**
As a `<Student>`
I want to `<view and print the Enrollment Fees paper>`
So that `<I can pay the fees and sign the paper>`

**User Story 5**
As a `<Student>`
I want to `<view and print the Book Fees paper>`
So that `<I can pay for my books on time>`

**User Story 6**
As a `<Student>`
I want to `<view and print the Residency Fees paper>`
So that `<I can keep my residency status valid>`

**User Story 7**
As a `<Student>`
I want to `<see any additional fees that should be paid>`
So that `<I don't miss any payment>`

**User Story 8**
As a `<Student>`
I want to `<upload the signed papers (payment receipt) to the system>`
So that `<the faculty can confirm that I completed the service>`

**User Story 9**
As a `<Student>`
I want to `<receive an email notification about any meeting with the staff>`
So that `<I don't miss important appointments>`

**User Story 10**
As a `<Student>`
I want to `<see the status of each service (pending, completed, rejected)>`
So that `<I know what I still need to do>`

### Student Affairs (Staff)

**User Story 11**
As a `<Staff member>`
I want to `<upload the student's data to the system after the student registers at the faculty>`
So that `<the student can sign in and use the services>`

**User Story 12**
As a `<Staff member>`
I want to `<edit or update a student's data>`
So that `<the information stays correct>`

**User Story 13**
As a `<Staff member>`
I want to `<add additional fees to a specific student>`
So that `<the student is informed and can pay them>`

**User Story 14**
As a `<Staff member>`
I want to `<review the signed papers and receipts uploaded by students>`
So that `<I can verify and approve the payments>`

**User Story 15**
As a `<Staff member>`
I want to `<schedule a meeting and send an email notification to the student>`
So that `<the student is informed automatically>`

**User Story 16**
As a `<Staff member>`
I want to `<search for students and track the status of their services>`
So that `<I can follow up with students who haven't completed their services>`

---

## Functional Requirements

### Authentication and Account Management

- **FR1:** The system shall allow Student Affairs staff to upload and register student data.
- **FR2:** The system shall allow registered students to sign in with a username and password.
- **FR3:** The system shall allow students to reset their password.
- **FR4:** The system shall restrict each user to the features of their role (Student or Student Affairs).

### Services

- **FR5:** The system shall display a button for each available service after the student signs in.
- **FR6:** The system shall show the details of the selected service (Medical Examination, Enrollment Fees, Book Fees, Residency Fees, Additional Fees).
- **FR7:** The system shall generate a printable version of each service form or payment paper.
- **FR8:** The system shall allow students to upload the signed papers or payment receipt (PDF or image).
- **FR9:** The system shall track and display each service's status (Not started, Pending review, Completed, Rejected).

### Staff Functions

- **FR10:** The system shall allow staff to add, edit, and search student records.
- **FR11:** The system shall allow staff to add additional fees to a student's account.
- **FR12:** The system shall allow staff to view, approve, or reject uploaded documents and receipts.
- **FR13:** The system shall allow staff to schedule meetings with students.

### Notifications

- **FR14:** The system shall send an email notification to the student for any meeting with the staff.
- **FR15:** The system shall notify the student when new additional fees are added or when an uploaded document is approved or rejected.

### Language and Reporting

- **FR16:** The system shall support English (and optionally Arabic) for the interface.
- **FR17:** The system shall allow staff to generate reports of paid and unpaid fees per student.

---

## Non-Functional Requirements

| Category | Requirement |
|----------|-------------|
| **Security** | Passwords must be stored encrypted (hashed). All data is transferred over HTTPS. Role-based access control must be enforced. Sessions expire after inactivity. |
| **Privacy** | Students' personal data (passport, medical, payment) must be accessible only to the student and authorized staff. |
| **Availability** | The system should be available 99% of the time, especially during registration periods. |
| **Usability** | The interface must be simple and clear for non-native speakers, with large service buttons and minimal steps. |
| **Maintainability** | The code should be modular so that new services can be added without changing the whole system. |
| **Email Delivery** | Email notifications should be sent within 1 minute of the triggering event. |
