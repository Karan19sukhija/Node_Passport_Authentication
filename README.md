# Node.js Passport Authentication Application 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

This is a simple MVC Application created with Node.js run time environment, express, passport
(for authentication and login), ejs template view engine, bcryptjs (to encrypt the stored password),
mongoose ( to intergrate with cloud version of MongoDB), Bootstrap 4 ( to download the 
dismissable alerts for the alert messages ) and finally the application get deployed
on Heroku ( Cloud based ' Platform as a service ').

## Table of Contents

  - Features (with screenshots)
  - Installation 
  - Technologies
  - Code Snippet

    ### Features (with screenshots)
  
    1. Home Page
        
        The landing Page of the application is the home page which basically display the user 
        allowing to choose either to register or to login directly (if the user is already registered).
        ![Alt text](/screenshots/Output_1.png?raw=true "Working of Web Sockets")

    2. Registeration Page
        
        The Registeration Page of the application allows the user to register with unique valid email
        id, name and password. We also validated for the confirm password. 
        ![Alt text](/screenshots/Output_2.png?raw=true "Working of Web Sockets")
    
    3. Login Page
        
        After getting registered with the application, the user is redirected to the login
        page. With valid credentials, the user can successfully log in. 
        ![Alt text](/screenshots/Output_3.png?raw=true "Working of Web Sockets")

    4. User details get stored in MongoDB ( Atlas)
        
        Below screenshot clearly shows that the new user ( Sanjay Sukhija ) details gets stored
        in the database. Also note that the password stored is the Hash Value
        ![Alt text](/screenshots/Output_4.png?raw=true "Working of Web Sockets")

    5. Registered User trying to login
        
        The user who has already registered himself with this application can log in
        to this application 
        ![Alt text](/screenshots/Output_5.png?raw=true "Working of Web Sockets")

    6. Dashboard
        
        The user after successfully logging in to the application reaches to the dashboard
        of the application  
        ![Alt text](/screenshots/Output_6.png?raw=true "Working of Web Sockets")

    7. Logging Out
        
        The user can Log out from the application  
        ![Alt text](/screenshots/Output_2.png?raw=true "Working of Web Sockets")

    
    
    
    The approach which this application posses can be seen below in the image:
    
   ![Alt text](/screenshots/socket.png?raw=true "Working of Web Sockets")


