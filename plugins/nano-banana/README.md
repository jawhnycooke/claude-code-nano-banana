# Nano Banana Plugin

Interactive JSON Prompt Translator for Nano Banana Pro (Gemini 3 Pro Image).

## Description

This plugin provides the `/nano-banana` slash command that helps you convert natural language descriptions into structured JSON schemas for precision image generation with Nano Banana Pro.

Instead of vague prompts, you get precise specifications where every element—lighting, camera angle, composition, props—lives on its own "dial." Change one thing without affecting everything else.

## Features

**Supported schema types:**
- **Marketing Images** - Product shots, hero images, brand photography
- **UI/UX Mockups** - App screens, dashboards, websites
- **Diagrams** - Flowcharts, architecture diagrams, process maps
- **Data Visualizations** - Charts, graphs with accurate data
- **Social Graphics** - Platform-specific social media content

## Usage

Invoke the command with a rough description:

```bash
/nano-banana vinyl record product shot, moody lighting, vintage feel
```

The translator will:
1. Ask clarifying questions using structured choices
2. Guide you through thinking about your visual
3. Generate a complete JSON specification
4. Provide instructions for using it with Nano Banana Pro

## Example Workflow

```bash
/nano-banana product shot for a lime seltzer can
```

The plugin will ask about:
- Camera angle (front, three-quarter, overhead, etc.)
- Lighting style (dramatic, soft, backlit, natural)
- Background treatment (solid, gradient, bokeh, environment)
- Props and composition details

Then output a complete JSON like:

```json
{
  "marketing_image": {
    "subject": { ... },
    "camera": { "angle": "three_quarter_front", ... },
    "lighting": { "key_light_direction": "right", ... },
    ...
  }
}
```

Ready to paste into Nano Banana Pro for rendering.

## Tutorial

See the full tutorial: [Dials, Not Dice: A Precision Prompting Guide for Nano Banana Pro](https://jawhnycooke.ai/blog/precision-prompting-nano-banana-pro-with-claude-code)

## Author

Jawhny Cooke
Contact: plugins@jawhnycooke.ai

## Version

1.0.0
