# Ex-05_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

![image](https://github.com/user-attachments/assets/9b96865f-767c-49d0-b931-70b12d595f85)

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
![image](https://github.com/user-attachments/assets/26ffb95e-2f88-496e-8f0a-3f42b9f58587)
 
Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/user-attachments/assets/cc982df8-3084-42af-9100-cd1fc111fbf4)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

![image](https://github.com/user-attachments/assets/73a0632f-dba5-4ad0-8c32-a7e73b8a2ff0)

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).

![image](https://github.com/user-attachments/assets/b4fe87f9-8aed-4e3f-9d02-6fb0a8c5a4f9)


Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.
Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 
Step 4: Carefully select your RESTful resource (web service) and click OK.
 
![image](https://github.com/user-attachments/assets/7fd04997-fcc3-4bfa-b6ec-82a5d43563fc)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/user-attachments/assets/b8786578-1b66-42e2-9117-fad19ff7be5d)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 ![image](https://github.com/user-attachments/assets/1bbe36d0-8fa6-4968-9588-2f75a816afe6)

Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/user-attachments/assets/ff809ff5-84f5-44cd-9c1a-b2c2cc27e5a9)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![image](https://github.com/user-attachments/assets/a631a569-05f0-481c-bfda-03d4d319b137)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/user-attachments/assets/6b1dd699-8af0-4714-a418-f4169c25c4a7)


Step 11: Save the project and build it.

![image](https://github.com/user-attachments/assets/32ae7c37-14dc-41c0-84ff-40016cf3cc39)

Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
