# Workflow Analysis for TheHive Case Management

## Description
This workflow demonstrates how to interact with TheHive platform to manage cases, including creating a case, creating an observable with a custom type, and then retrieving the case details.

## Input Details
The workflow is triggered manually, allowing for immediate execution and testing.

## Process Summary
First, the workflow creates a new case in TheHive with a specified title, description, and severity. Next, it adds an observable to the newly created case, specifying its data, custom type, and IOC (Indicator of Compromise) status. Finally, it retrieves all details of the case, including the ID generated in the initial step, to confirm the operations.

## Output Details
The workflow outputs the details of the created case and observable, then retrieves and displays the full case details from TheHive.
