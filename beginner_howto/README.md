# secuTrial beginners guide

# Overview

The following topics are covered by this documentation:

- [Introduction](#intro)
- [CustomerAdminTool](#customeradmin)
- [AdminTool](#admin)
- [FormBuilder](#formbuilder)
- [DataCapture](#datacapture)
- [ExportSearchTool](#exportsearch)

<a name="intro" />

# Introduction

This manual is intended to give you a rough overview of secuTrial’s functionalities
without going into too much detail. Also, it may be helpful as an indicator when you
feel lost, which will most likely happen often during your initial user experience.
secuTrial is the software we use to set up electronic case report forms (eCRFs) for clinical studies/trials. It has a browser based interface both for setup and data acquisition.

![](https://placehold.it/15/228B22/000000?text=+) setup

![](https://placehold.it/15/1589F0/000000?text=+) productive

The colors are a good orientation and commonly the secuTrial logo in the top left
will help you assess if you are currently viewing the productive or the development
environment.

Before we get started please keep the following in mind for future reference:

- If in doubt why something is not working check the account permissions in the
AdminTool.

- Never use the browser integrated navigation (←,→,F5). Only use the secuTrial
links.

<a name="customeradmin" />

# CustomerAdminTool

This is the highest order administration and only has one administrative account. Here
you can initialize sub-admin accounts for the different customer areas. 
These accounts allow you to access the AdminTool. Until you are more
familiar with secuTrial you will probably not be using the CutomerAdminTool.


<a name="admin" />

# AdminTool

Here you can register projects/trials and create accounts for yourself
to setup the eCRF and for customers to test and later capture
data. All accounts can be equipped with custom permissions.
Furthermore, this is where you can delete patients.
Mass removal is possible in the development environment:
Patients → select project → clean up → select patients to remove

#### Creating user accounts

In the CustomerAdminTool you need to register yourself as an admin for an area if you
are not registered yet. With this account
you can log in to the AdminTool for the specific area. Here you click ”Participant” and
then create a ”New participant” (bottom left). Enter first name, last name, user-id, 
email and password for the new participant.
Finally, under Centres (bottom of the page) you specify the project, centre and
role for the new participant. ”Save and back” and inform the new participant that the
account is active. If the centre does not yet exist it needs to be created. The same is
true for the role.

<a name="formbuilder" />

# FormBuilder

eCRFs are constructed in the development environment and when they are finished
they are transferred to the productive area. First you need to set up the configuration
(”Edit configuration”). Then you can start building forms and the visit plan.
Forms are made up of questions which are made up of items (Form → Question →
Item). Visit plans are a collection of forms that need to be filled over the course of the
clinical trial. Data entry is possible in the DataCapture module.

<a name="datacapture" />

# DataCapture

This module allows filling the forms that were created in the FormBuilder with specific
data. Within the development area you can enter and delete data in order
to test your implementation. Within the productive area extreme care and caution is
advised (if in doubt do not enter or delete data).

#### Reports

Reports are intended to allow secuTrial users to get rough overviews of their acquired
data. Report templates can be generated in the FormBuilder. Custom reports can be
created by clicking ”Edit reports” and then ”New report”. In some cases it may be
necessary to write SQL queries. For this you need to select ”free SQL”. An overview
of the underlying table structure can be viewed by clicking the ”i” next to ”SELECT
statement”. After creating a report type it needs to be released for certain roles. This
can be achieved in the AdminTool via the ”Ressources” panel. The status must be
checked for a report to work. If the status is not checked it will not appear in the
DataCapture.

#### Import

In most cases data will be manually entered into the eCRF. However, in some cases
batch data needs to be imported. Data imports must be specified in the FormBuilder
for each form family with ”Edit import formats”.

<a name="exportsearch" />

# ExportSearchTool

At some point the clinical investigators will need an export of their data. Old exports
can be viewed in the ”Export history”. If you would like to rerun an export with a
previously defined configuration you can click the ”Export again” (round arrow) on
the left. This will recreate the export with the currently entered data. A new export can
be created by selecting ”Export”. Remember to save your TAN.


This recipe was tested under secuTrial version 5.5.1.10
