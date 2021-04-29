# db_design_final_project
CS3200 Final Project

The project is called Symptoms x Conditions. I am on team 14, and am working independently. My name is Adriell Louis and I am in Section 4 of CS3200
 -This database seeks to simplify the decision making process for healthcare providers and to help patients understand their health more fully. It relates 
 symptoms and conditions so that patients can see what symptoms are associated with a given condition/vice versa.
  -A user can be a healthcare provider or patient. This is represented by a portable enumeration "Role." 
  -Users can have many symptoms, a symptom can have many conditions and users, and a condition can have many symptoms. 
  -Users have an id (int), first name, last name, username, password, email, date of birth (all Strings), and role (enum Role).
  -Conditions have a scientific name, common name (both strings), and id (int).
  -Symptoms have a scientific name, common name, location (all strings), and id (int).
  -UserSymptoms have an id, user id, and symptom id.
  -ConditionSymptoms have an id, condition id, and symptom id.
  -In the database, these structures are related through two classes - UserSymptoms and ConditionSymptoms. Symptoms and conditions are the domain objects; they are related by a many to many relationship with the aforementioned ConditionSymptoms class in the database. Users and Symptoms are related by a Many to Many relationship using the ConditionSymptoms class in the database. There is a One to Many relationship between Users and UserSymptoms and between Symptoms and UserSymptoms, with Usersymptoms having the many end of both relations. Likewise, There is a One to Many relationship between Condtions and ConditionSymptoms and between Symptoms and ConditionSymptoms, with Conditionsymptoms having the many end of both relations.
  -Anyone hoping to see what symptoms are associated with different conditions can make use of this database. It can help healthcare providers make medical decisons, and it can help patients understand their symptoms. 
  -A UML diagram representing this database can be found here: https://lucid.app/lucidchart/invitations/accept/inv_7fbb351d-75b3-4239-9547-9f27c17fc2e0
  -The Repository Interfaces of the code implement the methods of CrudRepository.
  
  
  Unresolved issues with the code: 
  1) new symptoms cannot be created in the webpage

Code renders using the index.html file under webpage/react (below the users folder).
