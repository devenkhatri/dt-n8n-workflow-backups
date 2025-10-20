# Workflow Analysis for Stoic Quote Twitter Bot

## Description
This workflow automates the posting of stoic philosophy quotes to Twitter, leveraging AI to generate the quotes.

## Input Details
The workflow is triggered manually and takes no specific input data.

## Process Summary
First, the workflow generates a stoic philosophy quote using OpenAI. It then reformats the response from OpenAI. Next, it checks to see if the generated tweet could be considered a "bad tweet" by searching for specific phrases. If it is not a bad tweet, it shortens the tweet and removes newlines, then finally posts the tweet to Twitter.

## Output Details
The workflow posts a stoic philosophy quote to Twitter.
