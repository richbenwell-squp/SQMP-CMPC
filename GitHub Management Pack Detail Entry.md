# Managing the GitHub Managment Pack Detail Entry

*Pairing with the [Management Pack Index](https://github.com/P2P-Nathan/SQMP-CMPC/blob/master/GitHub%20Managment%20Pack%20Index.md) this JSON file provides the details for a Community Based Management Pack.  The below steps provide documentation on using the file to describe a Management Pack*

## Overview
After the UI in the SCOM console has pulled the [Management Pack Index](https://github.com/P2P-Nathan/SQMP-CMPC/blob/master/GitHub%20Managment%20Pack%20Index.md) the second step proceeds to retrieve the detail file via HTTP GET.  This file is used for the following functions.

* Provided additional detail for the UI
* Indicates where there end user can obtain the pack
* Tracks the version of the pack so that we provide update notifications


## Index JSON structure
```json
{ 
    "ManagementPackSystemName":"SQMP.Community.ManagementPackCatalog",
    "ManagementPackDisplayName":"Community Management Pack Catalog",
    "URL":"http://www.SquaredUp.com/ManagementPacks",
    "Version":"1.2.4.3",
    "Author":"Squared Up Ltd."
}
```

## Property Descriptions

### ManagementPackSystemName
The exact System Name of the management pack.  This will be used to identify which packs are already installed as well as where updates may be available.

### ManagementPackDisplayName
The Display Name of the Management Pack to show in the Catalog

### URL
Where can the lateset version of the pack be obtained from?

### Version
What is the currently released version of the Management Pack?  This value will be evaluated against the currently installed packs to see if updates are available.

### Author
Indicates who wrote the management pack.
