[![Build Status](https://github.com/amanb12/hospitalAppointmentControl/actions/workflows/master_hospital-appointment-control-system.yml/badge.svg?branch=master)](https://github.com/amanb12/hospitalAppointmentControl/actions/workflows/master_hospital-appointment-control-system.yml)
<br />
<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg?labelColor=303030" /></a>
<a><img alt="GitHub Forks" src="https://img.shields.io/github/forks/sumitkumar1503/hospitalmanagement?color=orange" /><a>
<br />

## About The Project

<div>
  <p>
    This project is further development of
    <a href="https://github.com/sumitkumar1503/hospitalmanagement">sumitkumar1503/hospitalmanagement.</a>
  </p>
</div>

This is a sample project created for the purpose of learning and demonstration of Microsoft Azure skills during the
<a href="https://futurereadytalent.in/">Future Ready Talent Program</a>.
And so, this project is not intended for commercial deployment.

This is a simple doctor appointment management system. It is a web application that allows you to manage medical appointments of a single or group of doctor by a centralized administration.
A patient can book an appointment with a doctor at their convinience and if the admins approves this, the doctor can view the list of appointments of their patient.

<br />

## Functions

### Admin

<div>
  <a href="https://raw.githubusercontent.com/amanb12/hospitalAppointmentControl/master/static/screenshots/admin_dashboard.png">
    <img align="right" width="240px"  src="https://raw.githubusercontent.com/amanb12/hospitalAppointmentControl/master/static/screenshots/admin_dashboard.png">
  </a>
</div>

- Signup their account. Then Login (No approval Required).
- Can register/view/approve/reject/delete doctor (approve those doctor who applied for job in their hospital).
- Can admit/view/approve/reject/discharge patient (discharge patient when treatment is done).
- Can Generate/Download Invoice pdf (Generate Invoice according to medicine cost, room charge, doctor charge and other charge).
- Can view/book/approve Appointment (approve those appointments which is requested by patient).

### Doctor

- Apply for job in hospital. Then Login (Approval required by hospital admin, Then only doctor can login).
- Can only view their patient details (symptoms, name, mobile ) assigned to that doctor by admin.
- Can view their discharged(by admin) patient list.
- Can view their Appointments, booked by admin.
- Can delete their Appointment, when doctor attended their appointment.

### Patient

- Create account for admit in hospital. Then Login (Approval required by hospital admin, Then only patient can login).
- Can view assigned doctor's details like ( specialization, mobile, address).
- Can view their booked appointment status (pending/confirmed by admin).
- Can book appointments.(approval required by admin)
- Can view/download Invoice pdf (Only when that patient is discharged by admin).

## Drawbacks/LoopHoles

- Any one can be Admin. There is no Approval required for admin account. So you can disable admin signup process and use any logic like creating superuser.
- There should be at least one doctor in hospital before admitting patient. So first add doctor.
- On update page of doctor/patient you must have to update password.
