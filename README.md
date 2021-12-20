# Shreyanshi-s-Interview-Scheduler-Backend



Basic Requirements
An interview creation page where the admin can create an interview by selecting participants, start time and end time. Backend should throw error with proper error message if:
Any of the participants is not available during the scheduled time (i.e, has another interview scheduled)
No of participants is less than 2
An interviews list page where admin can see all the upcoming interviews.
Note: No need to add a page to create Users/Participants. Create them directly in the database



How to build and run this project
Clone this repository.
Execute npm install
Make sure MySQL is installed your system.
Login to MySQL using your root user.
Execute the following MySQL Queries:
CREATE USER 'username'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
GRANT ALL PRIVILEGES ON DB_NAME.* TO 'username'@'localhost';
FLUSH PRIVILEGES;
exit
Rename the following files:
.env.example --> .env
ormconfig.json.example --> ormconfig.json
Provide username, password and database (DB_NAME) info in ormconfig.json for typeorm to properly connect to the Database.
Provide NODE_ENV (dev/prod), PORT, EMAIL, PASSWORD in .env file
Execute npm start.
