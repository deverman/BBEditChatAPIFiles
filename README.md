# BBEdit Chat API Configuration Files

This repository contains JSON configuration files for connecting BBEdit AI Worksheets to various AI models and services.

## Purpose

BBEdit 15.1+ includes an AI Worksheet feature that can connect to different AI services. These configuration files make it easy to set up connections to:

1. **Claude 3.7 Sonnet** - Anthropic's high-performance language model
2. **Grok AI** - xAI's text and vision models
3. **Ollama** - Locally-run open source language models

## How to Use These Files

1. In BBEdit, choose "Application Support" from the Folders submenu of the BBEdit application menu
2. Create a new folder named "Chat API Descriptions" if it doesn't exist already
3. Copy the JSON files from this repository into that folder
4. Restart BBEdit or create a new AI worksheet to see the new AI models

## Configuration Files

### claude-3-7-sonnet.json
- Configures the Claude 3.7 Sonnet model from Anthropic
- Requires an API key from Anthropic (https://console.anthropic.com/)
- Sets optimal parameters including max_tokens and the correct API version

### grok-models.json (have not gotten this one to work yet)
- Configures xAI's Grok models including:
  - grok-2-1212 (text)
  - grok-2-vision-1212 (image understanding)
- Requires an API key from xAI (https://console.xai.com/)

### ollama-models.json
- Configures connection to locally-running Ollama models
- Includes configurations for:
  - gemma3:27b
  - llama3.2:latest
  - deepseek-r1:latest
- No API key required, but you need to have Ollama installed and running with these models

## Requirements

- BBEdit 15.1 or later
- API keys for Claude and Grok (if using those services)
- Ollama installed locally (if using Ollama models)

## Notes

- API keys need to be entered in BBEdit's settings for each service
- For Ollama, ensure the server is running at http://localhost:11434
- Changes to these files take effect the next time you create a new AI worksheet

## Adding More Models

You can modify these files or create new ones following the same structure to add support for additional AI models and services.
