# Krasnoperov Claude Plugins Marketplace

Custom marketplace for Claude Code plugins by krasnoperov.

## Installing Plugins

### Step 1: Add Marketplace

```bash
/plugin marketplace add krasnoperov/claude-plugins
```

### Step 2: Install Plugin

```bash
/plugin install gemini-images@krasnoperov-plugins
/plugin install transcribe@krasnoperov-plugins
```

Or browse available plugins:

```bash
/plugin
```

## Available Plugins

### gemini-images

Consistent image generation with Gemini - Create 2D game sprites, characters, and environments with visual consistency using reference sheets methodology.

**Core primitives:** `generate`, `edit`, `compose` - three operations that compose into any workflow.

**Repository:** https://github.com/krasnoperov/gemini-images

### transcribe

Audio/video transcription with speaker diarization, AI summarization, and infographic generation.

**Core operations:** `transcribe`, `summarize`, `infographic`, `process` - transform recordings into transcripts, summaries, and visuals.

**Repository:** https://github.com/krasnoperov/transcribe
