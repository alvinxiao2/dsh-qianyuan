# Changelog

## 0.1.0

- Initial release.
- Mounts the QianYuan MCP server (`https://qianyuan.ltd/mcp`, streamable-http)
  via `@deepseek-ai/dsh-mcp-client`. Exposes 15 tools as `mcp__qianyuan__*`.
- Config-layer only: no runtime code, single `cordis.patch.yml` patch.
- Endpoint verified at publish time: `initialize` → HTTP 200 + `mcp-session-id`;
  `tools/list` → 15 tools.
