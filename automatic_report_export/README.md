# Automatic export of secuTrial reports

```
Note: The automatic transfer of reports is described in 
      the manual of the CustomerAdminTool in section 5.1.
```

1. CustomerAdminTool
2. Click "Schemata"
3. Select "Schema" for which you would like to set up automatic export of reports.
4. Click the checkbox next to "Report-Export".
5. Configure according to your personal specifications.  

```
Note: A detailed explanation of how to set up the server
      is beyond the scope of this recipe and should be
      discussed with a systems administrator.
```

  ![auto_rep_exp_cfg](fig/auto_rep_exp_cfg.png "auto_rep_exp_cfg")

6. FormBuilder
7. Select your project of interest.
8. Click "Edit reports"
9. Select the free SQL report you would like to export.
10. Click the "export" checkbox
11. Specify how often the report should be exported.
12. Specify a file name.

  ![auto_exp_fb](fig/auto_exp_formbuild.png "auto_exp_fb")

The example above will export myfile_name.csv once a day.
