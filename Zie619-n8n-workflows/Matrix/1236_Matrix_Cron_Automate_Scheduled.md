# Workflow Analysis for Coffee Bot (Matrix)

## Description
This workflow automates the process of organizing virtual coffee groups for employees within a Matrix chat channel. It ensures fair and randomized grouping for weekly social interactions.

## Input Details
The workflow is triggered weekly every Monday at 10 AM by a scheduled cron job.

## Process Summary
The workflow starts by sending a greeting message to a designated Matrix room. It then retrieves a list of all employees who are members of the specified coffee chat Matrix room. Next, it shuffles the list of employees and divides them into randomized groups, aiming for an ideal group size of three, ensuring no group has only one person. Finally, it announces these newly formed virtual coffee groups to the Matrix room. The workflow also includes an error handler to manage execution failures.

## Output Details
The workflow outputs announcements of the randomized virtual coffee groups to a specified Matrix room.

## Tags
automation, n8n, production-ready, excellent, optimized, Matrix, coffee chat, group assignment, scheduling
