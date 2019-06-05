# secuTrail form import

When setting up a CDMA we often need the same or a similar form of another project — examples are "SAE forms" or "standard questionnaires". Forms in the same secuTrial environment may be copied directly. Forms from CDMAs in other environments need to be exported there (in the FormBuilder "Export/import project setup") and then imported into the CDMA in which the form is needed.

```
Note: check for uniqueness of the form name to be imported
      within the "form family". Duplicate imported form 
      names will get a consecutively number behind the name.
```

### Form import via FormBuilder
1. Make sure the "form family" where the form will be imported exists (or create it).
2. If the "form" to be imported contains "repetition" fields, consider where to save them (or create a corresponding "subform family").
3. Select "Export/import project setup".
4. Select "Browse" and find the *.zip-file of the exported "form".
5. "Upload and Preview"
6. Select the form family (i.e. of type "Visit" or "Casenode") in the drop-down "forms import into".
7. If needed also select the "subform family" ("subforms import into") where the repetitions are imported to.
8. "Finish import"

![importform](fig/import_form.png)
