# Salesforce Setup


<h3> Create a Salesforce account: </h3>
Navigate to https://www.salesforce.com/ in the browser.
Click on 'Login' link on the top left. 
If you have already login details, login. If not, click on 'Try for Free' button. Fill up the form with the details and click on 'Start Free Trial'
This will give a 30 day free Salesforce account. The system will send you an email to activate the link. Please check your email (provided at the time of 
registration) (Inbox / Junk / Spam folders) and follow the instructions.

<h3> Developer Edition account creation </h3>
In order to to development using Apex, Visualforce, Lightning, etc, we need to have a trial development account. So, create one using the link:
https://developer.salesforce.com/signup
<br> You can give the company email id as any dymmy email id, but this will be your login id going forward.
Once you sign up, system will sends an email to your email account provided (not the dummy one, there is one more email id you provided at the top) and
you need to follow the instructions in the email.


<h3> IDE Set up: </h3>

How to set up the IDE (Idea IntelliJ) and the plugin Illuminated Cloud, how to retrieve the data and how to push the data to salesforce server.


<h3> Download IntelliJ IDE: </h3>
For Windows OS, https://www.jetbrains.com/idea/download/#section=windows <br>
For Linux OS, https://www.jetbrains.com/idea/download/#section=linux <br>
For Mac OS, https://www.jetbrains.com/idea/download/# <br>

<h3> Download Illuminated Cloud plugin for IntelliJ </h3>
To work with Salesforce Development environment (Apex, Visualforce, Lightning, etc), download the plugin which will fasten the development process.
https://plugins.jetbrains.com/plugin/7831?pr=idea
and install from the Plugins feature <br> (Ctrl + Alt+ S) >> Plugins >> Install Plugin from Disk >> Select the path where you downloaded >> OK

<br> OR <br>

1. Select File >> Settings Or Ctrl + Alt + S
2. Select Plugins on left menu Or Enter Plugins in the filer
3. Enter 'Illuminated Cloud' in the Plugin search field on right side panel and keep 'All plugins' in the 'Show:' drop down.
4. Click OK or Install / Update (if it is already installed and you want to update to latest version) button.

<h3> Retrieving the code from Salesforce Cloud (Server) to Local Repository in the IDE: </h3>
Select the Project Name >> Right click >> Illuminated Cloud >> Retrieve Meta Data <br>
This will open a beyond compare version view of differences in the Server copy and Local copy. Select the files and merge based on the differences and the ones which you want to load.
<br> You can perform this operation from the menu too. Build >> Illuminated Cloud >> Retrieve Meta Data.

<h3> Pushing the code from local repository in the IDE to the Salecforce cloud (Server): </h3>
Select the Project Name >> Right click >> Illuminated Cloud >> Deploy Modified Meta Data <br>
This will open a  window with the files highlighting in a different colors (the color codes shows what it means in the bottom of the window as a legend) 
such as Local Only, Local + Server, Server Only, Subscribed. Select the check boxes at the top and Click OK button. This will sync up the changes to the server.

<h3> To verify the changes on the server side, </h3>
Select the Project Name >> Right click >> Illuminated Cloud >> Show Developer Console. This will takes you to the Salesforce server IDE version and you can search there for the files added in local and merged to the server.

<h3> How to test the classes developed: </h3>
As you have the classes developer, on the Salesforce window, under your name (top right) >> Developer Console. This will open a new window.
<br> Or <br>
From the IDE, Build >> Illuminated Cloud >> Show Developer Console <br>
Debug >> Execute Asynchronous Window (Ctrl  + E) <br>
Enter the code to access the classes / methods in it. 
Check the box 'Open Log' and click on 'Execute' button. This should run open the logs with out put. <br>
<i> Note: </i> As the Salesforce logs so many events, filter the output using 'Filter' check box and type 'DEBUG' to see the output generated from your debug statements in the code.

