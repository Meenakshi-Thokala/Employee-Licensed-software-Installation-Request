# Employee-Licensed-software-Installation-Request:

##youtube link: https://youtu.be/mu1SefGXiuI

# Development Steps

## Step 1: Requirement Analysis

* Identified the business requirement to automate licensed software requests.
* Defined the approval process involving the reporting manager and Software Asset Management (SAM) team.
* Planned the request lifecycle from submission to completion.

## Step 2: Create an Update Set

* Created a new Local Update Set to capture all project configurations.
* Made the Update Set current before starting development.

## Step 3: Create the Service Catalog Item

* Created a catalog item named **Request Licensed Software Installation**.
* Added the item to the **Service Catalog** under the **Software** category.
* Configured the short description and detailed description.

## Step 4: Configure Catalog Variables

Created the required variables:

* Requested For
* Software Name
* License Category
* Cost Center
* Business Justification

Configured appropriate variable types, mandatory fields, default values, and display order.

## Step 5: Configure UI Policy

* Created a Catalog UI Policy.
* Made the **Cost Center** field mandatory only when **License Category = Licensed**.
* Improved the user experience by displaying fields only when required.

## Step 6: Build the Flow Designer Workflow

Designed the automation flow to:

* Trigger when the catalog item is submitted.
* Send approval to the employee's manager.
* Send SAM approval if licensed software is requested.
* Create a Catalog Task after approvals.
* Assign the task to the IT Software Support group.
* Automatically close the Request Item when the task is completed.

## Step 7: Configure Task Assignment

* Configured the Catalog Task assignment.
* Assigned fulfillment tasks to the **IT Software Support** group.

## Step 8: Test the Application

Performed end-to-end testing by:

* Submitting requests for free software.
* Submitting requests for licensed software.
* Verifying approval routing.
* Confirming task creation.
* Validating automatic request closure after task completion.

## Step 9: Validate Results

* Verified that approvals were triggered correctly.
* Confirmed that tasks were assigned to the correct support group.
* Ensured the Request Item status updated automatically.
* Checked that all workflow conditions executed successfully.
