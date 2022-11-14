# Hoteling App v2
Desk Hoteling App
This app uses standard Power Platform Connectors with a SharePoint Backend. 

Hoteling App Screenshot

###### Main Screen
![Screenshot](https://github.com/MSPFE2019/HotelApp/blob/main/HA_Main.png)

###### Search by Map
![Screenshot](https://github.com/MSPFE2019/HotelApp/blob/main/SearchbyMap.jpg)

###### Search by Location
![Screenshot](https://github.com/MSPFE2019/HotelApp/blob/main/SearchbyLocation.jpg)

###### Selected Desk
![Screenshot](https://github.com/MSPFE2019/HotelApp/blob/main/Select_SearchbyMap.jpg)

###### Reserve Desk
![Screenshot](https://github.com/MSPFE2019/HotelApp/blob/main/DeskSelection.jpg)


1. Create SharePoint Lists
2. [Download App](https://github.com/MSPFE2019/HotelApp/blob/main/Hoteling%20App%20v2.msapp)

### Create SharePoint Lists

1. Connect to the destination SharePoint site 
Connect-PnPOnline -Url "https://destinationSite.sharepoint.com/sites/destinationSite"  -UseWebLogin

2. Import the items from the template file
Invoke-PnPSiteTemplate -Path "C:\Temp\SPList.pnp"

Download [SPList.pnp](https://github.com/MSPFE2019/HotelApp/blob/main/SPList.pnp)
###### It will create the following list:

deskList - List of Desk

..*Active Desk - 1

..*Inactive Desk - 0


floormapList - Floor Map list

reservationList - Store reservation for desk


### To import a App:
- Sign into Power Apps and select Solutions from the left navigation.
- Importing an app package
- You can import an app package via the following steps:
- Go to web.powerapps.com
- Select Apps from the left navigation bar
- Select Import package
- Select Upload and select the app package file that you want to import
- Once the package has been uploaded you will need to review the package contents and will need to provide additional input for any item marked with a red icon by selecting the wrench icon for each item and entering the required information.
- Once you have provided all of the required information select Import  
- When import completes you will be automatically redirected to a page (similar to the one below) that outlines whether or not the import operation was successful
- NOTE: If you are importing an app and chose to Update an existing app, the new changes will be saved as a draft of the applications.  You will need to publish those changes in order for them to be available all other users of the applications.





