Dog training Center - Pawtners - ERP training management system

A dog training center management system where administrator and trainers can manage dogs, training sessions, employees and training programs. 

Greeting page implementation

1. Center showcase
 · Promo banner or carousel with dog training center offers
 · featured training programs section (at least 4 cards)
 · each program card contains:
    	- image
    	- short description
    	- duration
   	- level
   	- “request” button
2. Training request form
  · Clicked “request” opens modal/form
  · Form fields:
 	- owner name
	- contacts
 	- dog name
 	- dog breed
 	- selected program
 	- additional notes
  · Client-side validation for required fields
  · Successful submission shows confirmation message
3. Centralised navigation
· Header nav links
· Login input/button in header for auth users
· Footer with GitHub of the RSS and team’s names

 Login page implementation
1. Input validation
  · Login form contains email and password fields
  · Client-side validation:
	- valid email format
	- password is required
  · clear validation error message
2. Integration with authentication service
  · integration with backend authentication API
  · invalid credentials message handling
  · authorization token storage after successful login
3. Redirection
  · successful login redirects to Dashboard
  · authenticated users cannot access login page directly

Dashboard Page implementation 
 1. Statistics overview
  ·  Total amount of clients
  ·  Total active programs
  ·  Upcoming sessions amount
  ·  Training scheduled for today.
 2. Schedule overview
   · Today’s schedule list
   · Upcoming training sessions
3. Statistics & analytics
   · Popular programs diagram/chart
4. Quick navigation 
   · links/buttons to:
	- clients
	- calendar
	- employees
	- programs
5. Priority clients
  · display pinned/frequently used clients
  · quick nav to client profiles


Client page implementation
1. Display clients list
   · Fetch and display client cards from backend API
   · Each client card contains:
- dog photo
- dog name;
- breed;
- owner name;
- assigned trainer.
2. Client Searching & Filtering
   · Search by:
- dog name;
- owner name;
- breed.
   · Filter by:
- trainer;
- program;
- training status.
3. Interactive client cards
  · hover effect on cards
  · Clicking a card nav to detailed client profile
4. Performance optimization
  · Pagination or lazy loading
5. Interactive client card
  · ‘pin client’ button on each client card
  · if already pinned - visual active status
  ·  ability to remove form pinned clients

Detailed client profile page implementation
1. Display Dog Information
  · Dog photo
  · Dog information:
	- sex;
- breed;
- age;
- weight;
- microchip number;
- vaccination information;
- assigned trainer.
2. Owner info
   · owner name
   · contacts
   · number of dogs owned
3. Health & behavior info
   · Health information section
   · Behavior summary section.
   · Internal trainer notes.	
4. Training progress
   · Training progress tracking:
- basic obedience;
- leash manners;
- recall;
- socialization;
- impulse control.
5. Edit client info
  · Edit mode for all client fields.
  · Add/edit notes.
  · Update dog photo.

Training calendar page implementation
1. Calendar display
  · Calendar with training sessions.
2. Session Management
  · Add training button.
  · Edit/delete training session.
  · Assign trainer and client.
3. Filtering
  · Filter sessions by:
- trainer;
- date;
- program.

Employees/Trainers page implementation
1. Display Employees List
  · Trainer cards with:
- photo;
- full name;
- specialization;
- contacts;
- years of experience;
- role/position.
2. Search Employees
  · Search input for trainers/employees.
3. Employee Management
  · Add an employee button.
  · Edit employee information.
  · Delete employee.
4. Detailed employee info
  · Assigned clients.
  · Assigned programs.
  · Work schedule overview.


Programs/courses page implementation
1. Display Programs List
  · display training programs:
- puppy socialization and manners;
- AKC S.T.A.R puppy program;
- behaviour modification;
- aggression handling;
- after-shelter dog adaptation;
- BAT;
- reactive dog training;
- dogs with special needs;
- senior dogs program;
- public/vet visiting adaptation.
2. Program Cards
  · Each card contains:
- title;
- duration;
- level;
- price;
- edit/delete actions.
3. Program Management
  · Add program button.
  · Edit program information.
  · Delete program.
4. Filtering & Sorting
  · Filter by:
- level;
- category;
- trainer.
  · Sort by:
- price;
- duration;
- Popularity.


Header & nav
1. Header
  · logo/name linking to dashboard
  · burger menu nav:
	- dashboard
	- clients
- employees
- programs
  · login/logout button
  · search input
2. Routing
  · all pages accessible via direct URLs.
  · browser navigation support.
  · protected authorized routes.
  · lazy-loaded pages.
  · 404 page implementation.

Beyond backend API -additional features
1. Internal notes
  · trainers can leave internal notes for dogs and sessions
2. Training session history
  · history of completed training sessions
3. Notifications
  · upcoming training reminders
  · vaccination reminders
4. Local persistence
  · saved filters/search history through localStorage
5. Pinned client persistence
  · pinned clients persist through local Storage or backend database

