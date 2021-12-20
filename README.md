# Shreyanshi-s-Interview-Scheduler-Backend



Basic Requirements
An interview creation page where the admin can create an interview by selecting participants, start time and end time. Backend should throw error with proper error message if:
1. Any of the participants is not available during the scheduled time (i.e, has another interview scheduled)
2. No of participants is less than 2
3. An interviews list page where admin can see all the upcoming interviews.
Note: No need to add a page to create Users/Participants. Create them directly in the database



How to build and run this project
1. Clone this repository.
2. Execute npm install
3. Make sure MySQL is installed your system.
4. Login to MySQL using your root user.
5. Execute the following MySQL Queries:
6. CREATE USER 'username'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
7. GRANT ALL PRIVILEGES ON DB_NAME.* TO 'username'@'localhost';
8. FLUSH PRIVILEGES;
9. exit
10. Rename the following files:
.env.example --> .env
ormconfig.json.example --> ormconfig.json
11. Provide username, password and database (DB_NAME) info in ormconfig.json for typeorm to properly connect to the Database.
12. Provide NODE_ENV (dev/prod), PORT, EMAIL, PASSWORD in .env file
13. Execute npm start.
