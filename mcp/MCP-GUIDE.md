# BAS Web MCP Guide - BAS 联网增强

BAS = Baseline Agent System / 定锚系统

## 2个 MCP 能力
- web-fetch: 抓任意 URL(`uvx mcp-server-fetch`)
- web-search: Tavily 联网搜索(`tavily-mcp@0.2.3`)

## 前置条件
- 安装 [uv](https://docs.astral.sh/uv/)(提供 `uvx`),供 web-fetch 使用
- 安装 Node.js,并到 tavily.com 申请 API Key,供 web-search 使用

## 使用方法
1. 把本目录的 mcp.json 复制到你的项目根目录,并改名为 .mcp.json(内容与本仓库根目录的 .mcp.json 相同)
2. 把 `YOUR_TAVILY_KEY` 换成你自己的 Tavily API Key(只在本地修改,不要提交到仓库)
3. 在 Cursor / Claude / VS Code 开启 MCP
4. Agent 即可联网搜索 -> 抓取 -> 按 BAS 模板输出

> 如果客户端启动 web-search 时卡住,可能是 npx 在等待安装确认。可先在终端运行一次 `npx tavily-mcp@0.2.3` 完成安装。

## BAS 工作流
搜索 -> 抓取 -> Baseline Check -> Retune 1 point -> Re-enter

## 快速测试
Ask Agent: 用 web-fetch 抓 https://example.com 并用 BAS 格式总结
