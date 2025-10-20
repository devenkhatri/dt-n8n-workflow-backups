# Workflow Analysis for Typeform Feedback Router

## Description
This workflow receives feedback from Typeform and routes it to the appropriate channel based on the feedback type.

## Input Details
This workflow is triggered by new Typeform survey submissions via a webhook.

## Process Summary
The workflow starts by receiving data from a Typeform submission. It then determines if the feedback is positive, negative, or a general suggestion by evaluating the "what_can_be_improved" field. Based on this evaluation, the workflow routes the feedback to different paths. If negative, an internal message is prepared. If positive, a success message is prepared. If neutral, it routes to generic flow.

## Output Details
The workflow sends either a success or an internal message based on feedback type, as well as a generic message for general feedback.
