# 🌾 Ask Loudi — AI Agricultural Assistant for Rwanda

**Ask Loudi** is a multilingual AI-powered agricultural knowledge assistant built by [Loudi Agricultural Development Limited](https://loudiagri.com) (LADL) and [Yuelu Tech Limited](https://yuelu.tech), designed to support rice farming across Rwanda.

> _Bridging Chinese agricultural expertise with East African farming realities through AI._

---

## What We Do

Ask Loudi provides practical, research-backed agricultural guidance to Rwandan farmers, agronomists, and extension workers — in **English**, **Chinese (中文)**, and **Kinyarwanda**.

Our knowledge base draws from:

- 🇨🇳 China Agricultural University's ShenNong agricultural AI framework
- 🇷🇼 Rwanda Agriculture Board (RAB) technical publications
- 🌾 MINAGRI National Rice Development Strategy (NRDS-II)
- 📊 Rwanda-specific varietal trials, soil data, and seasonal calendars

## Architecture

```
┌─────────────┐     ┌──────────────┐     ┌─────────────────┐
│   WhatsApp   │────▶│  RAG Engine   │────▶│  LLM (Gemini)   │
│   / Web UI   │◀────│  + Embeddings │◀────│  Response Gen    │
└─────────────┘     └──────┬───────┘     └─────────────────┘
                           │
                    ┌──────▼───────┐
                    │  Knowledge   │
                    │  Base (9000+   │
                    │  documents)  │
                    └──────────────┘
```

**Key design principles:**
- **RAG-first**: All responses are grounded in verified agronomic data — no hallucination
- **Multilingual by default**: Language detection with automatic response matching
- **Low-bandwidth friendly**: Optimized for WhatsApp delivery in areas with limited connectivity
- **Self-hosted**: Full deployment on private infrastructure for data sovereignty

## Supported Topics

| Domain | Examples |
|--------|----------|
| Rice Cultivation | Varieties, planting seasons, nursery management |
| Crop Management | Fertilization, irrigation, weed control |
| Pest & Disease | Rice blast, bacterial blight, stem borers |
| Agricultural Machinery | Land preparation, harvesting equipment |
| Policy & Programs | RAB guidelines, MINAGRI programs, seed certification |

## Project Context

LADL operates a rice localization and adaptive breeding program (属地化适应性测试与原种繁育) in Rwanda under the Loudi–Muhanga sister-city framework. Ask Loudi is the digital knowledge layer supporting this initiative — making Chinese agricultural expertise accessible to Rwandan farming communities.

**Yuelu Tech Limited** (Kigali, Rwanda) develops and maintains the AI infrastructure powering Ask Loudi.

## Open-Source Contributions

This repository hosts **non-confidential resources** we share with the community:

| Resource | Description | Status |
|----------|-------------|--------|
| NLP Glossary | Kinyarwanda–English–Chinese agricultural term mappings | 🔜 Coming soon |
| Prompt Templates | RAG prompt structures for agricultural advisory | 🔜 Coming soon |
| Evaluation Sets | Multilingual Q&A pairs for agricultural AI benchmarking | 🔜 Coming soon |

> ⚠️ The core application, knowledge base content, and model configurations are proprietary and not included in this repository.

## Tech Stack

- **LLM**: Google Gemini (via API)
- **Embeddings**: Jina AI (jina-embeddings-v3)
- **RAG Platform**: FastGPT (self-hosted)
- **Infrastructure**: Docker Compose on cloud VPS
- **Delivery**: Web UI + WhatsApp Business API (planned)

## Contact

| | |
|---|---|
| 🏢 LADL | Loudi Agricultural Development Limited, Hunan, China |
| 🏢 Yuelu Tech | Kigali, Rwanda |
| 🌐 Website | [yuelu.tech](https://yuelu.tech) \| [loudiagri.com](https://loudiagri.com) |
| ✉️ Email | info@yuelu.tech |

---

<p align="center">
  <i>Built with 🌾 for Rwandan agriculture</i><br>
  <sub>© 2026 Yuelu Tech Limited & Loudi Agricultural Development Limited</sub>
</p>
