# Public 9router-ollama fork

Fork of 9Router with Ollama Cloud API Key Provider + key rotation support.

## Changes

- Added Ollama Cloud as first-class API Key Provider (multi-key rotation via existing APIKEY_PROVIDERS infrastructure)
- Added 6 Ollama model pricing entries (gpt-oss:120b, kimi-k2.5, glm-5, minimax-m2.5, glm-4.7-flash, qwen3.5)
- Added usage reporting for Ollama Cloud in SSE and dashboard fetchers
- Fixed connection.apiKey reference in usage.js after destructuring

## Setup

Copy .env.example to .env and configure your providers.

See README.md for full setup guide.

> **OAuth credentials:** This fork uses placeholder OAuth client IDs/Secrets. Replace YOUR-* placeholders in src/lib/oauth/constants/oauth.js and open-sse/config/providers.js with your own values before using OAuth providers.
