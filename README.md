# Nano Banana Pro JSON Prompt Translator

Stop rolling dice. Start turning dials.

This repository contains a Claude Code slash command that translates natural language descriptions into structured JSON schemas for [Nano Banana Pro](https://blog.google/technology/google-labs/gemini-image-generation-updates/) (Gemini 3 Pro Image).

## What It Does

Instead of writing vague prompts and hoping for the best, the translator helps you build precise specifications where every element - lighting, camera angle, composition, props - lives on its own "fader." Change one thing without affecting everything else.

**Supported schema types:**
- **Marketing Images** - Product shots, hero images, brand photography
- **UI/UX Mockups** - App screens, dashboards, websites
- **Diagrams** - Flowcharts, architecture diagrams, process maps
- **Data Visualizations** - Charts, graphs with accurate data
- **Social Graphics** - Platform-specific social media content

## Installation

### From GitHub (Recommended)

First, add the marketplace to Claude Code:

```bash
/plugin marketplace add https://github.com/jawhnycooke/claude-code-nano-banana
```

Then install the plugin:

```bash
/plugin
```
Follow these steps:
1. Select `1. Browse and install plugins`
2. Select marketplace `claude-code-nano-banana`
3. Press the `Space bar` to select `nano-banana`
4. Press `i` to install
5. `/exit` Claude code and restart

This installs the plugin directly from this repository.

## Usage

Invoke the command with a rough description:

```
/nano-banana vinyl record product shot, moody lighting, vintage feel
```

The translator will ask clarifying questions, then output a complete JSON specification ready to paste into Nano Banana Pro.

## Tutorial

See the full tutorial: [Dials, Not Dice: A Precision Prompting Guide for Nano Banana Pro and Claude Code](https://jawhnycooke.ai/blog/precision-prompting-nano-banana-pro-with-claude-code)

The `examples/vinyl-record-tutorial/` folder contains the JSON files from the tutorial so you can follow along.

## Contact

For questions, issues, or contributions, contact: plugins@jawhnycooke.ai

## License

MIT
