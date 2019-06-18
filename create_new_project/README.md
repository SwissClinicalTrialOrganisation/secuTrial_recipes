# Create new project

1. Login to the CustomerAdminTool, select the customer area or define a new one. Select "new scheme/neues Schema". Create the adminuser as well as the "new scheme/neues Schema".
2. Login to the AdminTool, set you password. In the AdminTool navigate to the respective customer area and select "Participant/Teilnehmer". Select yourself as administrator and click the checkbox "Can create and edit new projects/Darf Projekte anlegen und editieren".  

    ```
    Note: If the checkbox does not appear, go to the other
      admin accounts and disable the checkbox there.
    ```

3. Go to the FormBuilder and create a new project. It is automatically assigned to the new scheme.  

    ```
    Note: If you are not sure whether to select 
        "Registry" or "Part project" you should 
        likely select "Registry".
    ```

4. Go back to the AdminTool and un-check the checkbox that allows you to create new projects. 

5. In the AdminTool: (Define at least one centre of the project.)  (Make sure to refresh the browser)  
    5.1 Select "centre" and create a "new centre"  
    5.2 Select "participant" and choose yourself as admin. Under "Projekt oder Zentrum hinzufügen" you can choose your project and enable to see the project for all the previously defined centres  

6. In the FormBuilder:  
    6.1 Select "Edit configuration". At the level "Additional patient-ID (Add-ID)" enable "instead of Pat-ID" and specify the format: e.g. NNN (Click on set)  
    6.2 Select "Use project prefix" and "Use centre prefix" (This enables you to create the project-prefix in the AdminTool  

7. In the  AdminTool:  
    7.1 Select projects, and choose your project. Under Zus-ID, Präfix/Add-ID, prefix  type your project prefix: e.g. TEST-  
    7.2 Select centres and choose the centre for your study. Add the  prefix for the Add-ID/ "Präfix für Zus-ID", e.g USB-  

# Further configurations and visit plan implementation

1. In the FormBuilder:  
    1.1 Select New form family → New form → set the name, check the save checkbox, set the name for the database table. Define at least one question when you like to add a new patient in DataCapture.  
    1.2 Make sure that check of completion is selected.  
    1.3 Click on Edit visit plan: Define at least one Initial * / maximal count of planned visits e.g. 1/1  
    1.4 Check the box "Preset entry date with current date". This sets the entry date to the current date when you add a new patient in DataCapture.  
    1.5 Click on New visit and name it.  
    1.6 Click on the checkbox in Form family for your visit to assign the form to the visit.  
    1.7 Select Edit Reports → New report → Patient Overview  
      
2. In the AdminTool:Ressources → Find the report for your study → select "Für alle Rollen freigeben"

3. In DataCapture: Click "New patient"

 ```
    Note: This will be enabled once you edit the participant role.
          See "create user logins".
 ```


This recipe was tested under secuTrial version 5.5.1.10
