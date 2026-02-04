# Privacy Policy

**OpenClaw Google Workspace Integration**

Last updated: February 3, 2026

## What This Integration Does

The OpenClaw Google Workspace skill allows you to access your Gmail and Google Calendar directly from your local machine using the official Google APIs.

## Data Collection

**We do not collect, store, or process any of your data.**

- All authentication tokens are stored locally on your machine
- All API requests go directly from your machine to Google's servers
- No data passes through OpenClaw servers
- No telemetry or analytics are collected

## How It Works

1. You authenticate directly with Google using OAuth 2.0 with PKCE
2. Google issues a token that is stored on your local machine only
3. When you use the skill, your machine communicates directly with Google
4. OpenClaw acts only as the "app identity" for the OAuth flow

## Security: OAuth 2.0 with PKCE

We use **PKCE (Proof Key for Code Exchange)** for all OAuth flows. This is the modern security standard for desktop/public clients:

- A cryptographic `code_verifier` is generated locally on your machine
- This verifier never leaves your machine and is never shared
- Even if someone intercepts the authorization code, they cannot exchange it for tokens without your local verifier
- The `client_secret` becomes non-critical for security - PKCE provides the actual protection

## Data Access

The integration requests access to:

- **Gmail**: Read, send, and manage your emails
- **Calendar**: Read and create calendar events

You can revoke access at any time at: https://myaccount.google.com/permissions

## Your Rights

- You control all data on your machine
- You can delete stored tokens at any time
- You can revoke OAuth access at any time via Google
- No data is shared with third parties

## Open Source

This integration is fully open source. You can review exactly what it does:
https://github.com/openclaw/openclaw

## Contact

For questions about this privacy policy:
- GitHub: https://github.com/openclaw/openclaw/issues
- Discord: https://discord.com/invite/clawd

## Changes

We may update this policy occasionally. Changes will be posted to this repository.
