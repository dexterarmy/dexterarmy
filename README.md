### Mohit Sharma

**Full Stack Software Engineer — I build the layer that makes AI agents safe to run in production.**

MCP servers, policy engines, and tamper-evident audit trails, in TypeScript and Node.js.
India.

📄 **[dexterarmy.github.io/portfolio](https://dexterarmy.github.io/portfolio/)** · ✉️ [immohitsharma8@gmail.com](mailto:immohitsharma8@gmail.com) · 💼 [LinkedIn](https://linkedin.com/in/mohit-sharma-094517249)

---

#### What I work on

I'm one of three engineers owning an enterprise **AI Governance, Risk & Compliance** platform. That put me on the unglamorous half of agentic AI: permissions, data boundaries, and proving after the fact what an agent actually did.

The main thing I've built is the platform side of **Asenion AI Guardian** — an AI-governance runtime delivered as an **MCP service that agents call before they take an action**. Every consultation writes a tamper-evident, hash-chained witness record, so each record's hash covers the one before it and altering history breaks the chain. I built agent enrollment, the token-exchange endpoint (RFC 8705 certificate-bound tokens), per-organization JWKS, and witness-record ingest. It exposes three tools — `list_policies`, `consult_policy`, `evaluate_response` — to any MCP-capable agent.

I also wrote the zero-dependency Node.js **stdio bridge** connecting Claude Desktop to Guardian's streamable-HTTP MCP server behind mTLS, minting a fresh single-use RS256 token per request.

#### Pinned work

**[consult-first](https://github.com/dexterarmy/consult-first)** — a chat agent on Cloudflare that must consult a policy table before it acts. Llama 3.3 on Workers AI drives a tool-calling loop where every consequential tool is gated: the policy verdict decides whether the call runs, pauses for human Approve/Deny, or is refused with the policy named. State lives in a Durable Object with its own SQLite; a Workflow audits the hash chain on demand.

#### Toolkit

`TypeScript` `JavaScript` `Python` `Node.js` `Express` `GraphQL` `Apollo Server 4` `React 18` `Next.js` `MongoDB` `PostgreSQL` `Redis` `DataLoader` `MCP` `@modelcontextprotocol/sdk` `Claude API` `Azure OpenAI` `AWS Bedrock` `RAG` `embeddings` `vector search` `Docker` `GitHub Actions` `CI/CD` `BullMQ` `Prometheus` `JWT` `OAuth2` `RBAC` `multi-tenancy`

---

