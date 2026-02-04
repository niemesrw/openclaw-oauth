# OpenClaw Google OAuth

Community OAuth app for the [OpenClaw](https://github.com/openclaw/openclaw) Google Workspace skill.

## What This Is

This repository hosts the OAuth app identity that allows OpenClaw users to connect their Gmail and Google Calendar without needing to set up their own Google Cloud project.

## How It Works

1. You install the `google-workspace` skill
2. You run `python skill.py auth` which opens Google's OAuth consent
3. You authorize access to your Gmail/Calendar
4. Tokens are stored **locally on your machine only**
5. All API calls go **directly from your machine to Google**

**No data passes through any intermediary servers.**

## Credentials

Download `credentials.json` from this repo and place it in your skill directory:

```bash
curl -o credentials.json https://raw.githubusercontent.com/niemesrw/openclaw-oauth/main/credentials.json
```

## Privacy & Terms

- [Privacy Policy](PRIVACY.md)
- [Terms of Service](TERMS.md)

## Revoking Access

You can revoke access at any time: https://myaccount.google.com/permissions

## Questions?

- [OpenClaw GitHub Issues](https://github.com/openclaw/openclaw/issues)
- [OpenClaw Discord](https://discord.com/invite/clawd)
