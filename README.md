# REPORT FOR  NEW HEALTH ORDER PROJECT .
## Introduction: 
![Alt text](New_health_order-NHO-final-/img/screenshots/2024-07-11 (1).png)

The New Health Order focuses on preventive healthcare measures in Ghana.The health system in Ghana prioritizes acute treatments, neglecting preventive measures.This intervention aims to make early detection of infectious diseases and promote sustainable health habits accessible. Many youths and some gadults or old people are suffering from various infectious diseases which they fear to talk about with other people. They fear to be seen in hospitals because they find it shameful to have these diseases like HIV, Hepatitis B. With New Health Order, these people are able to receive medical attention and health education from any where as lon as they make an appointment with the health personnel or advocates via New Health Order website.

# Development of Ne Health Order website.

We developed New Health Order website with aim to enable patients book the medical sessions that we put there. Since, we are currently making the project without focusing on making profits but to improve health, and the fact that medical personnel are few in Ghana, we decided that we schedule the appointments according to the availability of the health advocates working together with New Health Order. 

### Tools used:

Tools	Version
PHP	8.0.28
HTML	HTML5
CSS	CSS6
SQL	

### Functionality:
The website has three main functionalities depending on the user type(admin, health advocate and client).
#### Admin: 
Admin is the person controlling the website, posting the different sessions, adding doctors to the system and keeping track of the data eg different appointments between patients/clients and health advocates.
The admin logs in with a specific email and password.

#### Client: 
This is the person booking the appointment. This person might be a patient looking for a medical intervention or any person who wants health advice or education.
With the website, he or she is able to sign up, login, book different sessions with doctors which are added in by the admin, delete, edit or view account details. He can also see all his appointments in ‘My bookings’.


![Alt text](New_health_order-NHO-final-/img/screenshots/2024-07-11.png)



![Alt text](New_health_order-NHO-final-/img/screenshots/2024-07-11 (5).png)

#### Heath Advocate:
He can use the website to login into his account using the account details provided by the admin. He can view his patients, appointments, cancel different sessions and appointments.

The Health Advocate can be health personnel eg doctor, nurse, laboratory technician or health educators.

![Alt text](New_health_order-NHO-final-/img/screenshots/2024-07-11 (4).png)


## Usage of the website:
### Opening the website with code spaces:

The repository of the website (https://github.com/Bernadettenakazibwe/New_health_order-NHO-final-): Can be opened with code spaces easily. After opening with codespaces you need to run the codes below.

-	docker-compose build
-	docker-compose up

Then, the website will open on **port 80**. But at the beginning, you will need to **start the database** .

### Starting the database:
For the database, you go the ports at the top of your terminal. There will be 3 ports running . Choose **port: 8080** and open it in the webbrowser. This will take you to **phpMyAdmin page** where you will login using the credentials below:

USERNAME	PASSWORD
user	userpassword

From the repository, there is a file named **edoc.sql**.  Download this file by right clicking on it via code spaces and then select download.

**After loging into the phpMyAdmin, you will need to import this edoc.sql database.**

Then, the database will be set and you can now re -run the website to see different functionalities.
As Admin: 

**If you want to login  as Admin, here are the details.**

Email Address	Password
admin@edoc.com    123


### As client: 
If you are a new user without a registered email address and password, you will need to first sign up in order to make an appointment. Then, you can login with the emailaddress and password you signed up with. After signing up, you can do book the appointment an duse different functionalities available.

### As Health Advocate:
At the home page click on the ‘Make Appointment ’ button and the login using the  password and email address you gave the admin while adding you to the system( the health advocate details used by the admin to register this health personnel/ health advocate).

## Problems encountered during the development of the website at the Technical side:
1.	### Adding in docker: 
We faced a huge issue when we uploaded the project to github and opening it with codespaces. The docker failed to work on the local machine . We think we lacked some dependencies on our local machines. So, we decied to continue the development from code spaces. Codespaces was able to add in all the dependencies needed and we were able to use docker though we had to change most of the formats for all php files.

2.	### Uploading to cloud:
We were an enable to upload to the AWS cloud. We tried but with the cloud, we could see only the HTML page and  we could get errors while connecting to the databases forexample during registering and login. So, we decided to staywith docker and make sure the project works with docker atleast. 

3.	### Database connection:
The database does not start automatically on running code: ‘**docker-compose up**’. You need to go to the **port 8080** leading you to phpMyAdmin, where you login with credentials provided above, and then import edoc.sql.

4.	### Port 3306: 
Sometimes after starting the docker, the message appears that the project is running on port 3306 , but when I go to this port, we get error message. We can only see interface from port 80.











