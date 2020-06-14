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
        
        The user can Log out from the application and will be redirected to the login page  
        ![Alt text](/screenshots/Output_7.png?raw=true "Working of Web Sockets")

    8. Validation Part -1 ( Missing Credentials)
        
        The application will give an error if the user try to log in without entering the credentials 
        ![Alt text](/screenshots/Output_8.png?raw=true "Working of Web Sockets")

    9. Validation Part -2 ( Password Incorrect)
        
        The application will block the user to log in if the user try to login with incorrect password
        ![Alt text](/screenshots/Output_9.png?raw=true "Working of Web Sockets")

    10. Validation Part -3 ( Trying accessing the dashboard without logging in the application )
        
        The application will deny the access of the dashboard page without successfully loggging in
        to the application
        ![Alt text](/screenshots/Output_10.png?raw=true "Working of Web Sockets")

    11. Validation Part -4 ( Denial access of Dashboard b )
        
        The application will deny the access of the dashboard page without successfully loggging in
        to the application
        ![Alt text](/screenshots/Output_11.png?raw=true "Working of Web Sockets")

    12. Validation Part -5 ( Registering again the same email address  )
        
        The application will prevent the user to regsiter with the email address which is already taken
        ![Alt text](/screenshots/Output_12.png?raw=true "Working of Web Sockets")
    
    13. Deployed on the cloud (Logged Out version)
        
        The user can easily log out and get redirected to the login page again. This has happened 
        on the cloud. 
        Below screenshot when the application is getting deployed on Heroku

        ![Alt text](/screenshots/heroku_deployment_done.png?raw=true "Working of Web Sockets")

        Below screenshot is when the user is running the application on the cloud and
        get himself logged out

        ![Alt text](/screenshots/Output_13.png?raw=true "Working of Web Sockets")

    ### Installation 
  
        The application requires 'Node.js' to run. Install the dependencies and start the server.
        The following below dependencies were installed on the local environment using npm
        node manager.

    #### To install: 
  
     ```sh
    npm i nodemon --save-dev (only needed in the development environment )
    npm i express -save
    npm i bcryptjs ( to encrypt the stored password )
    npm i passport passport-local ( for authentication )
    npm i ejs
    npm i express-ejs-layouts
    npm i mongoose
    npm i connect-flash ( for flash messaging )
    npm i express-session ( flash depends upon this)
    
     ```
    1. Placed this CDN as the script tag on the front end: [Bootswatch theme](https://bootswatch.com/)
     This provides free themes for the bootstrap.
    2.  Also, placed this CDN as the script this tag on the root page: 
     [Font awesome](https://bootswatch.com/). This was for different font styles
    3. Got the bootstrap dismissable alerts from this URL:
     [Bootstrap Dismissable Alerts](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
     These are used for styling the alert messages such as success or error messages
    4. Also, got some bootstrap dismissable components from this URL:
    [Bootstrap Dismissable components](https://getbootstrap.com/docs/4.5/components/alerts/#dismissing)

    #### Running the Development Server: 
   
     ```sh
    $ npm run dev
     ```

     Application accessible on this URL:
    [Application live on Heroku](https://node-passport-authentication.herokuapp.com/)

    ### Technologies 
   
    - The application was coded in the Visual Studio code IDE. 
    - The application was created using latest versions of Node.js(v10.15.3) and Express (4.17.1).
    - The application uses the passport package and passport-local strategy for authentication
    - The application uses bcryptsjs library to encrypt the stored password and to compare
      the stored password with the current one (during login)
    - The application uses ejs as the templating engine and as ejs does not have the layout,
      hence it also used express-ejs-layouts package
    - The application uses connect-flash library which is basically used in displaying the 
      success or the error messsage displayed by the server. In short, this library is used
      for flash messaging
    - Flash messaging also depends upon the expression session. Hence, the application also uses
      express-session library

    ### Code Snippets 
   
    - The passport local strategy used for authenticating the user
      ![Alt text](/screenshots/code_1.png?raw=true "passport-local")
    - After successfully validating the user, encrypting the password and then storing it
      in the database
      ![Alt text](/screenshots/code_2.png?raw=true "passport-local")
    - Requesting for the flash message before redirecting the user to the failure screen
      or the success screen
      ![Alt text](/screenshots/code_3.png?raw=true "passport-local")
    - Initializing the passport session and declaring the flash global variables in the
      root file (app.js) of the project structure
      ![Alt text](/screenshots/code_4.png?raw=true "passport-local")
    - The application created the partial file which stores the bootstrap 
      dissmisable alert message components.
      ![Alt text](/screenshots/code_5.png?raw=true "passport-local")
    
    
        


