# Workflow Analysis for Pyragogy AI Village - Orchestrazione Master (Architettura Profonda V2)

## Description
This workflow orchestrates a dynamic sequence of AI agents to process user input, such as summarizing, synthesizing, peer reviewing, and archiving content. It intelligently determines the best agent order, supports iterative refinement based on feedback, and requires human approval before finalizing archival content. Approved content is stored in a database and optionally synced to GitHub.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing user-submitted data in the request body.

## Process Summary
The workflow starts by validating the database connection and then uses a Meta-Orchestrator AI to determine the optimal sequence of specialized agents (e.g., Summarizer, Synthesizer, Peer Reviewer) based on the input. It executes each agent in order, collecting their outputs and contributions. If multiple reviewing agents flag major issues, the workflow loops back to the Synthesizer for up to two rounds of refinement. When the Archivist agent is reached, it prepares content for human review via email; only approved content is saved to the database and optionally committed to GitHub. The final output includes all agent contributions and the processed result.

## Output Details
The workflow returns a JSON response with the final processed output, a list of agent contributions, and the executed agent sequence; it also saves approved content to a PostgreSQL database and may push it to a GitHub repository.

## Tags
AI orchestration, agent workflow, content synthesis, human-in-the-loop, archival system, iterative refinement, n8n, OpenAI, PostgreSQL, GitHub integration
