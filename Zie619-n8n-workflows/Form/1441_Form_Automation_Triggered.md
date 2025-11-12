# Workflow Analysis for Image to license plate number

## Description
This workflow extracts the license plate number from a vehicle in an uploaded image using an AI language model with vision capabilities, and returns the result on a completion page.

## Input Details
The workflow is triggered by a web form where a user uploads an image file (JPEG or PNG) containing a vehicle.

## Process Summary
The workflow starts with a form trigger that accepts an image upload. It then sets the AI model to use (GPT-4o) and defines a prompt instructing the model to extract only the license plate number from the front-most car in the image. The image and prompt are passed to an OpenRouter-powered LLM capable of processing image inputs. The extracted license plate text is then displayed on a completion page shown to the user.

## Output Details
The workflow displays the extracted license plate number on a web page as a completion message after form submission.

## Tags
automation, n8n, production-ready, excellent, optimized, license plate recognition, image analysis, AI, LLM, form processing
