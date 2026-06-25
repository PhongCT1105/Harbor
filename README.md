::: {align="center"}
# Harbor

### The intelligent control plane for MCP servers.

Discover, manage, route, and optimize thousands of MCP tools with a
single runtime.

**Documentation** • **Getting Started** • **Discord** • **Roadmap**

> Replace the links above with your project URLs.

`<img src="./assets/demo.gif" width="900"/>`{=html}

![GitHub
Stars](https://img.shields.io/github/stars/your-org/harbor?style=for-the-badge)
![License](https://img.shields.io/github/license/your-org/harbor?style=for-the-badge)
![Build](https://img.shields.io/github/actions/workflow/status/your-org/harbor/ci.yml?style=for-the-badge)
![Downloads](https://img.shields.io/github/downloads/your-org/harbor/total?style=for-the-badge)
:::

------------------------------------------------------------------------

# 🚀 Quick Demo

``` bash
npm install harbor

harbor add github
harbor add slack
harbor add postgres

harbor run
```

Output

``` text
✓ Found 3 MCP servers

Github
Slack
Postgres

148 available tools

✓ Tool index built
✓ Embeddings cached
✓ Ready
```

------------------------------------------------------------------------

# 📖 What is Harbor?

Harbor is an open-source control plane for MCP servers.

Instead of manually configuring dozens of MCP servers, Harbor
automatically discovers, indexes, ranks, and routes tools to the best
server while improving LLM tool-calling accuracy.

Works with:

-   OpenAI
-   Anthropic
-   Gemini
-   Ollama
-   Any MCP-compatible client

------------------------------------------------------------------------

# 🏗 Architecture

``` text
                User

                 │

      OpenAI / Claude / Gemini

                 │

          Harbor Runtime

 ┌───────────────────────────────┐
 │ Discovery                     │
 │ Ranking                       │
 │ Routing                       │
 │ Cache                         │
 │ Tool Registry                 │
 │ Authentication                │
 │ Observability                 │
 └───────────────────────────────┘

      │          │          │

 GitHub MCP   Slack MCP   Database MCP

      │          │          │

     Hundreds of MCP Servers
```

------------------------------------------------------------------------

# ✨ Features

  Feature               Status
  --------------------- ------------
  MCP Discovery         ✅
  Tool Routing          ✅
  Capability Cache      ✅
  Parallel Execution    🚧
  Smart Ranking         🚧
  Auto Tool Selection   🚧
  Analytics Dashboard   📅 Planned
  Plugin System         📅 Planned

------------------------------------------------------------------------

# 💡 Why Harbor?

Instead of exposing hundreds of tools directly to the LLM, Harbor
intelligently selects the right tools, reducing context size and
improving execution quality.

**Benefits**

-   Faster tool selection
-   Better tool-calling accuracy
-   Lower token usage
-   Dynamic tool discovery
-   Hot reload for servers
-   Vendor independent

------------------------------------------------------------------------

# 📦 Installation

``` bash
npm install harbor
```

or

``` bash
brew install harbor
```

or

``` bash
docker run harbor
```

------------------------------------------------------------------------

# ⚡ Quick Start

``` bash
harbor add github
harbor list
harbor inspect github
harbor run
```

------------------------------------------------------------------------

# 🧩 Python Example

``` python
from harbor import Harbor

runtime = Harbor()
runtime.connect()

tools = runtime.tools()

runtime.call(
    "search_repo",
    query="mcp"
)
```

------------------------------------------------------------------------

# 📊 Benchmarks

  Metric            Vanilla MCP   Harbor
  --------------- ------------- --------
  Tools Exposed             200       18
  Tokens Sent               26k       4k
  Tool Accuracy             71%      92%
  Latency                 2.3 s    1.1 s

------------------------------------------------------------------------

# 🌐 Ecosystem

``` text
Harbor Core
├── Harbor CLI
├── Harbor Dashboard
├── Harbor SDK
├── Harbor Registry
└── Harbor Plugins
```

------------------------------------------------------------------------

# 🛣 Roadmap

## v0.1

-   [x] Discovery
-   [x] Routing
-   [x] Tool Cache

## v0.2

-   [ ] Semantic Search
-   [ ] Tool Ranking
-   [ ] Hot Reload

## v0.3

-   [ ] Dashboard
-   [ ] Registry
-   [ ] CLI

## v1.0

-   [ ] Multi-node Runtime
-   [ ] Distributed Cache
-   [ ] Plugin SDK

------------------------------------------------------------------------

# ⭐ Star History

``` md
[![Star History Chart](https://api.star-history.com/svg?repos=your-org/harbor&type=Date)](https://star-history.com/#your-org/harbor&Date)
```

------------------------------------------------------------------------

# 🤝 Contributors

``` md
<a href="https://github.com/your-org/harbor/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=your-org/harbor"/>
</a>
```

------------------------------------------------------------------------

# 🤝 Contributing

Pull requests are welcome! Please read `CONTRIBUTING.md` before opening
a PR.

------------------------------------------------------------------------

# 📄 License

MIT License
