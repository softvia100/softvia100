<div align="center">

<br />

<img src="https://qianwen-res.oss-accelerate-overseas.aliyuncs.com/logo_qwen3.png" alt="OpenAgent" width="280" />

<br />
<br />

**The open-source operating system for AI agents.**

Not a framework. Not a library. **Infrastructure.**

<br />

[![](https://img.shields.io/badge/openagent.io-3D5AFE?style=flat-square&logo=safari&logoColor=white)](https://openagent.io)
[![](https://img.shields.io/badge/docs-00E5FF?style=flat-square&logo=readthedocs&logoColor=black)](https://docs.openagent.io)
[![](https://img.shields.io/badge/discord-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/openagent)
[![](https://img.shields.io/badge/license-Apache_2.0-22c55e?style=flat-square)](https://opensource.org/licenses/Apache-2.0)

</div>

---

```bash
npm install -g @openagent/cli
openagent init my-agent && openagent dev agent.yaml
```

*First agent running in under 5 minutes.*

---

### What we're building

OpenAgent lets you define agents in YAML, deploy them to any infrastructure, route across any model, and observe every token — all through a single CLI. Think Kubernetes, but for AI agents.

```yaml
spec:
  model:
    provider: anthropic
    name: claude-3-7-sonnet-20250219
  routing:
    fallback: [openai/gpt-4o, groq/llama-3.1-70b-versatile]
  tools: [web_search, read_url, write_file]
  memory:
    vector: { backend: pgvector }
```

---

### Repositories

| | |
|---|---|
| [**openagent/openagent**](https://github.com/openagent/openagent) | Core runtime — the main repo |
| [**openagent/cli**](https://github.com/openagent/cli) | CLI binary (`openagent`) |
| [**openagent/examples**](https://github.com/openagent/examples) | Ready-to-run agent library |
| [**openagent/helm**](https://github.com/openagent/helm) | Kubernetes Helm charts |
| [**openagent/docs**](https://github.com/openagent/docs) | Documentation site |

---

### Stack

`Go` · `Python` · `Rust` · `PostgreSQL + pgvector` · `Redis` · `NATS` · `Kubernetes` · `OpenTelemetry`

---

<div align="center">

Apache 2.0 · Built in the open · [Contribute →](https://github.com/openagent/openagent/blob/main/CONTRIBUTING.md)

</div>
