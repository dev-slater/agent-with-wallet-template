# agent with wallet template

## What this is

A pre-configured [OpenClaw](https://github.com/openclaw/openclaw) agent template with a Tempo wallet. Deploy it on Pinata's agent marketplace and get an agent that can discover, compare, and pay for any service in the Tempo MPP directory — 100+ services at launch, including web search, AI image generation, data enrichment, and more.

## Post-deploy setup

After deploying, do three things:

1. **Fetch the Tempo skill**
   ```
   bash setup.sh
   ```
   This pulls the latest Tempo skill from [tempo.xyz/SKILL.md](https://tempo.xyz/SKILL.md).

2. **Create a wallet for this agent**
   ```
   "$HOME/.tempo/bin/tempo" wallet create
   ```
   This generates a fresh Tempo wallet for this agent instance. Each deployed agent gets its own wallet. The agent will prompt you to back up the private key to Pinata's secret vault — do this so the wallet survives restarts.

3. **Fund the agent's wallet**
   Send funds to the wallet address shown after creation, or visit [wallet.tempo.xyz](https://wallet.tempo.xyz). The agent will notify you when it needs a top-up.

## Usage

Just talk to the agent. It will search the Tempo services directory, compare options, and execute purchases on your behalf (with confirmation for anything over 1 usd).

**Example prompts:**
- "Find me the cheapest web search API and search for 'best noise cancelling headphones 2026'"
- "What AI image generation services are available and how much do they cost?"
- "Summarize this URL using Parallel's extract API"
