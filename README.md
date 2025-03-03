Meeting Room Booking System
📌 Overview
The Meeting Room Booking System is a Python-based web application that helps organizations efficiently manage their meeting rooms. It eliminates conflicts, prevents double bookings, and allows users to plan meetings hassle-free. The app is built using Streamlit for an intuitive and interactive UI.

🚀 Features
✅ Book a Meeting Room – Select a date, time slot, and available room
✅ Real-Time Availability – Check available rooms dynamically
✅ Automatic Time Validation – Ensures start time is after the current time
✅ Confirmation Email – Sends a confirmation email upon successful booking
✅ Easy-to-Use Interface – Built with Streamlit for a smooth user experience

🛠️ Tech Stack
Python (Core logic)
Streamlit (Frontend UI)
CSV Storage (For managing booking data)
SMTP (Email Service) (For sending confirmation emails)
📥 Installation & Setup
Clone the Repository

sh
Copy
Edit
git clone https://github.com/Bhanukaushik/meeting_room.git
cd meeting-room-booking
Install Dependencies

sh
Copy
Edit
pip install -r requirements.txt
Set Up Streamlit Secrets (for Emailing)

Open Streamlit Cloud → Manage App → Secrets
Add the following details:
toml
Copy
Edit
sender_email = "your-email@example.com"
email_password = "your-app-password"
Run the Application

sh
Copy
Edit
streamlit run meeting_room.py
📧 Email Setup (SMTP)
The app sends confirmation emails using an SMTP service.
For Gmail users:

Enable 2-Step Verification in your Google account.
Generate an App Password (Google App Passwords).
Use this password in st.secrets["email_password"].
For Outlook users, follow Microsoft’s app password setup.

🎯 How It Works
Select a Date & Time – Users choose the meeting date and time slot.
Check Available Rooms – The system dynamically lists available rooms.
Enter Booking Details – Users provide name, email, and meeting title.
Confirm Booking – The system registers the booking and sends a confirmation email.
📷 Screenshots
(Add screenshots of the UI here if available.)

📌 Future Enhancements
🚀 Database Integration – Move from CSV to PostgreSQL/MySQL for better scalability
🚀 Admin Dashboard – View and manage bookings in an admin panel
🚀 Cancel/Reschedule Meetings – Allow users to modify bookings
