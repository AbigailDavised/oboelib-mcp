# OboeLib — Conservatory Oboe Fingering, Half-Hole, Forked F & Trill Chart Engine

[![Official Website](https://img.shields.io/badge/Website-oboelib.com-blue)](https://oboelib.com)
[![MCP Registry](https://img.shields.io/badge/MCP_Registry-com.oboelib%2Fmcp-green)](https://www.mcptry.com/servers/com.oboelib/mcp)
[![Glama Connector](https://img.shields.io/badge/Glama-Connector-purple)](https://glama.ai/mcp/connectors/com.oboelib/mcp)

Look up Conservatory oboe fingerings, half-hole, left/forked F rules, octave keys & trills.

- **Official Workbench**: [https://oboelib.com](https://oboelib.com)
- **Remote MCP Endpoint**: `https://oboelib.com/api/mcp` (`streamable-http`, read-only, no API key required)
- **Public OpenAPI 3.0**: [https://oboelib.com/openapi.json](https://oboelib.com/openapi.json)
- **LLM Context**: [https://oboelib.com/llms.txt](https://oboelib.com/llms.txt) · [https://oboelib.com/llms-full.txt](https://oboelib.com/llms-full.txt)

## Tools Provided (4 Read-Only Tools)

| Tool Name | Summary |
| :--- | :--- |
| `lookup_oboe_fingering` | Look up Conservatory system oboe fingerings, Half-Hole register rules (Db5/D5/Eb5), Left F vs Forked F rules, and octave key switches. |
| `check_oboe_f_fingering_choice` | Determine whether to finger Regular Side F, Left F, or Forked F given the preceding and following notes so fingers never slide across keys. |
| `diagnose_oboe_reed_response` | Diagnose sharp/flat A440 pitch, hard attacks, or collapsed openings on North American long-scrape and European short-scrape oboe reeds. |
| `lookup_conservatory_oboe_trills` | Look up dedicated trill keys (C-D trill levers, Ab-Bb trill, Left Eb-E, Banana key C-Db) on full Conservatory oboes. |

## Connect in 10 Seconds

### Claude Code
```bash
claude mcp add --transport http oboelib https://oboelib.com/api/mcp
```

### Cursor / Claude Desktop / Windsurf (`mcp.json`)
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

### Agent Skill (`skills.sh`)
```bash
npx -y skills@latest add AbigailDavised/oboelib-mcp -y
```

## License

MIT © [OboeLib](https://oboelib.com)
