# Workflow Analysis for Automate Competitor Research with Exa.ai, Notion, and AI Agents

## Description
This workflow automates the process of competitor research by leveraging Exa.ai to identify similar companies and then uses multiple AI agents to gather detailed information. It aims to provide comprehensive insights into competitors for marketing research purposes.

## Input Details
The workflow is manually triggered and takes a source company URL as its primary input to initiate the competitor search.

## Process Summary
The workflow begins by setting a source company URL and then utilizes Exa.ai's 'findSimilar' search to identify competitors. Each discovered competitor is then processed individually in a loop. Three dedicated AI agents concurrently gather information: one for company overview (Crunchbase, WellFound, LinkedIn, news), another for product offerings (features, pricing, technology), and a third for summarizing customer reviews from various platforms. Finally, the collected data from all agents is compiled into a single, comprehensive report.

## Output Details
The workflow outputs a detailed competitor research report, which is then formatted and inserted as a new page into a designated Notion database.
