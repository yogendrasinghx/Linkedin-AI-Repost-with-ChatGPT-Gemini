# Privacy Policy

**Last Updated: February 2, 2026**

## Overview

LinkedIn AI Repost with ChatGPT & Gemini ("the Extension") is committed to protecting your privacy. This privacy policy explains how we handle data when you use our Chrome Extension.

## Data Collection

**We do NOT collect, store, or transmit any personal data to our servers.**

The Extension operates entirely locally in your browser and communicates directly with your chosen AI provider (Google Gemini or OpenAI).

## What Data is Stored Locally

The Extension stores the following data in Chrome's encrypted sync storage:

- **API Keys**: Your Google Gemini or OpenAI API key (encrypted by Chrome)
- **Settings**: Your selected AI provider, model preferences, and tone preferences
- **Temporary Prompts**: When using free tier mode, prompts are stored temporarily (5-minute expiry) in Chrome's local storage

All data is stored locally on your device using Chrome's secure storage APIs. We never transmit this data to any server we control.

## Data Transmission to Third Parties

When you use the Extension's AI features, your content and API requests are transmitted directly to:

- **Google Gemini** (if you selected Gemini as your provider)
- **OpenAI** (if you selected OpenAI/ChatGPT as your provider)

These transmissions are governed by the respective privacy policies of these services:
- [Google Privacy Policy](https://policies.google.com/privacy)
- [OpenAI Privacy Policy](https://openai.com/privacy/)

**Important**: We do NOT proxy, log, or store any of this data. The Extension acts as a client that facilitates direct communication between your browser and the AI provider you choose.

## Chrome Permissions

The Extension requests the following permissions:

- **storage**: To save your API keys and settings securely in Chrome's sync storage
- **Host permission (*.linkedin.com)**: To inject the AI writer toolbar on LinkedIn pages

We do not request or use any other permissions.

## Third-Party Services

The Extension integrates with:

1. **Google Gemini API**: Subject to [Google's Terms of Service](https://policies.google.com/terms) and [Generative AI Additional Terms](https://ai.google.dev/gemini-api/terms)
2. **OpenAI API**: Subject to [OpenAI's Terms of Use](https://openai.com/policies/terms-of-use)
3. **LinkedIn**: The Extension operates on LinkedIn.com but is not affiliated with or endorsed by LinkedIn Corporation

You are responsible for complying with the terms of service of these third-party platforms.

## API Key Security

- API keys are stored using Chrome's `chrome.storage.sync` API, which provides encryption at rest
- API keys are never sent to any server we control
- API keys are transmitted only to the respective AI provider (Google or OpenAI) using HTTPS
- You can delete your API keys at any time through the Extension's options page

## User Responsibilities

You are responsible for:
- Securing your API keys and not sharing them with others
- Monitoring your API usage and associated costs with your AI provider
- Reviewing and editing AI-generated content before posting on LinkedIn
- Complying with LinkedIn's Terms of Service and content policies

## Data Retention

- Settings and API keys are stored indefinitely until you remove them or uninstall the Extension
- Temporary prompts (free tier mode) expire after 5 minutes
- Uninstalling the Extension removes all locally stored data

## GDPR and CCPA Compliance

Since we do NOT collect or process personal data:
- There is no data to request, export, or delete from our servers
- All data resides locally in your browser
- You have full control over your data through Chrome's extension settings

## Children's Privacy

The Extension is not intended for use by children under 13. We do not knowingly collect data from children.

## Changes to This Policy

We may update this privacy policy from time to time. The "Last Updated" date at the top indicates when changes were made. Continued use of the Extension after changes constitutes acceptance of the updated policy.

## Contact

For questions or concerns about this privacy policy:
- **Developer**: [https://yogendrasingh.in](https://yogendrasingh.in)

## Disclaimer

This Extension is provided "AS IS" without warranties. We are not affiliated with LinkedIn Corporation, Google LLC, or OpenAI. Use of this Extension is at your own risk.
