# ace-workshop  
  
## Workshop Preparation  

Install Postman  
Install App Connect Enterprise Toolkit v11.  
Toolkit can be downloaded from:  
https://www.ibm.com/marketing/iwm/iwm/web/dispatcher.do?source=swg-wmbfd  
  
Run the downloaded file to install. App Connect Enterprise v11 can run on Windows 10, Windows 8, Windows Server 2012, 2016, 2019.  
  
Download ace-workshop.zip to your local drive.  
Open your App Connect Enterprise Toolkit. Right click on the left pane, select "Import", then "Project Interchange File". Browse to the saved zip file and import.


## Workshop Agenda  
  
1. Architecture of App Connect Enterprise  
2. App Connect Developer Toolkit overview
3. Lifecycle of integration development with App Connect Enterprise  
4. Hands-on lab: Create an integration server local  
  
  Open App Connect Enterprise command console and executing the following commands:
  ```
mqsicreatebroker TESTNODE
mqsistart TESTNODE
mqsicreateexecutiongroup TESTNODE -e server
```
6. Hands-on lab: create a web service integration service  
7. Hands-on lab: create a REST API, invoking an external web service  
