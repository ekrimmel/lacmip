---
title: Groups
navcat: Modules
tags:
last_modified_at: 2019-06-18
---
Groups are a useful way to save and share recordsets in EMu. If you have a set of search criteria that you frequently use, or a set of specific records that you need to share with another person, groups will help.

To access an existing group, navigate to *Tools > Group > Retrieve Group* and select the group you are looking for. Note that groups exist within modules, i.e. the module you are in affects the groups you see listed.

## Static groups

A static group is a set of records that remains the same. Once created, re-opening the static group will display the same records every time. To create a static group in any module:
1. Run a search.
1. From the results, go to *Tools > Group > All Records in Results...*
1. Click *New* to save new group. You will need to give your new group a title. *Description*, *Purpose*, and *Status* are optional.
1. If you would like this group to be available to other EMu users, navigate to *Security* tab and select them, as shown in the image below. Only the creator (you) can edit this group later.
1. Click *OK* to save.

{% include figure image_path="/assets/images/groups_static.png" alt="image of EMu groups dialog windows" caption="EMu dialog windows when you create a new static group. Notice that the general tab tells you how many records you are including in the group (circled in red, above). To share your new group with other EMu users, or user groups, find and *Add* them on the *Security* tab."%}

## Dynamic groups

A dynamic group of records is a set that may change each time the group is opened. Whereas a static group saves a list of records, a dynamic group saves search criteria. Re-opening a dynamic group will run the saved search again and refresh the recordset. To create a dynamic group in any module:
1. Run a search.
1. From the results, go to *Tools > Group > Save Search Criteria...*
1. Click *New* to save new group. You will need to give your new group a title. *Description*, *Purpose*, and *Status* are optional. Note that the *General* tab shows "Unknown" for *Records* instead of a numerical value; this is because the number of records in a dynamic group changes every time it is retrieved.
1. If you would like this group to be available to other EMu users, navigate to *Security* tab and select them, as shown in the image below. Only the creator (you) can edit this group later.
1. Click *OK* to save.

## Adding or subtracting records

**Adding records** to an existing static group is simple. From any record or list of records, go to *Tools > Group > All Records in Results...* **or** *Tools > Group > Current Record* **or** *Tools > Group > Selected Records*, depending on which record(s) you want to add. When the groups dialog window appears, instead of clicking *New*, highlight the existing group that you want to add the record(s) to and select *Add*.

Similar to above, you may also **replace a group** with any record or list of records. Follow the same steps as above, but select *Replace* instead of *Add*.

Note that you cannot add records to or subtract records from a dynamic group.
{: .notice--warning}

You can **subtract records** from an existing static group in one of two ways. The most straightforward way is by replacing the group. To use this method:
1. Retrieve the group.
1. Select the records you wish to subtract and remove them from the set by going to *File > Discard > Selected Records*. Discard does not delete records, only removes them from view.
1. Replace the group by going to *Tools > Group > All Records in Results...*, selecting the same group name, and clicking *Replace*.

The other way to **subtract records** is via the Groups module. If you do not see the Groups module in your EMu, you can ask the Museum's database manager to make it available to you. To subtract records via the Groups module:
1. Open the Groups module and search for your group in the field *Name*.
1. From the results, double-click to open your group.
1. Navigate to the *Static* tab, where you should see a list of records included in the group, as shown in the image below.
1. Highlight the record(s) you wish to remove, then right-click and select *Delete*. This will remove them from the group, **not** delete the records entirely.
1. Save and exit the groups module.

{% include figure image_path="/assets/images/groups_subtract.png" alt="image of EMu groups module" caption="Screenshot of the *Static* tab in the Groups module, showing how to subtract records from a group."%}

## Adjusting group security
Members of the Invertebrate Paleontology permission group have the ability to set the security on groups that they create. This is important because by default users can only edit or delete groups that they create. The most common use case for adjusting these default security settings is in managing Catalogue record groups for [label printing]({{ site.baseurl }}/documentation/labels/). To adjust the security settings:
1. Search for a group in the Groups module as described under the section on subtracting records, above.
1. From the results, double-click to open your group.
1. Navigate to the *Security* tab, where you should see a list of users and user permission groups, as shown in the image below. You can select "Add" if you do not already see the user or permission group you need.
1. Clicking on any user or user permission group from the list will allow you to edit its permissions by checking or unchecking the "Edit" and "Delete" boxes. For label printing groups, you will want to check both "Edit" and "Delete" for Invertebrate Paleontology, and "Edit" for whichever IP Cataloger user you are creating this group for.

{% include figure image_path="/assets/images/groups_security.png" alt="image of EMu groups module" caption="Screenshot of the *Security* tab in the Groups module, showing where to adjust the security settings for user permission groups (left) and individual users (right)."%}

## Shared groups

Groups that are shared with your user permission group will be visible when you go to retrieved a group. An incomplete list of shared groups is highlighted below.

### Multimedia

- **Statz Publications**: (static) scanned and annotated PDFs of Georg Statz publications, most attached to [bibliography records]({{ site.baseurl }}/documentation/bibliography/)  but not all

### Sites

- **CSC Localities**: (static) sites affiliated with the Cretaceous Seas of California project
- **EPICC Localities**: (static) sites affiliated with the Eastern Pacific Invertebrate Communities of the Cenozoic project
- **Non-Marine Localities**: (static) non-marine sites
- **CSC Georeferencing Progress**: (dynamic) CSC sites that have a latitude/longitude assigned via a trusted method, either "LACMIP Georeferencing..." or from the collector ("GPS" or "transcribed...")
- **EPICC Georeferencing Progress**: (dynamic) EPICC sites that have a latitude/longitude assigned via a trusted method, either "LACMIP Georeferencing..." or from the collector ("GPS" or "transcribed...")
