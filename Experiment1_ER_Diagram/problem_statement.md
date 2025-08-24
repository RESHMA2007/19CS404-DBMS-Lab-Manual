# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:

### 🔹 Scenario 1: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).

---

### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name:RESHMA R    212224040274

## Scenario Chosen:
University / Hospital (choose one)
## SCNERIO CHOSEN : University

## ER Diagram:
![ER Diagram](er_diagram.png)
<img width="1367" height="557" alt="Screenshot 2025-08-24 095454" src="https://github.com/user-attachments/assets/2d5d5c7f-17e9-4aae-bc9a-6de3ff6290e0" />


## Entities and Attributes:
Student: Name, DOB, Register Number, Phone Number, Email ID, Subjects Enrolled
University:University Name, University ID, Students and Faculties

Department:Department Name, Department ID

Program:Program Name, Program Code, Subjects

Faculties:Name, Subject, Faculty ID

Course:Course Name, Course Code, Credits


## Relationships and Constraints:
Relationship1 – Relationship (Many-to-Many, Student–University)

Relationship2 – Is in a (Many-to-Many, Student–Department)

Relationship3 – Provides (Many-to-Many, Department–Program)

Relationship4 – Contains (Many-to-Many, Program–Course)

Relationship5 – Handles (Many-to-Many, Faculties–Course)

Relationship6 – Has (Many-to-Many, University–Faculties)


## Extension (Prerequisite / Billing):
Explain how you modeled prerequisites or billing.
First, a self-referencing M:N
relationship called "Prerequisite" would be added within the Course entity, allowing
the system to model the dependency between different courses. This ensures that
course enrollment rules based on previous completions can be enforced properly.
Second, a new entity called "Payment" would be introduced and linked to the
Student entity through a One-to-Many relationship. This addition would help track
all financial transactions, manage tuition fees, and support billing operations,
providing a complete view of the financial obligations of each student. These
enhancements would make the model more realistic and capable of supporting a
fully functional university management system.
## Design Choices:
Brief explanation of why you chose certain entities, relationships, and assumptions.

## RESULT
