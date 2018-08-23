# Clone-User-in-Salesforce
Clone User in Salesforce with Public Group Membership and Permission Set Assignments.

1. Create a custom field "Cloned From" in User sObject to store the id of User from which the new user is being cloned from.
   - This step is necessary because the value in this custom field will help us to clone the Public Group Membership and Permission Set        Assignment.
   
2. Add the custom field to user Page Layout.

3. Create a custom Label "UserClonedFromId" to store the Id of the Custom field "Cloned From".
   - You will get this Id by going in the User Edit Page and then right click in the browser > go to inspect element > select the input        field of "Cloned From" field and get the Id and store it in the custom label.
   - Note: When deploying your code from Sandbox to Production the value of this ID will change so change your custom label accordingly.
   
4. Create a visualforce Page "CloneUser.vfp".

5. Create a new Custom Link "Clone User" in the User Detail Page.

6. Add custom link "Clone User" in the User Page Layout.

7. Create a trigger to Clone public Group Membership and Permission Set assignment.

8. Create a test class to test your Trigger.
