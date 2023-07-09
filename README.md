# Salesforce Developer Virtual Internship

## Description:
I have successfully completed the Salesforce Developer Virtual Internship, a comprehensive program designed to enhance skills in Salesforce platform development. Throughout this internship, I gained proficiency in various technologies and skills, including Salesforce Platform, Lightning Web Components, JavaScript, Application Lifecycle Management, Object-Oriented Programming, Apex, System Integration, SOQL/SOSL, Web Services, and more. The program provided me with hands-on training, self-paced courses, and mentorship to develop practical expertise in Salesforce development.

## Tasks:

1. Apex Triggers:
   - AccountAddressTrigger.apxt: This trigger runs before inserting or updating an Account record. If the "Match_Billing_Address__c" field is set to true, it copies the BillingPostalCode value to the ShippingPostalCode field.

   - ClosedOpportunityTrigger.apxt: This trigger runs after inserting or updating an Opportunity record. If the StageName field is set to "Closed Won," it creates a new Task with the Subject "Follow Up Test Task" and associates it with the Opportunity.

2. Apex Testing:
   - VerifyDate.apxc: This class contains a method called "CheckDates" that takes two Date parameters. It checks if the second date is within the next 30 days of the first date. If it is, it returns the second date; otherwise, it returns the end of the month of the first date.

   - TestVerifyDate.apxc: This class contains test methods to verify the functionality of the VerifyDate class. It tests scenarios where the second date is in the past, within 30 days, and more than 30 days from the first date.

   - RestrictContactByName.apxt: This trigger runs before inserting or updating a Contact record. It checks if the Last Name is set to "INVALIDNAME" and throws an error if it is.

   - TestRestrictContactByName.apxc: This class contains a test method to verify that the RestrictContactByName trigger throws an error when the Last Name is set to "INVALIDNAME."

3. Asynchronous Apex:
   - AccountProcessor.apxc: This class contains a method called "countContacts" that takes a set of Account IDs. It queries for the specified accounts and their related contacts. It updates the Number_of_Contacts__c field on each account based on the count of contacts associated with it.

   - AccountProcessorTest.apxc: This test class creates an Account record, associates it with multiple Contact records, and tests the functionality of the AccountProcessor class by verifying that the Number_of_Contacts__c field is updated correctly.

   - LeadProcessor.apxc: This class implements the Batchable interface and processes batches of Lead records. It sets the LeadSource field to "Dreamforce" for each lead in the batch.

   - LeadProcessorTest.apxc: This test class creates Lead records and tests the functionality of the LeadProcessor class by verifying that the LeadSource field is updated correctly.

   - AddPrimaryContact.apxc: This class implements the Queueable interface and adds a primary contact to multiple accounts based on a specified state. It queries for accounts with a matching BillingState and creates new Contact records associated with those accounts.

   - AddPrimaryContactTest.apxc: This test class tests the functionality of the AddPrimaryContact class by verifying that the correct number of Contact records is created.

   - DailyLeadProcessor.apxc: This class implements the Schedulable interface and updates Lead records by setting the LeadSource to "DreamForce" for leads with an empty LeadSource field.

   - DailyLeadProcessorTest.apxc: This test class schedules the DailyLeadProcessor class and verifies that the LeadSource field is updated correctly.

4. Apex Integration Services:
   - AnimalLocator.apxc: This class makes a REST callout to an external service to retrieve the name of an animal based on its ID.

   - AnimalLocatorTest.apxc: This test class verifies the functionality of the AnimalLocator class by mocking the HTTP callout and asserting the expected animal name.

   - ParkLocator.apxc: This class makes a SOAP callout to an external service to retrieve a list of parks based on a country name.

   - ParkLocatorTest.apxc: This test class verifies the functionality of the ParkLocator class by mocking the SOAP callout and asserting the expected park name.

   - AccountManager.apxc: This class exposes a RESTful web service endpoint to retrieve account details and associated contacts.

   - AccountManagerTest.apxc: This test class verifies the functionality of the AccountManager class by simulating a REST request and asserting the expected account details.

5. Apex Specialist Superbadge Codes:
   - MaintenanceRequestHelper.apxc: This class contains a method called "updateWorkOrders" that updates work orders based on changes in Case records. It creates new Case records with specific criteria and inserts them.

   - MaintenanceRequest.apxt: This trigger runs before and after updating Case records. It calls the updateWorkOrders method from the MaintenanceRequestHelper class.

   - WarehouseCalloutService.apxc: This class makes a REST callout to an external warehouse system to retrieve equipment records. It upserts the received equipment records in Salesforce.

   - WarehouseCalloutServiceMock.apxc: This mock class simulates the REST callout response for testing purposes.

   - WarehouseCalloutServiceTest.apxc: This test class verifies the functionality of the WarehouseCalloutService class by mocking the REST callout and asserting the expected equipment records.

   - WarehouseSyncSchedule.apxc: This class implements the Schedulable interface and enqueues a job to synchronize warehouse data using the WarehouseCalloutService class.

   - WarehouseSyncScheduleTest.apxc: This test class verifies the scheduling logic of the WarehouseSyncSchedule class by asserting the scheduled job's ID.

6. Lightning Web Components (LWC) and APIs:
   - Set up Visual Studio Code (VS Code) and Salesforce CLI for development.
   - Explored Lightning Web Components (LWC) and their basics.
   - Learned about integrating Salesforce org with VS Code environment.
   - Explored the use of Lightning Components in Lightning Experience.
   - Got familiar with REST API and SOAP API.

I successfully completed all the requirements of the internship, including the guided project and SuperBadges. This internship has equipped me with the necessary skills and knowledge in Salesforce development, allowing me to contribute effectively in this field.
