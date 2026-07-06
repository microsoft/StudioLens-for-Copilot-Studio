<div align="center">

# 🔎 StudioLens

#### by Microsoft Business Value Advisory (BVA)

### **for Copilot Studio** — a Power BI template for **deep agent performance & evaluation**: quality, containment, topics, transcripts, errors, feedback, and message-credit consumption.

[![Built by Microsoft BVA](https://img.shields.io/badge/BUILT_BY-MICROSOFT_BVA-4F73B8?style=for-the-badge&labelColor=1C2632)](https://github.com/Keithland89/StudioLens-for-Copilot-Studio)
[![Power BI Template](https://img.shields.io/badge/POWER_BI-TEMPLATE-F2C811?style=for-the-badge&logo=powerbi&logoColor=1C2632&labelColor=1C2632)](#choose-your-path)
[![Deploy](https://img.shields.io/badge/DEPLOY-DATAVERSE_OR_FABRIC-09B39D?style=for-the-badge&labelColor=1C2632)](#choose-your-path)
[![Stars](https://img.shields.io/github/stars/Keithland89/StudioLens-for-Copilot-Studio?style=for-the-badge&color=7F215D&labelColor=1C2632)](https://github.com/Keithland89/StudioLens-for-Copilot-Studio/stargazers)

**Agent sessions · turns · errors · sub-agent calls · quality & performance · topics · knowledge files ·
user feedback · Copilot Studio message-credit consumption** — purpose-built to analyse how your
**Copilot Studio agents** actually perform, resolve, contain, and cost.

![StudioLens for Copilot Studio — demo](./assets/studiolens-demo.gif)

> *Demo shown with anonymised sample data.*

Found this useful? ⭐ **Star this repo to help others discover it!**

**[Choose your path ↓](#choose-your-path)**

</div>

<details>
<summary>⚠️ <strong>Usage & compliance disclaimer</strong></summary>

While this tool helps customers understand the business value of their AI usage data, Microsoft has
**no visibility** into the data customers input, nor control over how the template is used. Customers
are solely responsible for ensuring their use complies with all applicable laws and regulations
(including data privacy and security). **Microsoft disclaims all liability** arising from use of this
template.

This is an **experimental** template that reads Copilot Studio conversation transcripts from
Dataverse. Transcripts are intended to give visibility into agent interactions, not to serve as the
sole source of truth for licensing or full-fidelity reporting. Not supported through Microsoft
support channels — please open an issue in this repo.
</details>

---

## Choose your path

Two builds of the **same StudioLens** template. Each path folder is **self-contained** — the template,
notebooks/resources, and step-by-step setup all live inside it. Pick the one that fits your platform:

| Path | Best for | What you need | Go to |
|---|---|---|---|
| **1 · Dataverse (Direct)** ⭐ | the **simplest** footprint — transcripts parsed live **in the Power BI model** (Power Query M); nothing else to stand up | a Dataverse environment + an org-data CSV | **[`1. Dataverse (Direct)/`](./1.%20Dataverse%20(Direct)/)** |
| **2 · Fabric** | **scheduled** Spark ingestion, larger volumes, and the **PPAC message-credit** pages | a Fabric capacity + Lakehouse | **[`2. Fabric/`](./2.%20Fabric/)** |

Both surface the same Copilot Studio agent analytics — **Dataverse (Direct)** reads live transcripts and
parses them in-model; **Fabric** lands them (plus credit consumption) as Delta tables for scale and
scheduling. New to StudioLens? Start with **Dataverse (Direct)** for the fastest look.

| | Dataverse (Direct) | Fabric |
|---|---|---|
| Setup effort | ✅ lowest (open `.pbit`, set 3 params) | notebooks + Lakehouse |
| Infrastructure | none | Fabric capacity + Lakehouse |
| Transcript pages (quality, topics, flow, errors, feedback) | ✅ | ✅ |
| PPAC message-credit pages | ✖ | ✅ |
| Best data volume | small–medium (Dataverse ~30-day retention) | large / historical |
| Multi-environment | ✅ (one or many Dataverse URLs) | via Lakehouse |

---

## Related

**StudioLens is part of [CopilotScope](https://github.com/Keithland89/CopilotScope)** — a wider kit of
Power BI "lenses" for Microsoft 365 Copilot (value, adoption, readiness, maturity, behaviour, leadership).
StudioLens is the **Copilot Studio agent** lens, available here as a **standalone** template (incl.
Dataverse-Direct, no Fabric) for teams who only need the agent deep-dive. Want the broader
whole-Copilot value story too? See **[CopilotScope](https://github.com/Keithland89/CopilotScope)**.

## About

StudioLens and CopilotScope are created and maintained by the **Microsoft Business Value Advisory (BVA)** team.
