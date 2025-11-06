# IDAI101-1000409-mohammed-saif
AI powered campus guide.Build using Dialogflow
Name:Mohammed Saif
Registration:100409
CRS name:Artificial Intelligence
Course name : Artificial Intelligence: Real-World Applications and implications
School name:Jain vidyalaya IB World School

CAMPUS NAVIGATION CHATBOT – PROJECT DOCUMENTATION
1. Project Overview

Project Title: Campus Navigation Chatbot
Platform: Google Dialogflow

Objective:
To design and implement a friendly and interactive chatbot that helps students, faculty, parents, and visitors navigate the campus easily. The chatbot will answer queries about campus buildings, departments, events, and facilities through text or voice conversation.

2. Problem Understanding and User Research

Problem Statement:
Many people find it difficult to locate buildings, offices, or events within a large campus. The goal of this chatbot is to act as a virtual campus guide that simplifies navigation and provides instant information.

Primary Users:

New students exploring the campus

Parents and guests visiting the campus

Faculty and staff searching for specific areas or events

User Pain Points:

Difficulty locating offices, classrooms, and departments

Lack of quick access to event details or schedules

Unawareness of campus rules and timings

Need for easy guidance without human assistance

Chatbot Goals:

Provide accurate directions to any building or department

Share event information, schedules, and venues

Display campus maps and facility details

Maintain a polite and helpful tone for all users

3. Chatbot Design and Development

Platform Used: Google Dialogflow ES

Development Approach:

Designed conversation flows using intents and entities.

Trained the Dialogflow agent with example phrases and slot-filling.

Tested the chatbot with real-world queries to ensure accuracy.

4. Entities (11 Total)

building_name – Science Block, Library, Admin Office

department_name – Computer Science, Physics, English

event_name – Orientation, Tech Fest, Cultural Night

location_area – North Campus, Main Block, East Wing

person_type – student, staff, visitor, parent

facility_name – cafeteria, parking, ATM, auditorium

day_name – Monday, Saturday, Sunday

time_slot – morning, afternoon, evening

transport_mode – bus, car, cycle, walk

event_date – today, tomorrow, 10th November

rules_type – dress code, ID rules, mobile use

Each entity helps the chatbot understand specific details from the user query, improving response accuracy.

5. Intents (16 Total)

Welcome_Intent – Greets users when they start a conversation.
Example: “Hi”, “Hello”
Response: “Hello! I’m your Campus Guide. How can I help you today?”

Find_Building_Intent – Helps users locate buildings.
Example: “Where is the Admin Office?”
Response: “The Admin Office is located in the Main Block near the entrance.”

Find_Department_Intent – Provides department locations.
Example: “Where is the Computer Science department?”
Response: “The Computer Science Department is on the second floor of the Academic Block.”

Find_Event_Location_Intent – Gives event locations.
Example: “Where is the Tech Fest happening?”
Response: “Tech Fest is being held at the Auditorium in the South Campus.”

Campus_Timings_Intent – Tells campus or facility timings.
Example: “What are the library hours?”
Response: “The Library is open from 8:00 AM to 6:00 PM on weekdays.”

Facilities_Location_Intent – Locates campus facilities.
Example: “Where is the cafeteria?”
Response: “The Cafeteria is located behind the Science Block.”

Department_Info_Intent – Provides department information.
Example: “Tell me about the Physics Department.”
Response: “The Physics Department offers B.Sc and M.Sc programs and is located in the East Wing.”

Event_Schedule_Intent – Gives event date and time.
Example: “When is the Cultural Night?”
Response: “Cultural Night is scheduled on 12th November at 6 PM in the Auditorium.”

Rules_Intent – Shares campus rules.
Example: “Are mobiles allowed in class?”
Response: “Mobile use during class hours is not permitted.”

Transport_Info_Intent – Provides transport or route info.
Example: “How can I reach the campus by bus?”
Response: “Take Bus No. 21 from the city center, it stops at the Main Gate.”

