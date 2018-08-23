# Clone-User-in-Salesforce
Clone User in Salesforce with Public Group Membership and Permission Set Assignment

1. Create a visualforce Page "CloneUser.vfp"
2. Create a new Custom Link "Clone User" in the User Detail Page.
3. Add custom link "Clone User" in the User Page Layout.
4. Create a custom field "Cloned From" in User sObject to store the id of User from which the new user is being cloned from.
   - This step is necessary because the value in this custom field will help us to clone the Public Group Membership and Permission Set        Assignment.
5. Add the custom field to user Page Layout.
6. Create a custom Label "UserClonedFromId" to store the Id of the Custom field "Cloned From".
   - You will get this Id by going in the User Edit Page and then right click in the browser > go to inspect element > select the input        field of "Cloned From" field and get the Id and store it in the custom label.
   - Note: When deploying your code from Sandbox to Production the value of this ID will change so change your custom label accordingly.
7. Create a trigger to Clone public Group Membership and Permission Set assignment.
8. Create a test class to test your Trigger.
