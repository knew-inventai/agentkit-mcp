# fetch-mcp

網頁抓取 MCP Server，讓 AI 助理能直接擷取任意 URL 的內容，自動將 HTML 轉換為 Markdown 格式。

## 安裝設定

```json
{
  "mcpServers": {
    "fetch": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-fetch"]
    }
  }
}
```

## 可用功能

- 抓取網頁內容（回傳 Markdown）
- 擷取原始 HTML
- 支援帶 HTTP headers 的請求

## 使用情境

- 查閱線上文件
- 抓取 API 回傳的 JSON
- 確認網站是否正常運作
- 搜集公開資料

## 來源

[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch)
