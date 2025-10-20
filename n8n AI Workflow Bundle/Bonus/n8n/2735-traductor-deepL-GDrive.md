# Workflow Analysis for DeepL Translator for Google Drive Files

## Description
This workflow automates the translation of documents uploaded to a specific Google Drive folder using DeepL, then saves the translated document to another designated Google Drive folder.

## Input Details
The workflow is triggered manually and requires the user to specify the file ID of the document they wish to translate from a Google Drive folder.

## Process Summary
The workflow starts by retrieving the content of the specified Google Drive file. It then extracts the file name and sends the document content to DeepL for translation into English. After translation, the workflow uploads the translated document to a designated "traduccion" (translation) folder in Google Drive, renaming it to include "(EN)" before its original extension. Finally, it deletes the original file from the source folder to complete the process.

## Output Details
The workflow produces a translated document in English, which is saved to a specific "traduccion" folder in Google Drive.
