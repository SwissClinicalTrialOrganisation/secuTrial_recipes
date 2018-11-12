# Create new project

1. Login to the CustomerAdminTool as ‘admin’, select the customer area or define a new one. Select ‘new scheme/ neues Schema’. Note that the name of the new scheme should be in the continuing order and include a german 3-letter abbreviation of the department (“Abteilung”) where the trial takes place and a sequential 2-digit number → 5 characters in total! e.g. (END16).

2. Go to the AdminTool of the respective customer area and select `Participant`/`Teilnehmer`. Select yourself as administrator and click the checkbox ‘Can create and edit new projects`/`Darf Projekte anlegen und editieren`. If the checkbox does not appear, go to the other Admins and disable the checkbox there.

3. Go to the FormBuilder and create a new project. It is automatically assigned to the new scheme.
Project name: Use the official title/name of the trial. If not yet available, use temporarily the CTU name/abbreviation of the trial and change to the official title later, latest before going into production with the eCRF.

4. Go back to the AdminTool and un-check the checkbox again

5. In the AdminTool: (Define at least one centre of the project.)
    • Select `centre` and create a `new centre`
    • Select `participant` and choose yourself as admin. Under ‘Projekt oder Zentrum hinzufügen’ you can choose your project and enable to see the project for all the previously defined centres 

6. In the FormBuilder:
    • Select ‘Edit configuration’. At the level `Additional patient-ID (Add-ID)’ enable ’instead of Pat-ID’ and specify the format: e.g. NNN
    • Select ‘Use project prefix’ and ‘centre prefix’ (This enables you to create the project-prefix in the AdminTool

7. In the  AdminTool: 
    • Select projects, and choose your project. Under Zus-ID, Präfix/Add-ID, prefix  type your project prefix: e.g. TEST-
    • Select centres and choose the centre for your study. Add the  prefix for the Add-ID/ ‘Präfix für Zus-ID’, e.g USB-


Further configurations and visit plan implementation

1. In the FormBuilder:
    • Select New form family→New form→ set the name, check the save checkbox, set the name for the database table. Define at least one question when you like to add a new patient in DataCapture
    • Make sure that check of completion is selected
    • Click on Edit visit plan: Define at least one Initial * / maximal count of planned visits e.g. 1/1
    • Check the box `Preset entry date with current date`. So the date is set with the current date when you add a new patient in DataCapture
    • Click on New visit and name it
    • Click on the checkbox in Form family for your visit to assign the formular to the visit
    • Select Edit Reports→New report→ Patient Overview
      
2. In the AdminTool:Ressources→ Find the report for your study→ select ` Für alle Rollen freigeben’

3. In DataCapture: Select new patient


