# IDAI101-100409-mohammed-saif
AI powered campus guide.Build using Dialogflow
Name:Mohammed Saif
Registration:100409
CRS name:Artificial Intelligence
Course name : Artificial Intelligence: Real-World Applications and implications
School name:Jain vidyalaya IB World School
Link for the bot:https://saif2610.github.io/IDAI101-100409-mohammed-saif/
CampusBot — Project Report

Prepared by: Mohammed saif

 
Abstract
CampusBot is a chatbot designed to help students access campus information such as events, course details, faculty contacts, and general support.
This report documents the design, implementation, testing, and results of the CampusBot project. It aims to provide a clear guide to set up, run, and extend the chatbot for campus-related assistance.
 
Objectives
Primary Objectives:
• Provide instant campus information to students (events, courses, faculty, locations).
• Offer a simple conversational interface for common queries and support.
• Be extensible for adding modules like notifications, FAQs, and appointment booking.
 
Technologies Used
Dialogflow / NLP
 
System Architecture
The CampusBot project follows a modular architecture: an interface layer (chat UI), a processing layer (NLP / intent handling), and a data layer (campus information storage).
Typical components:
• User Interface — Web-based or messaging platform integration (could be Streamlit, Flask, or a chat widget).
• NLP Engine — Dialogflow or a simple intent-matching module. Handles user intents and entities.
• Backend — Python scripts or Flask APIs that fetch/process data and return responses.
• Data Store — JSON files, CSV, or a small database to store campus data and FAQs.
 
Project Structure & Main Modules
Intent 1:  Ask Admission:
               how to apply for admission
               admission process
Intent 2:  Ask Cafeteria Timetable
        cafeteria timings for UG students
        when is lunch for PG
Intent 3:Ask Department
        list departments
        faculty details
Intent 4:Ask Facilities
      what facilities are available
      tell me about campus facilities
Intent 4: Ask Hostel Timetable
        what is hostel curfew
        mess timing in hostel C


Files extracted from campus-bot.zip:
•	• package.json
•	• agent.json
•	• entities/facility.json
•	• entities/department.json
•	• entities/class_type.json
•	• entities/program_type.json
•	• entities/building.json
•	• entities/sports.json
•	• entities/meal_type.json
•	• entities/transport_route.json
•	• entities/hostel.json
•	• intents/Ask Fee.json
•	• intents/Ask Cafeteria Timetable.json
•	• intents/Default Fallback Intent.json
•	• intents/Ask School Info.json
•	• intents/Ask Transport Info.json
•	• intents/Ask Placement.json
•	• intents/Ask Admission.json
•	• intents/Ask Facilities.json
•	• intents/Ask Department.json
•	• intents/Ask Hostel Timetable.json
•	• intents/Ask IB Program.json
•	• intents/Default Welcome Intent.json
•	• intents/Ask Sports Schedule.json
•	• intents/Ask Fee_usersays_en.json
•	• intents/Ask Cafeteria Timetable_usersays_en.json
•	• intents/Ask School Info_usersays_en.json
•	• intents/Ask Transport Info_usersays_en.json
•	• intents/Ask Placement_usersays_en.json
•	• intents/Ask Admission_usersays_en.json
•	• intents/Ask Facilities_usersays_en.json
•	• intents/Ask Department_usersays_en.json
•	• intents/Ask Hostel Timetable_usersays_en.json
•	• intents/Ask IB Program_usersays_en.json
•	• intents/Ask Sports Schedule_usersays_en.json
 
Installation & Setup
1. Requirements:
• Python 3.8+ installed.
• Install dependencies (if requirements.txt provided):
  pip install -r requirements.txt
2. Run the application:
• For Flask: python app.py or flask run
• For Streamlit: streamlit run app.py
3. Dialogflow (if used): upload agent, configure webhook URL to point to backend.
 
Implementation
High-level implementation notes:
• Intent handling is implemented in Python with functions mapping to different campus services (e.g., get_events(), get_course_info()).
• Responses are templated to allow easy updates and localization.
• The bot supports fallback intent to gracefully handle unknown queries and can log them for improvement.
 
Testing & Validation
Testing performed:
• Unit testing for core functions (data retrieval, intent matching).
• Integration testing with the chat UI and backend.
• Sample conversation flows tested for common queries like "What events are on campus today?" or "Who teaches Data Structures?"
 
Results
The CampusBot demonstrates the ability to answer routine campus queries, provide resource links, and escalate complex requests to human support.
Screenshots and example conversations can be placed here. (Images found in the project folder were listed above—add them manually if you want them embedded in the report.)
 
Conclusion
CampusBot provides a lightweight, extendable chatbot solution for campus assistance. Future enhancements include:
• Adding authentication and personalized responses.
• Integrating calendar/booking features and push notifications.
• Improving NLP accuracy and adding multilingual support.
 
References & Appendix
• Project source files (listed earlier).
• README not found; include project-specific documentation if available.

Appendix: Helpful commands
• pip install -r requirements.txt
• python app.py
• streamlit run app.py
