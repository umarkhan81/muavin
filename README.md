Complete Muaavin project code for the mobile apps and backend services.

Muaavin project has the following divisions:
•	Muaavin client app. (Android app.)
•	Muaavin Admin app. (Android app.)
•	Muaavin backend services (Java)
•	Database (MySQL)
All source code for mobile apps. , services and database schema is available on the following GitHub URL:
https://github.com/codeforpakistan/muavin
In the above mentioned GitHub repo, following folders contain:
Muaavin-Android contains code for Muaavin client app.
Muaavin-AndroidAdminModule contains code for Muaavin Admin app.
Muaavin-Web-master contains code for services, also having Muaavin database.sql database schema.
Environment Setup
•	Android Studio
•	Eclipse J2EE
•	Apache Tomcat
•	MySQL
Following is the deployment procedure:
•	For Backend Database and services:
•	Use the Muaavin database.sql file inside Muaavin-Web-master folder to restore database in MySQL.
•	Now run the code for backend services in eclipse. Export it and generate .war file.
•	Publish the services using Apache Tomcat.
•	For Muaavin Admin app.
•	Get the IP and Port of the services hosted in the above step.
•	Import code for Muaavin admin app. inside android studio.
•	Open  com.cfp.muaavin.BusinessLogic.Admin.java and replace baseURL with the IP and Port of your hosted services IP and port.
•	Build and run the project.
•	For Muaavin Android app.
•	Import code for Muaavin client app. inside android studio.
•	For services:
•	Open  com.cfp.muaavin.ui.MenuActivity.java and replace baseURL with the IP and Port of your hosted services IP and port.
•	For Facebook api integration:
•	Create a new application on Facebook developer console. https://developers.facebook.com/ 
•	Get App ID of application from Dashboard.
•	Open strings.xml and replace facebook_app_id with App ID and fb_login_protocol_scheme with fb<App ID>
•	Open AndroidManifest.xml and replace the App ID mentioned in provider with your App ID.
•	For Twitter: 
•	Create a new application in twitter. https://apps.twitter.com/app/new 
•	Get Consumer Key and Consumer Secret.
•	Open  com.cfp.muaavin.ui.MenuActivity.java and replace TWITTER_KEY with the Consumer Key and TWITTER_SECRET with Consumer Secret.
•	For Fabric api key:
•	Login to Fabric account & open https://fabric.io/kits/android/crashlytics/install
•	Find the meta-data code block in AndroidManifest.xml
•	Find your fabric api Key pre filled in the code.
•	Open AndroidManifest.xml and replace the fabric api key mentioned in meta-data tag with your fabric api key.
•	For Page Posting:
•	Create a facebook page.
•	Get its Page Id and generate a non-expiry Page Token for the page.
•	Open com.cfp.muaavin.ui.MenuActivity.java and replace pageId and pageToken with your Page Id and Page Token.
•	Build and run the project.
