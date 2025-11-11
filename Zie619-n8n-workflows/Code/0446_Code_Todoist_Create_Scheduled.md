# Workflow Analysis for Stickynote Workflow

## Description
This workflow automates the creation of recurring tasks in Todoist based on a template project. It reads tasks with custom scheduling rules (like days of the week and due times), filters them for the current day, and creates new tasks in the Inbox with a 'daily' label. It also cleans up any previously created daily tasks to avoid duplication.

## Input Details
The workflow is triggered on a schedule every day at 5:10 AM and processes tasks from a predefined Todoist template project.

## Process Summary
The workflow starts by fetching all tasks from a template project in Todoist. It parses each task's description to extract scheduling instructions like days of the week and due times. It then filters tasks that match the current day of the week. Separately, it checks the Inbox for tasks labeled 'daily' and deletes them to prevent duplicates. Finally, it creates new tasks in the Inbox for the current day with the parsed due times and a 'daily' label.

## Output Details
The workflow creates new recurring tasks in the Todoist Inbox with appropriate due times and a 'daily' label, and deletes any existing daily tasks to maintain a clean task list.

## Tags
Todoist, task automation, recurring tasks, scheduling, daily tasks, n8n workflow, productivity
