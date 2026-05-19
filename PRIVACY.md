# Privacy Policy

This document describes how the OrcaRouter plugin for Dify handles user data.

## 1. Plugin Data Handling

The OrcaRouter plugin is a thin client for the OrcaRouter API
(https://api.orcarouter.ai/v1). It does not collect, store, log, or transmit
any personal data on its own. All data sent through the plugin is forwarded
directly to the OrcaRouter service:

- Your **API key**, sent as `Authorization: Bearer` header on every request
- The **prompts, messages, and parameters** you submit through Dify
- The **input text** for embedding and text-to-speech endpoints
- Optional **routing preferences** (orcarouter_fallback_models, orcarouter_route)

No telemetry, analytics, or third-party data sharing happens in the plugin code.

## 2. OrcaRouter Service Data Handling

OrcaRouter's own data handling (request logging, billing data retention,
upstream provider routing, etc.) is governed by the OrcaRouter Privacy Policy:

**https://www.orcarouter.ai/privacy.html**

Please review that policy to understand how OrcaRouter handles your requests
and any personal information you provide directly to OrcaRouter (account
registration, billing, API key management).

## 3. Upstream Provider Routing

When you use the plugin, your requests are routed to the upstream LLM provider
selected by OrcaRouter (OpenAI, Anthropic, Google, DeepSeek, etc.) according to
your configured routing strategy. The upstream provider's own privacy policy
applies to that portion of the request.

## 4. Local Configuration

API keys and endpoint URLs you enter in Dify's Model Provider settings are
stored by Dify in your Dify deployment. The plugin does not transmit these
credentials anywhere other than to the OrcaRouter API endpoint you configured.

## 5. Data Retention

The plugin retains no data. Any retention happens at:
- The Dify side (your configured credentials)
- The OrcaRouter side (per their privacy policy)
- The upstream provider side (per their privacy policy)

## 6. Changes to This Policy

This privacy policy may be updated when the plugin's data handling changes.
The current version ships with each plugin release and can be reviewed in the
plugin source repository:

**https://github.com/Continuum-AI-Corp/dify-plugin-orcarouter**

## 7. Contact

For privacy questions about the plugin or the OrcaRouter service, contact
OrcaRouter via the channels listed on https://www.orcarouter.ai or open an
issue on the source repository.
