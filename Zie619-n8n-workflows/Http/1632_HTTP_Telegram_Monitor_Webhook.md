# Workflow Analysis for Telegram Tron Wallet Blacklist Checker

## Description
This n8n workflow template allows users to check if a Tron wallet address is blacklisted on the USDT contract via a Telegram bot. When a user sends the command {walletAddress} through the Telegram bot, the workflow queries the Tronscan API to determine if the provided wallet address is blacklisted. The result is then sent back to the user via the Telegram bot.

## Input Details
This workflow is triggered by messages received from a Telegram bot, specifically when a user sends a wallet address.

## Process Summary
The workflow starts by receiving a message from Telegram. It then checks if the received message contains a valid Tron wallet address format. If the format is correct, it makes an HTTP request to a Tron blacklist API. After receiving the API response, a code node processes the response to determine if the wallet is blacklisted. If the wallet address format is incorrect, a custom error message is generated. Finally, the workflow sends a message back to the Telegram user with the result or an error.

## Output Details
The workflow sends a Telegram message back to the user, indicating whether the provided Tron wallet address is blacklisted or if the address format was invalid.

## Tags
automation,n8n,production-ready,excellent,optimized
