# Nubra for Developers

**Trading and market data APIs for Indian markets.** Build algos, options analytics, dashboards and AI agents with Nubra's Python SDK, WebSocket feeds and MCP server.

[![PyPI](https://img.shields.io/pypi/v/nubra-sdk?label=nubra-sdk)](https://pypi.org/project/nubra-sdk/)
[![Docs](https://img.shields.io/badge/docs-nubra.io-blue)](https://nubra.io/products/api/docs/)
[![X](https://img.shields.io/badge/follow-@nubra__io-black)](https://x.com/nubra_io)

## ⚡ Quickstart

pip install nubra-sdk

from nubra_python_sdk.start_sdk import InitNubraSdk, NubraEnv
from nubra_python_sdk.marketdata.market_data import MarketData

nubra = InitNubraSdk(NubraEnv.UAT, env_creds=True)   # UAT = safe test environment
chain = MarketData(nubra).option_chain("NIFTY", exchange="NSE")
print(chain.chain.expiry, chain.chain.at_the_money_strike)

## 📦 Repositories

| Repo | What it is |
|---|---|
| [nubra-python-sdk](https://github.com/NubraAPI/nubra-python-sdk) | Official Python SDK docs, examples and reference |
| [nubra-cookbook](https://github.com/NubraAPI/nubra-cookbook) | Ready-to-run strategy projects: hedging bots, backtests, OI dashboards |
| [nubra-mcp-server](https://github.com/socials-zanskar/nubra-mcp-server) | Use Nubra market data with Claude, ChatGPT, Cursor and other AI tools |

## 🧰 What you can build

- 📊 Option chain analytics: Greeks, OI, PCR, max pain
- 📡 Real-time apps on WebSocket feeds for ticks, depth and order updates
- 🤖 Algo strategies and backtests, tested safely on UAT first
- 🧠 AI trading assistants with the Nubra MCP server

## 💬 Community

- 👋 Start here → [Discussions](https://github.com/orgs/NubraAPI/discussions)
- 🙏 Questions → [Q&A](https://github.com/orgs/NubraAPI/discussions/categories/q-a)
- 🙌 Built something? → [Show and tell](https://github.com/orgs/NubraAPI/discussions/categories/show-and-tell)
- 🐛 Bugs → [Issues](https://github.com/NubraAPI/nubra-python-sdk/issues)
- ✉️ Account and login help → support@nubra.io

---

<sub>Nubra is a product of Zanskar Securities Private Limited. Code and content here are for educational and development purposes only and do not constitute investment advice. Trading in securities involves risk.</sub>
