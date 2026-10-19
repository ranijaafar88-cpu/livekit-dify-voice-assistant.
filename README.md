LiveKit + Dify Voice Assistant

A voice assistant built with LiveKit and Dify, using Retrieval-Augmented Generation (RAG) to answer questions from a knowledge base.

Project Overview

This project connects a LiveKit voice assistant to a Dify knowledge base through an HTTP retrieval action. During development, I tested different integration approaches, troubleshot API errors, and corrected a dataset ID mismatch.

Architecture

1. User: Asks a question through the voice interface.
2. LiveKit: Manages the voice assistant interaction.
3. Dify API: Receives the question and retrieves relevant knowledge.
4. Response: The retrieved information supports the assistant’s answer.

Repository Contents

* livekit_dify_voice_assistant_journey_updated.pdf — Project report and troubleshooting journey.
* setup-guide.md — Integration configuration and troubleshooting instructions.
* RAG VOICE ASSISTANT... — Project-related configuration or documentation file.
* AI_Agents_Harnesses... — Supporting research document.

Technologies

* LiveKit
* Dify
* HTTP API
* Retrieval-Augmented Generation (RAG)

Security

API keys, access tokens, and other credentials must be stored securely and must never be committed to this repository.

Status

The LiveKit-to-Dify knowledge retrieval integration was tested successfully after correcting the dataset ID.
