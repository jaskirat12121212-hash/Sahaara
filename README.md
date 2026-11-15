🌿 SAHAARA 360

AI-Powered Elderly Care & Family Coordination Ecosystem

Care that connects. Intelligence that protects. Independence that matters.

SAHAARA 360 is an AI-powered elderly care platform designed to simplify healthcare management for elderly individuals while connecting family members and caregivers through a shared, accessible and intelligent system.

It goes beyond basic medication reminders by combining smart medication management, AI-assisted care monitoring, family coordination, voice assistance and emergency alerts in one platform.

---

📌 Problem Statement

Elderly individuals often face difficulties managing:

- Multiple medications and dosage schedules.
- Doctor appointments and health records.
- Daily healthcare routines.
- Communication with family members and caregivers.
- Emergency situations and timely assistance.

When family members live separately or caregivers change shifts, healthcare information can become fragmented.

SAHAARA 360 aims to solve this problem through a centralized, intelligent and accessible elderly care ecosystem.

💡 Our Solution

SAHAARA 360 provides a shared healthcare platform where elderly individuals can manage their daily routines while authorized family members and caregivers can monitor activities, coordinate tasks and receive important updates.

The platform focuses on three main user roles:

- 👴 Elderly Person: Simple dashboard, medication schedules, appointments and voice assistance.
- 👨‍👩‍👧 Family Member: Monitor care activities, manage permitted information and receive alerts.
- 🧑‍⚕️ Caregiver: Manage daily tasks, record medication updates and coordinate follow-ups.

---

✨ Key Features

1. 💊 Smart Medication Management

- Add, update and delete medication details.
- Set dosage, frequency and medication schedules.
- Track taken, skipped and missed doses.
- View daily and weekly medication schedules.
- Send upcoming-dose and missed-dose reminders.
- Estimate medication refill dates based on available stock.

2. 🤖 AI Care Gap Radar

An intelligent monitoring system that identifies patterns in daily healthcare activities.

- Detect repeated missed or skipped doses.
- Identify unanswered daily check-ins.
- Generate care-priority alerts.
- Provide understandable summaries for caregivers.
- Suggest follow-up actions.

Innovation: Instead of treating every reminder separately, the system identifies repeated patterns that may require human attention.

3. 📷 AI Prescription Scanner

- Upload prescription images.
- Extract medicine names and schedule details using OCR and AI.
- Generate a draft medication schedule.
- Allow authorized users to verify extracted information before saving.

4. 🎙️ Voice-First Health Companion

A voice-based interface designed to make the platform easier for elderly users.

Example commands:

- "Meri agli medicine kab hai?"
- "Aaj ki medicines complete ho gayi?"
- "Doctor appointment kab hai?"
- "Caregiver ko update bhejo."

Supports planned Hindi and English voice interactions.

5. 👨‍👩‍👧 Family Connect

- Shared elderly health profiles.
- Role-based permissions.
- Caregiver task assignment.
- Family activity feed.
- Medication and appointment updates.
- Audit history of important changes.

6. 🚨 Safety & Emergency Escalation

- Daily check-in reminders.
- Follow-up notifications when check-ins remain unanswered.
- Primary caregiver notifications.
- Secondary contact escalation.
- Emergency SOS notification to configured contacts.

7. 🏥 Health Companion

- Appointment management.
- Health timeline.
- Health Passport PDF generation.
- Appointment preparation summaries.
- Medication and care history.

---

🚀 Additional Innovations

Innovation| Purpose
AI Care Gap Radar| Identifies repeated care gaps
Prescription Scanner| Extracts medicine information from prescriptions
Refill Estimator| Estimates when medication stock may run low
Voice Assistant| Enables voice-based interaction
Health Passport| Generates shareable health summaries
Appointment Preparation AI| Helps prepare questions for doctor visits
Safety Escalation| Notifies designated contacts when follow-ups are needed

---

🛠️ Technology Stack

