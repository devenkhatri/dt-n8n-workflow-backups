# Workflow Analysis for Email Approval with Google Sheets

## Description
This workflow automates an email approval process, where incoming emails are parsed for specific information, a Google Sheet is updated, and approval emails are sent out. The sheet tracks the status of each approval request.

## Input Details
The workflow is triggered manually and requires email content as input.

## Process Summary
The workflow begins by extracting specific data points such as name, email, and company from the manually entered email body. This information is then used to update a Google Sheet with a pending status. Subsequently, an approval email, including the extracted data and an approval link, is sent to a specified approver. The approval link contains a webhook that, when clicked, updates the status in the Google Sheet to either "Approved" or "Rejected" based on the approver's action. Finally, a confirmation email is sent to the original sender indicating the approval status of their request.

## Output Details
The workflow updates a Google Sheet with approval statuses and sends approval/rejection emails to relevant parties.
