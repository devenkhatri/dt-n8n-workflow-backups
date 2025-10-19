# Workflow Analysis for AI Newsletter Generator

## Description
This workflow automates the creation of an AI newsletter using articles sourced from a specified RSS feed, summarized by AI, and then compiled into a polished newsletter draft that is ultimately sent via email.

## Input Details
The workflow is triggered manually or on a preset schedule, initiating the content generation process.

## Process Summary
The workflow starts by fetching articles from an RSS feed. Each article's content is then extracted and cleaned. A large language model (LLM) summarizes each article, extracting key insights. These summaries are then compiled and structured into a newsletter draft. Finally, another LLM is used to refine the draft, ensuring it is ready for distribution.

## Output Details
The workflow outputs a drafted newsletter, which is then sent as an email via Gmail.
