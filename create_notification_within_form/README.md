# Create a SAE notification within a joined AE and SAE form

``` diff
-When you have two separate forms for AE and SAE then follow 
-the recipe “Create email notifications” → “Emails for specific forms”) 
-for both froms or only for the SAE form.
-Is the SAE documentation included within the AE-form then perform the following steps:
```

In the **FormBuilder**:


1. Select your AE-form, find the Item “Is a SAE”, select it

2. New rule → Generate message if  → “Rule name: New SAE” → New or condition → own item = Yes

3. Under Message “Define New”:

  * Internal Title: “New SAE”
  * Execution “only with value changed”
  * Check HTML
  * Title:  “STUDY-NAME: SAE Notification of Patient <ADD-ID>”
  * Deselect Lab-ID
  * Select Email
  * Under “Form items” →  Questions → select Adverse Event→ Adverse Event Desription
  Make sure to push the “Add” button! (This will deliver the AE description in your Email notification)
  * Attach forms as PDF: check “Own form” 

![sae_notification](fig/ae_sae_form_notification.png)
  
``` diff
Proceed in the same way for the AE notifications in case you need it. 
But normally you will only need the SAE notification.
 ```

AE notificatioin
  * Move on to your AE form, find the Item “Is a AE”, select it
  * New rule “Rule name: New AE” > Generate message if, own item ≠ Yes
  * Under Message “Define New”: Proceed as for SAE and replace the word by AE.

 
In the **AdminTool**:

1. Select the "Ressources" tab
2. Select your project and check the notifications you want to send
3. Select: “Versenden als” →  interne Nachricht →  
Select your project →  Email an alle Teilnehmer des Projektes →  Select the role that should receive the message

  