Parking_Info_Intent – Tells about parking locations.
Example: “Where can I park my car?”
Response: “Visitors can park behind the Admin Block in Parking Zone A.”

Lost_and_Found_Intent – Handles lost item queries.
Example: “I lost my ID card.”
Response: “Please visit the Security Office near the Main Entrance to report lost items.”

Emergency_Contact_Intent – Gives emergency contact details.
Example: “Who to contact in emergency?”
Response: “In case of emergency, contact Campus Security at 1800-222-HELP.”

Farewell_Intent – Ends the conversation politely.
Example: “Thanks”, “Bye”
Response: “You’re welcome! Have a great day on campus.”

Map_Request_Intent – Shows campus map.
Example: “Show me the campus map.”
Response: “Here’s the campus map [image link].”

Feedback_Intent – Collects user feedback.
Example: “This chatbot is great!”
Response: “Thank you! Your feedback helps us improve.”

6. Features Implemented

Slot Filling: The bot asks for missing details automatically, such as asking “Which department?” if the user says “Where is the department?”.

Context Handling: Maintains short-term conversation flow for follow-up questions.

Suggestion Chips: Provides quick buttons like “Departments”, “Events”, “Timings”, and “Map”.

Media Responses: Displays images or maps of the campus.

Fallback Handling: Responds politely to unknown inputs.

Personalized Responses: Adjusts replies based on user type (student, visitor, etc.).

Follow-up Intents: Keeps conversations natural and continuous.

7. Testing and Optimization

Testing Approach:

Simulated multiple user queries in the Dialogflow console.

Verified that intents and entities are correctly recognized.

Tested context switching and follow-up interactions.

Ensured polite tone and clear answers.

Sample Test Queries and Results:

“Where is the Admin Office?” → Correctly responded with location.

“When is the Tech Fest?” → Provided accurate date and time.

“Where is parking?” → Directed to correct parking zone.

“What are library timings?” → Displayed correct hours.

Optimization Suggestions:

Add multilingual support for international students.

Integrate Google Maps API for real-time directions.

Add voice assistant capability through Google Assistant.

Connect with event calendar for live schedule updates.

8. Evaluation Metrics

Intent Recognition Accuracy – How accurately user intents are identified.

Entity Extraction Rate – How well the chatbot extracts keywords like building names or events.

Response Time – The speed of the chatbot’s replies.

User Satisfaction – Measured through feedback and ratings.

Error Recovery Rate – Ability to handle unclear or wrong inputs gracefully.

9. System Architecture

Components:

User Interface: Dialogflow web chat or Google Assistant.

Dialogflow Agent: Contains all intents, entities, and contexts.

Fulfillment (optional): Connects chatbot to external databases.

Database: Stores department and event data if needed.

Media Files: Maps and banners for responses.

Workflow:

User sends a message to the chatbot.

Dialogflow detects the intent and extracts entities.

The chatbot forms a response using detected information.

The reply may include text, images, or suggestion buttons.

Context is maintained for follow-up questions.

10. Sample Conversation

User: Hi
Bot: Hello! I’m your Campus Guide. How can I help you today?

User: Where is the Computer Science department?
Bot: The Computer Science Department is on the 2nd floor of the Academic Block. Would you like to see the map?

User: Yes
Bot: Here’s the campus map [image link].

User: What are the library timings?
Bot: The Library is open from 8:00 AM to 6:00 PM on weekdays.

User: Thanks
Bot: You’re welcome! Have a great day on campus!

11. Conclusion

The Campus Navigation Chatbot successfully provides instant, accurate, and helpful information for anyone navigating the campus. It enhances user experience by giving directions, timings, and event details in an easy conversational format.

The chatbot demonstrates the practical use of AI in education and can be further improved by integrating real-time data, GPS, and multilingual voice responses.

12. Summary

Total Intents: 16
Total Entities: 11
Platform: Google Dialogflow
Main Users: Students, Staff, Visitors, Parents
Main Functions: Campus navigation, event details, department info, rules, timings, feedback
Features: Suggestion chips, context handling, slot filling, and media responses
