# Online Appointment Booking System – "Zdrowy Ząbek" Clinic
This project presents a complete Object-Oriented Analysis and Design (OOAD) for a private dental clinic in Gdańsk. The system aims to automate the booking process, currently handled manually via paper calendars or simple spreadsheets.

Stage 1: Requirements Engineering & Use Case Modeling
This phase focused on defining what the system must do and identifying its primary users.
Problem Analysis: Conducted a study of the "Zdrowy Ząbek" dental clinic in Gdańsk to address high administrative costs (~90,000 PLN/year per receptionist) and manual scheduling inefficiencies.
Stakeholder Identification: Defined key actors, including the Patient, Receptionist, Dentist, Assistant, and Administrator, as well as external systems like Email/SMS.
Use Case Diagram (UCD):
Designed core system services such as registration, online booking, appointment cancellation, and schedule management.
Applied include and extend relationships to structure complex logic and avoid redundancy.
[Download Vision Document (PDF)](./stage1/WizjaSystemu.pdf)

Stage 2: Static Modeling (Class Architecture)
This stage involved designing the system's "skeleton"—its structure and data relationships.
Class Identification: Identified domain entities such as Patient, Doctor, Visit, and Service. The model focuses exclusively on business logic rather than technical implementation details like databases or UI screens.
Attributes & Operations:
Defined specific attributes for each class (e.g., PESEL, contactDetails, VisitStatus).
Assigned operations to the classes they logically belong to (e.g., assignDoctor() within the Visit class).
Relationship Mapping:
Associations: Defined with explicit multiplicities and role names to ensure data integrity.
![Class Diagram](./stage2/Class Model.png)

Stage 3: Dynamic Modeling (Behavioral Design)
The final phase modeled how objects interact over time and how they change states during system execution. A total of 6 diagrams were developed:
Sequence Diagrams (3):
Illustrated the chronological exchange of messages between actors, UI objects, and system lifelines.
Utilized Fragments (Alt, Opt, Loop) to model conditional logic and iterative processes.
Ensured deep-system interactions relied on synchronous message calls corresponding to the operations defined in the Class Diagram .
Communication Diagram (1):
Focused on the structural relationships and links between objects participating in a specific Use Case interaction .
Activity Diagram (1):
Modeled the high-level business process (e.g., the workflow from a patient's initial inquiry to the final payment) .
State Machine Diagram (1):
Defined the lifecycle of a complex object, such as a Visit.
Specified states (e.g., New, Confirmed, Cancelled, Completed) and transitions triggered by specific events, guarded by conditions, and resulting in defined effects .
