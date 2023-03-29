# Designing-Azure-Logic-Apps

![Screenshot 2023-03-29 at 2 30 56 PM](https://user-images.githubusercontent.com/121365233/228653044-87779682-e5a8-4d15-863b-afb2a26c1a08.png)

## Create a Storage Account and Container

--Click on "Create a resource" button in the top left corner of the portal. --Search for "Storage Account" and select it from the results.
--Fill in the required information in the wizard to create the storage account. --You will need to provide a unique name for the account, 
select the subscription and resource group, and choose a location. --Once the storage account is created, navigate to the "Containers" tab 
and create a new container within the storage account.

##Create the First Logic App

--Click on "Create a resource" button in the top left corner of the portal. --Search for "Logic App" and select it from the results.
Fill in the required information in the wizard to create the logic app. You will need to provide a unique name for the app, 
select the subscription and resource group, and choose a location.
Once the logic app is created, navigate to the "Logic app designer" tab and create a new trigger by selecting the "Request - Response" option.
Add a new step by selecting the "Azure Blob Storage" option and selecting the previously created storage account and container.
Add another step by selecting the "Blob - Create blob" option and configure it to create a new blob file in the container.
Save and run the logic app to test if it's creating a new blob file in the storage account.

![Screenshot 2023-03-29 at 4 06 43 PM](https://user-images.githubusercontent.com/121365233/228655246-2f248cf2-2b9b-4fd8-8881-ba4a2df07df2.png)

![Screenshot 2023-03-28 at 10 19 46 PM](https://user-images.githubusercontent.com/121365233/228655420-488e7cc0-7269-4981-a8a1-1253ed418aec.png)

##Create the Second Logic App

--Once the logic app is created, navigate to the "Logic app designer" tab and add a new trigger by selecting the "When a blob is added or modified (properties only)" option.
--Configure the trigger to monitor the previously created container in the storage account.
--Add another step by selecting the "Office 365 Outlook - Send an email" option and configure it to send an email notification whenever a new blob file is created in the container.
Save and run the logic app to test if it's sending email notifications whenever there's a change in the storage account.

![Screenshot 2023-03-29 at 4 03 13 PM](https://user-images.githubusercontent.com/121365233/228655871-00031c71-2bb6-4cf8-956e-9d33fbc28da4.png)

![Screenshot 2023-03-28 at 10 22 02 PM](https://user-images.githubusercontent.com/121365233/228655985-1046902c-a871-4a97-af62-179d55f99b31.png)

![Screenshot 2023-03-29 at 4 02 35 PM](https://user-images.githubusercontent.com/121365233/228656026-278fc3c8-2846-4384-a300-cfe7b14c9544.png)

