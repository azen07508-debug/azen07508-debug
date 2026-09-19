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

GitHub repository launch-readiness audit. Point it at a public repo and get a structured
report: evidence-backed findings (every claim carries a `path:line:reason` pointer),
rule-based reproducible scoring, and ready-to-paste launch copy.

Static analysis only — it never executes the audited repository's code. Exposed as an
MCP server, so any MCP-compatible agent can drive it directly.

`TypeScript` `Fastify` `MCP` `x402`

## Focus

- **AI agent infrastructure** — memory, skills, harness design, MCP tooling
- **DeFi primitives** — Uniswap v4 Hooks, onchain risk pricing, X Layer
- **Developer tooling** — the kind that actually ships

---

_中文：做链上金融与 AI Agent 基础设施的交叉地带。上面两个项目一个在 X Layer 上做 Uniswap v4 动态风险费率 Hook，一个把仓库上线就绪度审计做成 MCP 服务给 Agent 调用。_
