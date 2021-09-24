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
  
  - On ACE Toolkit, right click on "Application Development", select "New" --> "Start by creating integration service"
  - Define the operations, input and ouput
  - Modify the Message Flow by going to, Project Name --> Resources --> Message Flow
  - Add Mapping, by dragging Mapping node from Transformation on the pallete
  - Select input and output schema, and output XMLNSC
  - Drag input fields to output field, drag second input field to the task. Modify task into Math Operations --> fn:sum
  
7. Hands-on lab: create a REST API, invoking an external web service  
  
  - On ACE Toolkit, right click on "Application Development", select "New" --> "Start by creating a REST API"
  - Define the REST API Description, with operations, input and ouput
  - Add new "Model" for input and for output (2 models)
  - Add new operation in the "Resources", with method POST / GET
  - Add the subflow by clicking create subflow on right part the operations name
  - Add Mapping, by dragging Mapping node from Transformation on the pallete
  - Select input and output schema, and output JSON
  - Drag input fields to output field, drag second input field to the task. Modify task into Math Operations --> fn:sum
  
