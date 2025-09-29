# User Stories for Healthcare Appointment Booking System

This document outlines user stories for the key roles in the system: Admin, Patient, and Doctor. Stories are derived from standard healthcare management practices and focus on core functionalities like access control, appointment booking, and scheduling.<grok-card data-id="7e75b2" data-type="citation_card"></grok-card> <grok-card data-id="2a4c1b" data-type="citation_card"></grok-card> Each story follows the format: **As a [role], I want [feature] so that [benefit].** Acceptance criteria are listed below each story.

## Admin User Stories
Admins manage system access, users, and overall functionality to ensure secure and efficient operations.

### US-001: Manage User Accounts (High Priority)
**As an Admin, I want to create, edit, and delete user accounts (patients, doctors) so that I can control access to the system.**

- Acceptance Criteria:
  - Validate unique email and credentials during creation.
  - Role-based access (e.g., assign as Patient/Doctor).
  - Audit log for changes.
  - Confirmation email sent on creation.

### US-002: View System Reports (High Priority)
**As an Admin, I want to generate reports on appointments and user activity so that I can monitor system usage and performance.**

- Acceptance Criteria:
  - Filter by date range, user type, or status.
  - Export to PDF/CSV.
  - Real-time dashboard integration.

### US-003: Manage Doctor Specialties (Medium Priority)
**As an Admin, I want to add/update doctor specialties and availability rules so that patients can book accurately.**

- Acceptance Criteria:
  - Link specialties to doctors.
  - Set global availability constraints (e.g., max appointments/day).

### US-004: Handle System Emergencies (Medium Priority)
**As an Admin, I want to override appointments for emergencies so that critical cases are prioritized.**

- Acceptance Criteria:
  - Flag emergency requests and reassign slots.
  - Notify affected users via SMS/email.<grok-card data-id="926e50" data-type="citation_card"></grok-card>

## Patient User Stories
Patients book and manage appointments to access healthcare services efficiently.

### US-005: Search and Book Appointments (High Priority)
**As a Patient, I want to search for doctors by specialty, location, or symptoms and book available slots so that I can schedule care quickly without queues.**

- Acceptance Criteria:
  - Search filters with real-time availability.
  - Instant booking confirmation and calendar integration.
  - Payment gateway for fees.<grok-card data-id="51a7b4" data-type="citation_card"></grok-card> <grok-card data-id="025c4f" data-type="citation_card"></grok-card> <grok-card data-id="4aa6b6" data-type="citation_card"></grok-card>

### US-006: View and Cancel Appointments (High Priority)
**As a Patient, I want to view my upcoming appointments and cancel if needed so that I can manage my schedule flexibly.**

- Acceptance Criteria:
  - List view with details (doctor, time, notes).
  - Cancellation policy enforcement (e.g., 24-hour notice).
  - Reschedule option with available slots.

### US-007: Receive Notifications (Medium Priority)
**As a Patient, I want SMS/email reminders for appointments so that I don't miss my visits.**

- Acceptance Criteria:
  - Customizable reminder timing (e.g., 24 hours before).
  - Include directions and prep instructions.

### US-008: Update Personal Information (Medium Priority)
**As a Patient, I want to edit my profile (contact, medical history) so that my records stay accurate.**

- Acceptance Criteria:
  - Secure updates with verification.
  - Admin approval for sensitive changes.

## Doctor User Stories
Doctors manage availability and patient interactions to optimize their practice.

### US-009: Set Availability Schedule (High Priority)
**As a Doctor, I want to define my available time slots and update them so that patients can only book when I'm free.**

- Acceptance Criteria:
  - Calendar view for weekly/monthly setup.
  - Buffer time between appointments.
  - Sync with external calendars (e.g., Google).<grok-card data-id="4e7b34" data-type="citation_card"></grok-card> <grok-card data-id="38ea03" data-type="citation_card"></grok-card>

### US-010: View and Manage Appointments (High Priority)
**As a Doctor, I want to see my daily/weekly appointments and reschedule if needed so that I can prepare for patient visits.**

- Acceptance Criteria:
  - Detailed patient info on load.
  - One-click reschedule with patient notification.
  - Mark as completed/no-show.

### US-011: Access Patient History (Medium Priority)
**As a Doctor, I want to view patient medical history and prescriptions so that I can provide informed care.**

- Acceptance Criteria:
  - Pull from MongoDB/MySQL securely.
  - Consent-based access.

### US-012: Send Follow-up Instructions (Medium Priority)
**As a Doctor, I want to send post-appointment notes or prescriptions so that patients receive timely guidance.**

- Acceptance Criteria:
  - Template-based messaging.
  - Integration with e-prescription system.

## Next Steps
- Prioritize stories for sprints.
- Refine based on stakeholder feedback.
- Link to architecture: Stories map to dashboards (Admin/Doctor), booking flows (Patient), and DB models (Appointments/Patients).