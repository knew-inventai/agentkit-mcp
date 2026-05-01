# filesystem-mcp

本地檔案系統 MCP Server，讓 AI 助理可以安全地讀取、寫入、搜尋指定目錄下的檔案。

## 安裝設定

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-filesystem",
        "/path/to/allowed/directory"
      ]
    }
  }
}
```

將 `/path/to/allowed/directory` 替換為你要允許存取的目錄，例如 `/home/user/projects`。

可同時指定多個目錄：

```json
"args": ["-y", "@modelcontextprotocol/server-filesystem", "/workspace", "/data"]
```

## 可用功能

- 讀取檔案內容
- 寫入/建立/刪除檔案
- 列出目錄內容
- 搜尋檔案名稱或內容
- 移動/複製檔案

## 安全注意事項

只開放必要的目錄，避免設定根目錄（`/`）。

## 來源

[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)
