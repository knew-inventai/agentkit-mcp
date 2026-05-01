# github-mcp

GitHub 官方 MCP Server，讓 AI 助理可以直接操作 GitHub repos、issues、pull requests、branches 與檔案。

## 安裝設定

將 `mcp-config.json` 的內容合併至你的 Claude Code / Cursor MCP 設定中：

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<your-token>"
      }
    }
  }
}
```

## 取得 Token

1. 前往 https://github.com/settings/tokens
2. 建立 Personal Access Token（需要 `repo`、`read:org` 等 scope）
3. 將 token 填入設定的 `GITHUB_PERSONAL_ACCESS_TOKEN`

## 可用功能

- 列出/建立/搜尋 repositories
- 建立/更新 issues 與 PR
- 讀取/寫入檔案內容
- 管理 branches 與 commits
- 搜尋 code

## 來源

[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers/tree/main/src/github)
