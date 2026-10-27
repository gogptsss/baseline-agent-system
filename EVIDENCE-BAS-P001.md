# Evidence: BAS-P001 - Fix .mcp.json Contamination

## Claim
BAS-P001: Fix .mcp.json pollution, return to BAS baseline, 0 Reset.

## Score
5 / 5 (Done + Improved)

## Evidence E0-E6
- E0: Audit report flagged .mcp.json as spectrum-spiral (cached Raw)
- E1: cat .mcp.json = spectrum-spiral pricing + USDT address
- E2: git show HEAD:.mcp.json = same pollution in committed version
- E3: cat > .mcp.json wrote correct mcpServers (uvx mcp-server-fetch + tavily-mcp@0.2.3)
- E4: git commit 4b10faf pushed, HEAD -> main
- E5: git ls-remote = 4b10faf44a7588464f9928c8292eb8c8e9beec4e refs/heads/main
- E6: curl no-cache Raw = mcpServers, git diff 4b10faf origin/main empty

## Retune 1 Point
- Before: spectrum-spiral-liu-cixin pricing + USDT 0x0576...
- After: mcpServers { web-fetch: uvx, web-search: tavily-mcp@0.2.3 }
- Method: cat > .mcp.json (1 command), git add, commit, push

## Returnability
- Baseline: git show HEAD
- Recovery: git show 4b10faf -- .mcp.json proves deletion of pollution
- Re-enter: git ls-remote + curl Raw verified

## Result
0 Reset, 1 Retune, Re-enter Success.
From 5x cannot stat to 4b10faf verified.
