# Workflow Analysis for Product Hunt to Discord Rank Synchronization

## Description
This workflow automates the process of identifying new upvotes on Product Hunt for a specific product and assigning a corresponding role in Discord to the users who upvoted it.

## Input Details
The workflow is manually triggered to identify new Product Hunt upvotes.

## Process Summary
The workflow starts by retrieving new upvotes for a specified Product Hunt product. It then iterates through each upvote, extracting the user's Discord handle if available. For each user with a Discord handle, it finds their Discord user ID. Finally, it assigns a specific "Product Hunt Rank" role to these users in Discord.

## Output Details
The workflow assigns a "Product Hunt Rank" role to relevant users in a specified Discord server.
