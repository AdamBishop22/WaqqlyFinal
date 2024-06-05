File path navigation ----------------------------
HTML files stored in Public file (index.html is the main page)
Main JavaScript code is located in /public/js/main.js
-------------------------------------------------

Deployment instructions:
To deploy this project, a Firebase project needs to be created using the "hosting" and "realtime database" Firebase services at https://console.firebase.google.com/.

Deployment steps
1) Create a new app project
2) Specify Web App for project type
3) Follow steps on firebase to create hosting for the app (Ensure set up firebase hosting is checked)
4) Follow steps to add firebase SDK (npm install firebase)
5) From the JavaScript code provided by firebase setup Select the code under the comment "// Your web app's Firebase configuration" and replace the config under the same section in /public/js/main.js
*Replacing this config applies your own firebase project details to the app
6) Follow the final steps on firebase to install firebase CLI deploy firebase hosting (Ensure this setup process incldues and links a realtime database)
7) Once app is deployed, ensure database is linked by filling in one of the forms on the Waqq.ly webpage
8) Check to see if the form entry has been added to the realtime database (Database data can be viewed from the project dashboard on firebase)
9) If data does not pupulate database, you may need to enable write access by changing ".write:" to "true" in the "database.rules.json" file; then redeploy and try again
10) The app should now fully be hosted with a functioning database for registering dog walkers and dogs.