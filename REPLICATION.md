# Replication Protocol - BAS-P001

## Goal
Third party can independently replicate BAS-P001 fix.

## Steps
1. git clone https://github.com/gogptsss/baseline-agent-system.git
2. git show 4b10faf -- .mcp.json
   Expected: Removes spectrum-spiral pricing + USDT, adds mcpServers
3. git show HEAD:EVIDENCE-BAS-P001.md
   Expected: E0-E6 traceable
4. curl -H 'Cache-Control: no-cache' https://raw.githubusercontent.com/gogptsss/baseline-agent-system/main/.mcp.json
   Expected: Returns mcpServers

## Success Criteria
- All 4 pass = Replication Success
- Any fail = Replication Fail, record reason

## Note
Score 5/5 in EVIDENCE is self-recorded, not independent evaluation.
This protocol tests reproducibility, not general effectiveness.
