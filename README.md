# db_design_final_project
CS3200 Final Project

 -This database seeks to simplify the decision making process for healthcare providers and to help patients understand their health more fully. It relates 
 symptoms and conditions so that patients can see what symptoms are associated with a given condition/vice versa.
  -A user can be a healthcare provider or patient. Users can have many symptoms, a symptom can have many conditions and users, and a condition can have many symptoms. 
  In the database, these structures are related through two classes - UserSymptoms and ConditionSymptoms. Symptoms and conditions are the domain objects.
  -Anyone hoping to see what symptoms are associated with different conditions can make use of this database. It can help healthcare providers make medical decisons, 
  and it can help patients understand their symptoms. 
