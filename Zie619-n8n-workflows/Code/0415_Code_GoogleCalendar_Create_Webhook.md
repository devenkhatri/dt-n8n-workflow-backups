# Workflow Analysis for Latest Company News Before a Call

## Description
This workflow automatically checks your calendar every morning for meetings or calls with external companies and emails you the latest news about those companies to help you stay informed before your discussions.

## Input Details
The workflow is triggered daily at 7 AM and receives the user's calendar events for the current day from Google Calendar.

## Process Summary
Each morning at 7 AM, the workflow fetches the day's calendar events and filters for meetings or calls that start with 'Meeting with' or 'Call with'. For each matching event, it extracts the company name from the event title, then uses a news API to fetch recent articles about that company. The news articles are formatted into an HTML email and sent to a predefined list of email addresses. If no relevant meetings are found, the workflow ends without sending any emails.

## Output Details
The workflow sends an HTML-formatted email containing the latest news articles about each company the user is meeting with that day, delivered to the configured email recipients.

## Tags
calendar automation, news aggregation, email notification, company research, meeting preparation, Google Calendar, news API, daily digest
