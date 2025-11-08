# Workflow Analysis for AI Interview Agent for UK Driving Test Survey

## Description
This workflow automates user interviews using an AI agent and n8n forms to gather feedback on the UK Practical Driving Test. It asks dynamic questions, records responses in a temporary session, and then saves the complete interview transcript to a Google Sheet for analysis, finally presenting the user with their transcript.

## Input Details
The workflow is triggered by a form submission where the user provides their name to start an interview.

## Process Summary
1. A user starts the interview by submitting their name via a form, which generates a unique session ID and initializes a Redis session to store interview data. 2. An AI Agent, powered by Groq Chat Model, continuously generates and asks open-ended questions related to the UK Practical Driving Test, adapting to previous answers. 3. User responses are captured through a separate form and, along with the AI's question, are stored as a timestamped entry in the Redis session. 4. The interview continues in a loop until the user explicitly indicates they wish to stop, at which point the AI sets a 'stop_interview' flag. 5. Upon stopping, the entire interview transcript from Redis is extracted, transformed, and appended to a Google Sheet, and the session memory is cleared. 6. Finally, the user is redirected to a custom completion screen that fetches and displays the full interview transcript from Redis or a "404 Not Found" message if the session has expired.

## Output Details
The workflow produces a structured interview transcript, which is saved to a Google Sheet, and displays a dynamic HTML completion page containing the user's full interview transcript.
