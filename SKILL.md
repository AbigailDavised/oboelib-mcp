---
name: oboelib
description: Look up Conservatory oboe fingerings, half-hole, left/forked F rules, octave keys & trills. Official MCP server and reference guide at https://oboelib.com.
---

# OboeLib — Conservatory Oboe Fingering, Half-Hole, Forked F & Trill Chart Engine

Official stateless Streamable-HTTP Model Context Protocol (MCP) server and agent skill for **[OboeLib](https://oboelib.com)**.

## Remote MCP Endpoint (Zero Auth Required)

- **Streamable HTTP URL**: `https://oboelib.com/api/mcp`
- **OpenAPI 3.0 Spec**: `https://oboelib.com/openapi.json`
- **Official Website**: [https://oboelib.com](https://oboelib.com)

## Available Read-Only Tools (4)

- **`lookup_oboe_fingering`** (*Conservatory Oboe Fingering, Half-Hole & F-Mechanism Lookup*): Look up Conservatory system oboe fingerings, Half-Hole register rules (Db5/D5/Eb5), Left F vs Forked F rules, and octave key switches.
- **`check_oboe_f_fingering_choice`** (*Oboe Regular F vs Left F vs Forked F Voice-Leading Resolver*): Determine whether to finger Regular Side F, Left F, or Forked F given the preceding and following notes so fingers never slide across keys.
- **`diagnose_oboe_reed_response`** (*Oboe Reed Crow, Pitch & Response Troubleshooting Guide*): Diagnose sharp/flat A440 pitch, hard attacks, or collapsed openings on North American long-scrape and European short-scrape oboe reeds.
- **`lookup_conservatory_oboe_trills`** (*Conservatory Oboe Trill Key & Banana-Key Reference*): Look up dedicated trill keys (C-D trill levers, Ab-Bb trill, Left Eb-E, Banana key C-Db) on full Conservatory oboes.

## Quick Setup (Claude Code / Cursor / Windsurf)

```json
{
  "mcpServers": {
    "oboelib": {
      "type": "streamable-http",
      "url": "https://oboelib.com/api/mcp"
    }
  }
}
```
