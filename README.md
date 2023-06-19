#Description:

Blog Management System is a fullstack web application with user authentication, including blog setup, login,
logout and password reset. 
Registered users can create, set up their own blogs and can see all their content on admin dashboard. 
Readers can comment on the posts and can also reply to the comments.
Readers will get notified to the repiles on their comments via mail using nodemailer.
The web application enables them to peform CRUD operations on their blog content.
Implemented it by leveraging Model-View-Controller (MVC) architecture to separate concerns.
The application utilizes the Socket.IO library to facilitate real-time updates on posts and comments.

#How To Setup:

1) Make a config folder and add cofig.js file in it.
 
2) Paste below code in config.js file

code:

const session_secret = "";
const email_user = "";
const app_password = "";
module.exports = {
    session_secret,
    app_password,
    email_user
}

Follow below steps:
-> Add a secret session key of yours in session_secret
-> Add your gmail in email_user which will sent notifications.
-> Follow below link to setup app_password:
-> link : https://stackoverflow.com/questions/72470777/nodemailer-response-535-5-7-8-username-and-password-not-accepted
-> Enter the generated app password in app_password.

3) Open index.js
mongoose.connect("mongodb://localhost:27017/db_name")
change the db_name to the required database name.

#How to Run:

1) npm install

2) node index.js

2) open below url in browser tab after running above commands in terminal.
link : http://localhost:3000/
