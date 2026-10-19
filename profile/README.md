<div align="center">

<img src="https://avatars.githubusercontent.com/u/249934078?s=400&v=4" alt="Nubra" width="120" />

# Nubra for Developers

**Trading and market data APIs for Indian markets.**
Build algos, options analytics, real-time dashboards and AI trading agents in Python.

[![PyPI](https://img.shields.io/pypi/v/nubra-sdk?label=nubra-sdk&color=1f6feb)](https://pypi.org/project/nubra-sdk/)
[![Downloads](https://img.shields.io/pypi/dm/nubra-sdk?color=1f6feb)](https://pypi.org/project/nubra-sdk/)
[![Docs](https://img.shields.io/badge/docs-nubra.io-0a7f5a)](https://nubra.io/products/api/docs/)
[![Discussions](https://img.shields.io/badge/community-discussions-8250df)](https://github.com/orgs/NubraAPI/discussions)
[![X](https://img.shields.io/badge/follow-@nubra__io-000000)](https://x.com/nubra_io)
[![YouTube](https://img.shields.io/badge/YouTube-@Nubra__io-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/@Nubra_io)

[🌐 Nubra Web](https://nubra.io/) · [📘 Docs](https://nubra.io/products/api/docs/) · [🍳 Cookbook](https://github.com/NubraAPI/nubra-cookbook) · [💬 Discussions](https://github.com/orgs/NubraAPI/discussions) · [✉️ Support](mailto:support@nubra.io)

</div>

---

## 📱 Get Nubra

You'll need a Nubra account to use the APIs. Sign up, complete KYC, and trade on web or mobile, then automate with the SDK.

<div align="center">

[![Open an account](https://img.shields.io/badge/Open%20an%20account-demat.nubra.io-0a7f5a?style=for-the-badge)](https://demat.nubra.io/)
[![Google Play](https://img.shields.io/badge/Google%20Play-Download-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=com.zanskar.nubra)
[![App Store](https://img.shields.io/badge/App%20Store-Download-0D96F6?style=for-the-badge&logo=apple&logoColor=white)](https://apps.apple.com/in/app/nubra-stocks-option-trading/id6746636699)

</div>

---

## ⚡ Quickstart

```bash
pip install nubra-sdk
```

```python
from nubra_python_sdk.start_sdk import InitNubraSdk, NubraEnv
from nubra_python_sdk.marketdata.market_data import MarketData

# UAT is the safe test environment. Switch to NubraEnv.PROD when you're ready.
nubra = InitNubraSdk(NubraEnv.UAT, env_creds=True)

chain = MarketData(nubra).option_chain("NIFTY", exchange="NSE").chain
print(chain.expiry, chain.at_the_money_strike)
```

> 💡 New here? Start on **UAT**. Every example in our repos runs there by default, so you can explore without touching real money.

<details>
<summary><b>More examples: live quotes, WebSockets, placing orders</b></summary>
<br/>

Runnable versions live in [nubra-python-sdk/examples](https://github.com/NubraAPI/nubra-python-sdk/tree/main/examples):

- 📈 Live quotes and market depth
- 📡 Streaming index ticks and order updates over WebSockets
- 🛒 Placing and tracking orders on UAT
- 📊 Option chain analytics: Greeks, OI, PCR and max pain

</details>

---

## 🧠 Build with AI

Using Claude, ChatGPT or Cursor? Download the **Nubra Master Docs**, the full SDK documentation in one Markdown file, and give it to your AI assistant so it writes correct Nubra code. [Get it from the docs →](https://nubra.io/products/api/docs/)

Want your AI assistant to read live market data directly? Use the [Nubra MCP server](https://github.com/socials-zanskar/nubra-mcp-server):

```bash
pip install nubra-mcp
```

---

## 📦 Repositories

| | Repo | What it is |
|---|---|---|
| 🐍 | [**nubra-python-sdk**](https://github.com/NubraAPI/nubra-python-sdk) | Official Python SDK docs, runnable examples and API reference |
| 🍳 | [**nubra-cookbook**](https://github.com/NubraAPI/nubra-cookbook) | Ready-to-run strategy projects: hedging bots, backtests, OI dashboards |
| 🤖 | [**nubra-mcp-server**](https://github.com/socials-zanskar/nubra-mcp-server) | Connect Nubra market data to Claude, ChatGPT, Cursor and other AI tools |

---

## 🧰 What you can build

<table>
<tr>
<td width="50%" valign="top">

**📊 Options analytics**
Option chains with Greeks, OI, PCR and max pain, ready for screeners and dashboards.

</td>
<td width="50%" valign="top">

**📡 Real-time apps**
WebSocket feeds for ticks, market depth, option chains and order updates.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🤖 Algo strategies**
Place, modify and track orders, including multi-leg baskets. Backtest and test on UAT first.

</td>
<td width="50%" valign="top">

**🧠 AI trading assistants**
Give AI agents live market data through the Nubra MCP server.

</td>
</tr>
</table>

---

## 🎓 Learn with us

- 🎥 [Learn with YouTube](https://www.youtube.com/@Nubra_io): delta hedging, gamma hedging, building with MCP, and more
- 🏫 Encountered bugs? Need help  Reach out at [support@nubra.io](mailto:support@nubra.io)

---

## 💬 Community

| | |
|---|---|
| 👋 **New here?** | Say hi in [Discussions](https://github.com/orgs/NubraAPI/discussions) |
| 🙏 **Stuck?** | Ask in [Q&A](https://github.com/orgs/NubraAPI/discussions/categories/q-a) |
| 🙌 **Built something?** | Share it in [Show and tell](https://github.com/orgs/NubraAPI/discussions/categories/show-and-tell). We feature community projects! |
| 💡 **Have an idea?** | Post it in [Ideas](https://github.com/orgs/NubraAPI/discussions/categories/ideas) |
| 🐛 **Found a bug?** | Open an [Issue](https://github.com/NubraAPI/nubra-python-sdk/issues) |
| ✉️ **Found a bug or need help?** | Email [support@nubra.io](mailto:support@nubra.io) and our team will get back to you! |

⭐ **If our repos help you, star them.** It helps other developers find Nubra too.

---

<div align="center">
<sub>
Nubra is a product of Zanskar Securities Private Limited · SEBI Registration No. INZ000316631<br/>
Code and content here are for educational and development purposes only and do not constitute investment advice. Investments in securities markets are subject to market risks; read all related documents carefully before investing.
</sub>
</div>
