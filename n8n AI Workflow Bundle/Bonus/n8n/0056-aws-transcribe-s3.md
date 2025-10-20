# Workflow Analysis for AWS S3 to Transcribe Workflow

## Description
This workflow automates the transcription of audio files uploaded to an AWS S3 bucket using AWS Transcribe, then stores the transcriptions back into S3.

## Input Details
The workflow is manually triggered. It can also be triggered by a new file added to S3.

## Process Summary
The workflow starts by retrieving parameters defining the source S3 bucket, output S3 bucket, folder, and various transcription job settings. It then retrieves a list of media files from the specified source S3 bucket folder. It iterates through each file, starts a transcription job using AWS Transcribe, and waits for the job to complete. Once completed, it fetches the transcription result. Finally, it saves the transcription result (JSON) to the specified output S3 bucket.

## Output Details
The workflow outputs JSON transcription files, storing them in a designated AWS S3 bucket.
