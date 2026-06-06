# UML Documentation

## Unified Modeling Language (UML)

Unified Modeling Language (UML) is a standardized visual modeling language used to analyze, design, and document software systems. UML helps developers, designers, and stakeholders understand the structure and behavior of a system through graphical representations.

### Purpose of UML in Event Registration Portal

The UML diagrams for the Event Registration Portal provide a visual representation of system functionalities, user interactions, workflow processes, and system architecture. These diagrams assist in requirement analysis, system design, development, testing, and maintenance.

---

## 1. Use Case Diagram

### Description

The Use Case Diagram illustrates the interaction between users and the Event Registration Portal system.

### Actors

#### User

* Register Account
* Login
* View Events
* Search Events
* Register for Event
* View Registered Events
* Manage Profile
* Logout

Admin

* Login
* Create Event
* Update Event
* Delete Event
* Manage Participants
* Track Registrations
* Generate Reports
* Monitor Event Capacity
* Logout

### Purpose

* Identifies system functionalities.
* Shows interaction between users and the system.
* Helps gather functional requirements.

---

 2. Class Diagram

 Description

The Class Diagram represents the static structure of the Event Registration Portal.

 Classes

User

Attributes:

* userID
* name
* email
* password

Methods:

* register()
* login()
* searchEvents()
* registerEvent()

 Admin

Attributes:

* adminID
* username
* password

Methods:

* createEvent()
* updateEvent()
* deleteEvent()
* manageParticipants()

 Event

Attributes:

* eventID
* eventName
* description
* venue
* eventDate
* capacity

Methods:

* createEvent()
* updateEvent()
* deleteEvent()

 Registration

Attributes:

* registrationID
* registrationDate
* status

Methods:

* confirmRegistration()
* cancelRegistration()

 Relationships

* User registers for Event.
* Registration links User and Event.
* Admin manages Event.
* Admin monitors Registrations.

 Purpose

* Defines system entities and their relationships.
* Serves as the blueprint for database and software design.


3. Sequence Diagram

### Description

The Sequence Diagram illustrates the chronological interaction between system components during event registration.

Workflow

1. User logs into the portal.
2. System validates credentials.
3. User views available events.
4. System retrieves event information from the database.
5. User selects an event.
6. Registration request is submitted.
7. Registration details are stored in the database.
8. Confirmation is generated.
9. User receives registration confirmation.
10. Admin monitors registration information.

Purpose

* Visualizes message flow between system components.
* Helps understand process execution order.


## 4. Activity Diagram

 Description

The Activity Diagram represents the workflow involved in event registration.

### Process Flow

Start

→ User Registration/Login

→ Browse Events

→ Search and Filter Events

→ Select Event

→ Fill Registration Form

→ Submit Registration

→ Validate Information

Decision:

* If Valid → Store Registration → Send Confirmation → End
* If Invalid → Display Error Message → Return to Registration Form

Purpose

* Represents business process flow.
* Helps identify decision points and process logic.

 Benefits of UML Documentation

* Improves system understanding.
* Simplifies communication among team members.
* Assists in system design and implementation.
* Reduces development errors.
* Supports maintenance and future enhancements.
* Provides professional project documentation.

The UML diagrams used in this project follow standards established by the Object Management Group (OMG) and recognized by the International Organization for Standardization (ISO). Standard UML notation ensures consistency, clarity, and maintainability throughout the software development lifecycle.

