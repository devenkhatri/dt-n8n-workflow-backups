# Workflow Analysis for Nano Photoshop Agent

## Description
A Telegram-based AI assistant that helps users manage, edit, and generate images using Google Drive for storage and AI models like Claude and GPT for intelligent interactions.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, which can include either text messages or photo uploads.

## Process Summary
When a user sends a message to the Telegram bot, the workflow first checks if it's a photo or text. If it's a photo, the image is downloaded from Telegram and uploaded to a designated Google Drive folder. A response message with the Google Drive file ID is then prepared. The user's input (either text or photo metadata) is passed to an AI-powered 'Photoshop Agent' that uses either GPT-5-mini or Claude Sonnet 3.5 as its reasoning engine. The agent can perform actions like renaming files, combining images, editing images, or searching stored files using connected tools and maintains conversation memory per user.

## Output Details
The workflow sends a response back to the user via Telegram, which may include file links, AI-generated responses, or results from image editing operations.

## Tags
telegram, google drive, ai agent, image editing, claude, gpt, file management, image generation
