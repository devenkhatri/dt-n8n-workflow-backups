# Workflow Analysis for Hey Siri, Ask Agent Workflow

## Description
This workflow integrates with Apple Shortcuts to trigger an n8n AI Agent using a "Hey Siri" command. The shortcut captures spoken input, transcribes it, and sends it to the workflow. The AI Agent processes this input, incorporating the current date and time for context, and Siri then dictates the generated response back to the user.

## Input Details
The workflow is triggered by a POST request to a webhook node named "When called by Apple Shortcut", receiving spoken input from an Apple Shortcut.

## Process Summary
The workflow starts when an Apple Shortcut calls a webhook with spoken input. This input, along with the current date and time, is passed to an AI Agent. The AI Agent, utilizing an OpenAI Chat Model, processes the request to generate a concise, voice-friendly answer. Finally, the workflow sends this generated text response back to the Apple Shortcut.

## Output Details
The workflow returns the AI Agent's text response to the Apple Shortcut, which is then dictated by Siri to the user.

## Tags
Siri, Apple Shortcuts, AI Agent, Voice Assistant, OpenAI, Automation, Chatbot, Mobile, Productivity
