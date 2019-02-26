# Implement an external randomization list into Secutrial
```
Note: Before implementing the randomization make sure you implemented
      the form in which the randomization should be performed.
```

1. Make sure that you are able to randomize in the **CustomerAdminTool**. Therefore:  
    1.1 Select Administrator > select yourself and the specific Customer area.  
    1.2 Mark the Checkbox “Randomisierung-Verwaltung (RV)” and “Randonummern-Freigabe pro Zentrum (RZ)”: This enables you to see the Randomization option in the AdminTool.  
    
 2. In the **FormBuilder**:  
   2.1 Go to Edit configuration, under “Randomization”: Select “configurable”.  
   2.2 Navigate to the form/question in which you would like to implement a randomization.  
   2.3 Create a new item: type: “Configurable Randomization Button”  
   2.4 Algorithm: “External Randomization (with list import)”  
   2.5 Mark the checkbox "Centre assignment": The client should provide a randomization list that includes randomization numbers that are assigned to the centres (for multiple centre studies).  
   2.6 Group (arms): Provide the group names (e.g. “Placebo” and “Verum”).  
   2.7 Ignore the "stratification" checkox.  
   2.8 Leave a message: Inernal Title: Randomization, Trigger: Randomization, Title: Study_name: Randomization of ```<ADD-ID>``` to ```<RANDOM>```, Notes: Text for automatic delivery is checked, contrains Add_ID, Centre and Participant Name and Email  

3. In the **AdminTool** (make sure the form you are incorporating the randomization into is in the visit plan):  
  3.1 Go to the “Randomization” tab in the upper right corner.  
  3.2 Click on “New randomization list”.  
  3.3 Select your project.  
  3.4 Upload your randomization list (csv-file): This should include the randomization number and the randomization group. For multi-centre studies the centre name should also be specified (the centre name should not be included in the csv-file). Prepare the file with only two columns (“Randomization number” and the “Randomization group”) and be aware of the centre order. Order your numbers by centre names! ([example csv](https://github.com/SwissClinicalTrialOrganisation/DM_secuTrial_recipes/blob/master/external_randomization_list/dat/randomization_list_example.csv))   
  For further help, read the recipe [create_randomization_list](https://swissclinicaltrialorganisation.github.io/DM_secuTrial_recipes/create_randomization_list/).    
  3.5 Now you can assign the randomization numbers to the centres.  
  3.6 Under the specific centre in the AdminTool you can also assign the randomization numbers to the centre.  
     
