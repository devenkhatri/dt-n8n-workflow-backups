# Workflow Analysis for Daily Podcast Summary with AI

## Description
This workflow automatically generates a daily summary of top podcasts for a chosen genre. It fetches popular podcast episodes, transcribes a segment of their audio, uses AI to summarize the transcript, and then compiles this information into an HTML email that is sent to the user.

## Input Details
The workflow is triggered daily at a scheduled time (8 AM) and does not receive external input data upon trigger, but rather initiates data fetching based on internal configuration (podcast genre).

## Process Summary
The workflow starts daily at 8 AM and sets a predefined podcast genre (e.g., TECHNOLOGY). It fetches a list of the top 10 podcast episodes for that genre from the Taddy API and splits them into individual items. For each podcast, it downloads the audio, then sends it to an audio cutter API to crop the audio from 8 minutes to 24 minutes. After confirming the cropped audio is ready, it downloads the cut MP3 and transcribes the audio using OpenAI's Whisper API. Finally, OpenAI's GPT-4o-mini model summarizes the transcribed text, and this data is structured along with podcast details.

## Output Details
The workflow sends an email containing an HTML table with the podcast title, episode name with a link to the audio, and the AI-generated summary for each top podcast episode.
