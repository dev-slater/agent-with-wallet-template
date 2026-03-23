# tempo-buyer-template

## What this is

A pre-configured [OpenClaw](https://openclaw.dev) agent template with a Tempo wallet. Deploy it on Pinata's agent marketplace and get an agent that can discover, compare, and pay for any service in the Tempo MPP directory — 100+ services at launch, including web search, AI image generation, data enrichment, and more.

## Post-deploy setup

After deploying, do two things:

1. **Log in to your Tempo wallet**
   ```
   tempo wallet login
   ```
   This opens a browser window for passkey authentication.

2. **Fund your wallet**
   ```
   tempo wallet fund
   ```
   Or visit [wallet.tempo.xyz](https://wallet.tempo.xyz) to deposit funds via the dashboard.

## Usage

Just talk to the agent. It will search the Tempo services directory, compare options, and execute purchases on your behalf (with confirmation for anything over 1 usd).

**Example prompts:**
- "Find me the cheapest web search API and search for 'best noise cancelling headphones 2026'"
- "What AI image generation services are available and how much do they cost?"
- "Summarize this URL using Parallel's extract API"
