# BAS Web MCP Guide - BAS 联网增强

BAS = Baseline Agent System / 定锚系统

## 3个 MCP 能力
- web-fetch: 抓任意 URL
- web-browser: 浏览器操作
- web-search: Tavily 联网搜索

## 使用方法
1. 下载 mcp.json 改名为 .mcp.json 放到项目根目录
2. 在 Cursor / Claude / VS Code 开启 MCP
3. Agent 即可联网搜索 -> 抓取 -> 按 BAS 模板输出

## BAS 工作流
搜索 -> 抓取 -> Baseline Check -> Retune 1 point -> Re-enter

## 快速测试
Ask Agent: 用 web-fetch 抓 https://example.com 并用 BAS 格式总结
