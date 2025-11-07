# Workflow Analysis for Sales Assistant Build Workflow

## Description
This workflow automates the process of researching sales prospects and generating personalized sales outreach messages based on the gathered information and existing testimonials, updating all data in a Google Sheet.

## Input Details
The workflow is manually triggered and fetches prospect data including Name, Email, Company Name, Website, Business Type, and Project from a Google Sheet named "Meeting Data".

## Process Summary
First, the workflow retrieves prospect details from the "Meeting Data" Google Sheet. An AI Agent then researches the company using the Tavily tool to get an overview, tech stack, and recent updates, and uses a "Product List" Google Sheet to suggest relevant solutions. This gathered information is then written back into the "Meeting Data" Google Sheet. Subsequently, a "Sales Writing Assistant" AI agent utilizes the researched data and a "Testimonials Tool" Google Sheet to craft a personalized email subject, email body, and SMS message. Finally, these generated outreach messages are updated into the "Meeting Data" Google Sheet.

## Output Details
The workflow updates the "Meeting Data" Google Sheet with comprehensive company research (overview, tech stack, updates, solutions) and personalized sales outreach messages (email subject, email text, SMS).