Component| Technology
Frontend| React.js, Tailwind CSS
Backend| Python, FastAPI
Database| Supabase PostgreSQL
AI Integration| Gemini API
OCR| OCR service
Authentication| Role-based authentication
Notifications| SMTP / Email Provider
Background Tasks| APScheduler
Frontend Hosting| Vercel
Backend Hosting| Render

Technology choices may be adjusted during implementation.

---

🏗️ System Architecture

              USERS
                 |
        React Frontend
                 |
          FastAPI Backend
                 |
       ---------------------
       |         |         |
   Medication  AI/OCR   Authentication
   Management  Services  & Permissions
       |         |         |
       ---------------------
                 |
          PostgreSQL
                 |
       ---------------------
       |         |         |
    Email     Care Gap   Family &
 Notifications Radar    Caregiver
                         Updates

---

🗄️ Database Design

The proposed database contains the following major entities:

Entity| Purpose
Users| Stores user information and roles
Elderly Profiles| Stores elderly user profiles
Care Access| Manages permissions
Medicines| Stores medication details
Dose Logs| Records medication activity
Appointments| Stores doctor appointments
Check-ins| Tracks daily check-ins
Alerts| Stores notification information
Audit Logs| Records important changes

---

🔐 Privacy & Responsible AI

SAHAARA 360 follows a human-centred approach to elderly healthcare.

- Role-based access control.
- Explicit caregiver invitations.
- Revocable permissions.
- Secure handling of health information.
- Human verification of AI-extracted prescriptions.
- No automatic medication changes.
- No AI-based medical diagnosis.

Important: SAHAARA 360 is intended to support healthcare coordination. It does not replace doctors, professional medical advice or emergency services.

---

📂 Project Structure

SAHAARA-360/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── assets/
│   │   └── App.jsx
│   ├── package.json
│   └── .env.example
│
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── models/
│   │   ├── services/
│   │   ├── database/
│   │   └── main.py
│   ├── requirements.txt
│   └── .env.example
│
├── database/
│   └── schema.sql
│
├── docs/
│   └── project-proposal.pdf
│
├── .gitignore
└── README.md

This is the suggested repository structure; adjust it to match the actual implemented files.

---

⚙️ Installation & Setup

1. Clone the repository

git clone YOUR_REPOSITORY_URL
cd SAHAARA-360

2. Frontend Setup

cd frontend
npm install
npm run dev

3. Backend Setup

cd backend

python -m venv venv

Activate the environment:

Windows:

venv\Scripts\activate

Linux / macOS:

source venv/bin/activate

Install dependencies:

pip install -r requirements.txt

Start the FastAPI server:

uvicorn app.main:app --reload

Backend API documentation:

http://127.0.0.1:8000/docs

4. Environment Variables

Create ".env" files using the provided ".env.example" templates.

Example:

DATABASE_URL=
GEMINI_API_KEY=
SMTP_EMAIL=
SMTP_PASSWORD=

Never commit actual API keys, passwords or database credentials to GitHub.

---

🗺️ Development Roadmap

Phase| Focus
Phase 1| Authentication, profiles and permissions
Phase 2| Medication management and appointments
Phase 3| Email notifications and caregiver alerts
Phase 4| AI prescription scanner and Care Gap Radar
Phase 5| Voice assistant, SOS and Health Passport

---

🎯 Expected Impact

For Elderly Individuals

- Easier healthcare management.
- Improved visibility of daily routines.
- Greater independence.

For Families

- Better coordination.
- Timely updates.
- Shared responsibility.

For Caregivers

- Organized care tasks.
- Medication history.
- Structured follow-ups.

---

🔮 Future Scope

- Wearable device integration.
- Fall detection integration.
- Advanced multilingual voice assistant.
- More intelligent care pattern analysis.
- Expanded health record integrations.
- Improved AI-assisted appointment preparation.

---

❤️ Our Vision

SAHAARA 360 aims to transform elderly care from disconnected reminders into a coordinated, accessible and proactive support ecosystem.

We believe technology should not replace human care. It should make caring for our loved ones easier, safer and more connected.

SAHAARA 360 — Care that connects. Intelligence that protects. Independence that matters.