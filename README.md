# Krasnoperov Claude Plugins Marketplace

Custom marketplace for Claude Code plugins by krasnoperov.

## For Users: Installing Plugins

### Step 1: Add Marketplace

```bash
/plugin marketplace add krasnoperov/claude-plugins
```

### Step 2: Install Plugin

```bash
/plugin install gemini-images@krasnoperov-plugins
```

Or browse available plugins:

```bash
/plugin
```

## Available Plugins

### gemini-images

Consistent image generation with Nano Banana Pro.

**Core primitives:** `generate`, `edit`, `compose` - three operations that compose into any workflow.

**Key feature:** Reference sheets methodology for consistent characters across multiple generations.

**Repository:** https://github.com/krasnoperov/gemini-images

## Setting Up This Marketplace

### For Plugin Developers

To set up this marketplace for your own organization:

1. **Create marketplace repository** at `https://github.com/krasnoperov/claude-plugins`:
   ```bash
   mkdir claude-plugins
   cd claude-plugins
   mkdir .claude-plugin
   ```

2. **Copy marketplace.json**:
   ```bash
   cp marketplace.json .claude-plugin/marketplace.json
   ```

3. **Commit and push**:
   ```bash
   git init
   git add .
   git commit -m "Initial marketplace setup"
   git remote add origin https://github.com/krasnoperov/claude-plugins.git
   git push -u origin main
   ```

### Directory Structure

The marketplace repository should have this structure:

```
claude-plugins/
├── .claude-plugin/
│   └── marketplace.json     # Required: marketplace catalog
└── README.md               # This file
```

### Adding New Plugins

Edit `.claude-plugin/marketplace.json` and add entries to the `plugins` array:

```json
{
  "name": "plugin-name",
  "source": "krasnoperov/plugin-repo-name",
  "description": "Plugin description",
  "version": "1.0.0",
  "author": {
    "name": "krasnoperov"
  }
}
```

## Documentation

- [Claude Code Plugin Documentation](https://code.claude.com/docs/en/plugins)
- [Claude Code Marketplace Documentation](https://code.claude.com/docs/en/plugin-marketplaces)
