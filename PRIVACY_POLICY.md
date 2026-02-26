# Privacy Policy

**Last Updated: February 25, 2026**

## Overview

Quillzy ("the Extension") is committed to protecting your privacy. This privacy policy explains how we handle data when you use our Chrome Extension.

## Data Collection

**We do NOT collect, store, or transmit any personal data to our servers.**

The Extension operates entirely locally in your browser and communicates directly with your chosen AI provider (Browser AI on-device, Google Gemini, or OpenAI).

## What Data is Stored Locally

The Extension stores the following data in Chrome's secure storage:

- **API Keys**: Your Google Gemini or OpenAI API key (stored in Chrome's encrypted sync storage)
- **Settings**: Your selected AI provider, model preferences, tone preferences, custom prompts, and max word count
- **Browser AI State**: Download progress and availability status for the on-device AI model (stored in Chrome's local storage)
- **Temporary Prompts**: When using free tier mode, prompts are stored temporarily (5-minute expiry) in Chrome's local storage

All data is stored locally on your device using Chrome's secure storage APIs. We never transmit this data to any server we control.

## What Data is Processed Locally

When you use the Extension's features, the following data is read from LinkedIn pages and processed locally in your browser:

- **Post Content**: Text and author name from LinkedIn posts (for repost and comment modes)
- **Post Images**: Image URLs from LinkedIn posts (fetched for image-aware AI commentary)
- **Comment Context**: Text of the post being commented on
- **DM Context**: The last 2-3 messages in a LinkedIn conversation (sender names and message text, for DM reply mode)
- **Connection Note Context**: Recipient name and profile information from LinkedIn profile pages (for connection note mode)
- **Editor Content**: Text you type in LinkedIn editors (for new post and draft-aware modes)

This data is processed locally and sent only to your chosen AI provider for content generation. It is never stored persistently or sent to any server we control.

## Data Transmission to Third Parties

When you use the Extension's AI features, your content and AI requests are transmitted directly to:

- **Browser AI (Gemini Nano)**: Processed entirely on your device. No data is transmitted anywhere.
- **Google Gemini** (if selected as your provider): Text content and post images sent via Google's Generative Language API
- **OpenAI** (if selected as your provider): Text content and post images sent via OpenAI's Chat Completions API

These transmissions are governed by the respective privacy policies of these services:
- [Google Privacy Policy](https://policies.google.com/privacy)
- [OpenAI Privacy Policy](https://openai.com/privacy/)

**Important**: We do NOT proxy, log, or store any of this data. The Extension acts as a client that facilitates direct communication between your browser and the AI provider you choose.

## Browser AI (On-Device Processing)

When using Browser AI mode:
- All AI processing happens entirely on your device using Chrome's built-in Writer API (Gemini Nano)
- No data leaves your browser
- No API key is required
- No network requests are made for AI generation
- The AI model is downloaded once from Google's servers and runs locally

## Image Processing

When a LinkedIn post contains images:
- Image URLs are extracted from the page DOM
- Images are fetched from `media.licdn.com` (LinkedIn's CDN) by the extension's background script
- Images are resized locally (max 1024px) and compressed to JPEG
- Processed images are sent to your chosen cloud AI provider (Gemini or OpenAI) for visual context
- Browser AI mode does not support image input; a text-only fallback is used
- Images are never stored persistently by the Extension

## Chrome Permissions

The Extension requests the following permissions:

- **storage**: To save your API keys, settings, and Browser AI download state securely in Chrome's storage
- **Host permission (www.linkedin.com)**: To inject the Quillzy AI toolbar on LinkedIn posts, comments, DM editors, and connection note modals
- **Host permission (media.licdn.com)**: To fetch post images for image-aware AI commentary
- **Host permission (chatgpt.com, chat.openai.com)**: To auto-fill prompts on ChatGPT web for free tier mode
- **Host permission (claude.ai)**: To auto-fill prompts on Claude web for free tier mode
- **Host permission (gemini.google.com)**: To auto-fill prompts on Gemini web for free tier mode

## Third-Party Services

The Extension integrates with:

1. **Chrome Writer API (Gemini Nano)**: On-device AI model provided by Chrome. Subject to [Chrome's Terms of Service](https://www.google.com/chrome/terms/)
2. **Google Gemini API**: Subject to [Google's Terms of Service](https://policies.google.com/terms) and [Generative AI Additional Terms](https://ai.google.dev/gemini-api/terms)
3. **OpenAI API**: Subject to [OpenAI's Terms of Use](https://openai.com/policies/terms-of-use)
4. **LinkedIn**: The Extension operates on LinkedIn.com but is not affiliated with or endorsed by LinkedIn Corporation

You are responsible for complying with the terms of service of these third-party platforms.

## API Key Security

- API keys are stored using Chrome's `chrome.storage.sync` API, which provides encryption at rest
- API keys are never sent to any server we control
- API keys are transmitted only to the respective AI provider (Google or OpenAI) using HTTPS
- Gemini API keys are sent via `x-goog-api-key` HTTP header (not in URL parameters)
- You can delete your API keys at any time through the Extension's options page

## User Responsibilities

You are responsible for:
- Securing your API keys and not sharing them with others
- Monitoring your API usage and associated costs with your AI provider
- Reviewing and editing AI-generated content before posting on LinkedIn
- Complying with LinkedIn's Terms of Service and content policies

## Data Retention

- Settings and API keys are stored indefinitely until you remove them or uninstall the Extension
- Browser AI download state is stored in Chrome's local storage until cleared
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
