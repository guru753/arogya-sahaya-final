Problem Statement

In many rural areas, elderly patients often miss healthcare follow-ups because managing multiple medications and remembering health camp dates can be difficult. This leads to poor medication adherence, preventable complications, and emergency hospital visits.

Arogya-Sahaya Local addresses this challenge by providing a simple, accessible, and elderly-friendly healthcare companion application designed for users who may not be tech-savvy.

🎯 Vision

Arogya-Sahaya Local aims to become a reliable localized healthcare assistant with the following goals:

✅ Ensure zero-error medicine schedules
✅ Convert complex prescriptions into simple reminder-based routines
✅ Track health vitals such as:
Blood Pressure
Heart Rate
Glucose Levels
✅ Generate organized health logs for ASHA workers
✅ Improve medication adherence among rural elderly patients

📱 Features

Feature	Description
👤 Medical Profile	Store patient age, chronic conditions, allergies, and emergency details

💊 Pill Reminder	Schedule medicines for Morning / Afternoon / Night

⏰ Smart Notifications	Timely reminders using WorkManager / AlarmManager

📅 ASHA Connect	View upcoming local health camp dates (simulated)

📊 Vital Log	Enter daily BP, Sugar, and Heart Rate readings

📈 7-Day Health Trends	Visual charts using MPAndroidChart

🆘 Emergency SOS	Large emergency button for quick help simulation

🌙 Elderly-Friendly UI	High contrast colors and large readable fonts

💻 Tech Stack

Language: Kotlin

Architecture: MVVM + Repository Pattern

Database: Room Database

Background Tasks: WorkManager / AlarmManager

Charts: MPAndroidChart

UI Design: Material Design Components

Minimum SDK: Android 8.0 (API 26)

🛠️ Technical Architecture

📂 Project Structure
app/
├── data/
│   ├── local/          # Room DB — Entities, DAO, Database

│   ├── repository/     # Repository implementations

│   └── model/          # Data models
│
├── ui/
│   ├── profile/        # Medical Profile Screen

│   ├── reminder/       # Medicine Reminder Screen

│   ├── asha/           # ASHA Connect Calendar

│   ├── vitals/         # Vital Logs + Charts

│   └── emergency/      # SOS Emergency Screen
│
├── worker/             # WorkManager jobs
│
└── utils/              # Helper classes and constants

⚙️ Libraries & Tools Used
Purpose	Library / Tool

Local Storage	Room Database

Background Scheduling	WorkManager

Alarm Handling	AlarmManager

Charts & Graphs	MPAndroidChart

UI Components	Material Design

Architecture	MVVM + Repository Pattern

🔄 User Flow

User creates a medical profile

Medicines are added with dosage timings

App schedules reminder notifications

User logs daily health vitals

Vital trends are displayed in chart format

Health data can be shown to ASHA workers

Emergency SOS can be triggered if needed

✅ Success Criteria

 Reminder notifications work in Doze Mode
 
 7-day vital chart implemented
 
 Elderly-friendly accessible UI
 
 Repository Pattern implemented
 
 Local Room DB storage integrated
 
🌍 Impact Goals

Goal	Description
🏘️ Health Inclusion	Improving healthcare accessibility in rural regions

📂 Organized Records	Helping ASHA workers monitor patient history

🛡️ Preventative Care	Encouraging consistent medicine intake and monitoring

❤️ Elderly Support	Making healthcare easier for non-tech-savvy users
