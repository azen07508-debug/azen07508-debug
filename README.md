# azen07508-debug

Building at the intersection of onchain finance and AI agent infrastructure.

## Projects

### [XGuard Hook](https://github.com/azen07508-debug/xguard-hook)

Dynamic risk-fee [Uniswap v4](https://docs.uniswap.org/contracts/v4/overview) Hook for new-asset,
meme, and low-cap pools on X Layer. LP fees scale with swap impact — `Normal` 0.30%,
`Warning` 1.00%, `Protected` 3.00% — and the pool's risk state is verifiable onchain, so
traders and LPs price the same risk the contract does.

Ships with a demo router, a live frontend, and a Foundry test suite covering the fee
override, risk decay, and hard-threshold blocking paths.

`Solidity` `Foundry` `Uniswap v4` `X Layer` — [live demo](https://xguard-hook.vercel.app)

### [RepoPilot](https://github.com/azen07508-debug/repopilot)

The quality layer for agents that ship code. Point it at a public repo and get
evidence-backed findings (every claim carries a `path:line:reason` pointer) and
rule-based reproducible scoring — plus a **fix plan per finding**: ordered steps,
tests to add, acceptance criteria, and an `agentInstructions` block you can hand
straight to Codex or Claude Code.

Re-audit and see what actually changed: score movement attributed rule by rule,
findings split into resolved / new / still-open. The loop is
audit → fix plan → fix → re-audit → compare, over HTTP or MCP.

Static analysis only — it never executes the audited repository's code.

`TypeScript` `Fastify` `MCP` `x402`

## Focus

- **AI agent infrastructure** — memory, skills, harness design, MCP tooling
- **DeFi primitives** — Uniswap v4 Hooks, onchain risk pricing, X Layer
- **Developer tooling** — the kind that actually ships

---

_中文：做链上金融与 AI Agent 基础设施的交叉地带。上面两个项目，一个在 X Layer 上做 Uniswap v4 动态风险费率 Hook；另一个是给 Agent 用的仓库质量层——审计出问题、给出可执行的修复计划、改完再审计做前后对比。_
