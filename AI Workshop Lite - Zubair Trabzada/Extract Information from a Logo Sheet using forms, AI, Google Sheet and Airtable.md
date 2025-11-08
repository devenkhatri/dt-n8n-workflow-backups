# Workflow Analysis for AI Logo Sheet Extractor to Airtable

## Description
This automation allows users to upload an image of a logo sheet containing multiple product logos. An AI agent with vision capabilities then analyzes the image, extracting product names, their attributes, and identifying similar tools from the context. The extracted information is then systematically organized and stored in a structured Airtable database, ensuring that both new attributes and tools are created or updated efficiently.

## Input Details
The workflow is triggered by a form submission, receiving an image of a logo sheet and an optional additional text prompt.

## Process Summary
First, an AI agent (GPT-4o) processes the submitted image and prompt, extracting a structured list of tools, their attributes, and similar tools. Next, the extracted attributes are individually processed, where each unique attribute is upserted (created or updated) in the Airtable "Attributes" table, and their record IDs are retrieved. Subsequently, each identified tool is upserted into the Airtable "Tools" table using a generated hash for identification, and existing attributes for that tool are retrieved. Then, similar tools for each main tool are processed, ensuring they also exist in the "Tools" table and their record IDs are obtained. Finally, the main tool record is updated in Airtable, linking it to the appropriate attribute and similar tool record IDs.

## Output Details
The workflow populates and updates two Airtable tables: "Tools" (with tool names, attributes, and similar tools) and "Attributes" (with attribute names and linked tools).
