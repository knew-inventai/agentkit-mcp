# agentkit-mcp

AgentKit MCP Servers 集合。每個子目錄為一個 MCP server package。

## 安裝（Claude Code）

```shell
/plugin marketplace add knew-inventai/agentkit-mcp
/plugin install MCP_NAME@agentkit-mcp
```

## 目錄結構

```
agentkit-mcp/
  .claude-plugin/
    marketplace.json    ← Claude Code marketplace 定義（自動維護）
  {mcp-name}/
    plugin.json         ← Package metadata
    README.md           ← 說明文件（含安裝指令）
```
