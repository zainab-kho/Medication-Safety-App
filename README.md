# Medication-Safety-App
 
 This project is a database and application design for managing patients, doctors, appointments, and insurance records.

---

## Features
- Patient, doctor, appointment, and insurance tables  
- Constraints to ensure data integrity (unique IDs, no double bookings, valid insurance, etc.)  
- Role-based views for:  
  - Patients  
  - Doctors  
  - Receptionists  
  - Insurance staff  

---

## Schema (Simplified)
- **Patient**(name, patient_id, age, birthday, phone, email)  
- **Doctor**(name, doctor_id, specialty, phone, email)  
- **Appointment**(appt_id, patient_id → Patient, doctor_id → Doctor, appt_time, appt_date)  
- **Insurance**(insurance_id, provider_name, plan)  

---

## Constraints
- All IDs must be unique  
- Appointments must be scheduled for future dates  
- Doctors cannot have overlapping appointments  
- Insurance must be valid  

---
