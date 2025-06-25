# BBEdit Chat API Configuration Files

This repository contains JSON configuration files for connecting BBEdit AI Worksheets to various AI models and services.

## Purpose

BBEdit 15.1+ includes an AI Worksheet feature that can connect to different AI services. These configuration files make it easy to set up connections to:

1. **Claude Extra** - Anthropic's high-performance language models
2. **Grok AI** - xAI's text and vision models including web search
3. **Ollama** - Locally-run open source language models
4. **Venice AI** - Privacy focused large language models

## How to Use These Files

1. In BBEdit, choose "Application Support" from the Folders submenu of the BBEdit application menu
2. Create a new folder named "Chat API Descriptions" if it doesn't exist already
3. Copy the JSON files from this repository into that folder
4. Restart BBEdit or create a new AI worksheet to see the new AI models

## Configuration Files

### claude-extra.json
- Configures multiple Claude models from Anthropic including:
  - claude-3-7-sonnet-20250219 (Claude 3.7 Sonnet)
  - claude-sonnet-4-20250514 (Claude Sonnet 4)
  - claude-opus-4-20250514 (Claude Opus 4)
- Requires an API key from Anthropic (https://console.anthropic.com/)
- Sets optimal parameters including max_tokens and the correct API version

### grok-models.json (have not gotten this one to work yet)
- Configures xAI's Grok models including:
  - grok-2-1212 (text)
  - grok-2-vision-1212 (image understanding)
  - grok-3-beta (latest flagship model)
  - grok-3-mini-beta (smaller Grok 3 variant)
  - grok-3-fast-beta (optimized for speed)
  - grok-3-mini-fast-beta (small and fast variant)
- Requires an API key from xAI (https://console.xai.com/)

### ollama-models.json
- Configures connection to locally-running Ollama models
- Includes configurations for:
  - gemma3:27b
  - llama3.2:latest
  - deepseek-r1:latest
  - devstral
- No API key required, but you need to have Ollama installed and running with these models

### grok-models.json (have not gotten this one to work yet)
- Configures xAI's Grok models including:
  - venice-uncensored (text)
  - qwen-2.5-qwq-32b
  - qwen3-4b
  - mistral-31-24b
  - qwen3-235b
  - llama-3.2-3b
  - llama-3.3-70b
  - llama-3.1-405b
  - dolphin-2.9.2-qwen2-72b
  - qwen-2.5-vl
  - qwen-2.5-coder-32b
  - deepseek-r1-671b
  - deepseek-coder-v2-lite
- Requires an API key from xAI (https://venice.ai/settings/api)

## Requirements

- BBEdit 15.5.1 or later
- API keys for Claude, Venice Grok (if using those services)
- Ollama installed locally (if using Ollama models)

## Notes

- API keys need to be entered in BBEdit's settings for each service
- For Ollama, ensure the server is running at http://localhost:11434
- Changes to these files take effect the next time you create a new AI worksheet

## Adding More Models

You can modify these files or create new ones following the same structure to add support for additional AI models and services.
