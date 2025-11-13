# Workflow Analysis for Chinese Vocabulary Flashcard Generator

## Description
This workflow automatically creates language learning flashcards by translating English words into Chinese, generating pinyin pronunciation and example sentences using AI, fetching relevant images from Pexels, and updating a Google Sheet with all the flashcard data.

## Input Details
The workflow is triggered when a new row with an English word is added to a specific Google Sheet.

## Process Summary
When a new English word is added to the Google Sheet, the workflow first checks if the input is not empty. It then translates the word to Chinese using Google Translate. An AI agent (simulated via prompt) generates the pinyin and a simple example sentence in Chinese. Simultaneously, the workflow fetches a relevant image from Pexels based on the English word and uploads it to Google Drive. Finally, all data—including original word, translation, pinyin, example sentence, image filename, and image link—are merged and written back to the Google Sheet.

## Output Details
The workflow updates the original Google Sheet row with Chinese translation, pinyin, example sentence, image filename, and image link for flashcard creation.

## Tags
language learning, flashcards, Google Sheets, Google Translate, AI agent, Pexels, Google Drive, Chinese, pinyin, automation
