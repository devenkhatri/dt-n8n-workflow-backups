# Workflow Analysis for AI-Powered User Interview Workflow

## Description
This workflow automates user interviews using an AI agent. It dynamically generates questions based on a set topic, records user responses, and stores the full interview transcript in a Redis session. Upon completion, the transcript is saved to a Google Sheet and displayed on a custom completion screen.

## Input Details
The workflow is triggered by a form submission where a user provides their name to begin an interview about their experiences with the UK practical driving test.

## Process Summary
1. A user starts the interview by submitting a form with their name, generating a unique session ID and creating an interview session in Redis.
2. An AI agent, powered by the Groq Chat Model, dynamically generates open-ended questions based on the interview topic ("UK practical driving test") and previous answers.
3. The user responds to each question via a form, and both the AI's question and the user's answer are recorded in the Redis session, building a transcript.
4. The workflow checks if the user has requested to "stop interview"; if so, the session memory is cleared, and the workflow concludes, otherwise, it loops for the next question.
5. Upon interview conclusion, the entire session transcript is retrieved from Redis, transformed, and appended to a Google Sheet for data analysis. A dedicated webhook endpoint then retrieves the session data and renders a custom HTML page displaying the full interview transcript.

## Output Details
The workflow produces a dynamic stream of interview questions, stores a comprehensive transcript of the interview in Redis, saves the transcript to a Google Sheet, and presents a customized HTML completion screen with the full transcript.
