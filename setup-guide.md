LiveKit + Dify Voice Assistant — Setup Guide

Overview

This project connects a LiveKit voice assistant to a Dify knowledge base using an HTTP retrieval action. The assistant retrieves relevant information from the knowledge base to answer user questions.

Architecture

1. User asks a question through the voice assistant.
2. LiveKit handles the voice interaction.
3. The ask_dify HTTP action sends the question to Dify.
4. Dify searches the configured knowledge base.
5. The retrieved information is used to formulate the answer.

Dify Retrieval Configuration

* Method: POST
* Endpoint: https://api.dify.ai/v1/datasets/4cf1e0c7-c870-4dd3-94fc-fcbe7f426a40/retrieve
* Required parameter: query (string)
* Authorization: Use a valid Dify dataset API key in the HTTP Authorization header: Bearer YOUR_DIFY_API_KEY

Security: Never commit real API keys, access tokens, or secrets to GitHub.

Troubleshooting

* 403 Forbidden: Verify that the API key is authorized to access the selected knowledge base.
* 404 Not Found: Check the endpoint and dataset ID.
* 400 Bad Request: Verify the request body and required query field. If the error mentions model credentials, check the relevant model configuration separately.
* Incorrect retrieval: Confirm that the correct knowledge base is being queried and test capitalization or spelling variations.

Project Report

See livekit_dify_voice_assistant_journey_updated.pdf for the development journey, errors encountered, and final fix.

Demo

The repository includes a screen recording demonstrating the project setup.
