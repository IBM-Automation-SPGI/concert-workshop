# IBM Concert Workshop

<div style="background: linear-gradient(135deg, #0043ce 0%, #001141 60%, #0f62fe 100%); border-radius: 12px; padding: 3rem 2.5rem; margin: 1.5rem 0 2.5rem 0; text-align: center; box-shadow: 0 8px 32px rgba(0,67,206,0.35);">
  <div style="font-size: 0.85rem; font-weight: 600; letter-spacing: 0.18em; color: #78a9ff; text-transform: uppercase; margin-bottom: 0.6rem;">IBM Client Engineering</div>
  <div style="font-size: 2.4rem; font-weight: 700; color: #ffffff; letter-spacing: -0.01em; line-height: 1.15; margin-bottom: 0.5rem;">IBM Concert Workshop</div>
  <div style="font-size: 1.1rem; color: #a8c8ff; font-weight: 300; margin-bottom: 1.4rem;">Agentic ITOps · Observability · Resilience · Optimization</div>
  <div style="display: inline-flex; gap: 0.75rem; flex-wrap: wrap; justify-content: center;">
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🛡️ Concert Protect</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🔭 Concert Observe</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">⚡ Concert Resilience</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">📊 Concert Optimize</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🔄 Concert Workflows</span>
  </div>
</div>

!!! info "Welcome to the IBM Concert Workshop"
    This hands-on workshop will guide you through the key features of **IBM Concert**, the agentic ITOps platform that unifies observability, protection, operations and optimization in a single intelligent system.

    **Platform URL**: `https://concert.tec.spgi.ibm.com:12443`  
    **Username**: `ibmconcert`  
    **Estimated duration**: 4–5 hours

---

## What is IBM Concert?

IBM Concert is an agentic ITOps platform that creates a unified, adaptive operational layer across your entire environment. It connects signals, generates shared context, and coordinates actions between teams and tools so the whole system operates as one.

```mermaid
graph LR
    subgraph CONCERT["🎵 IBM CONCERT - Agentic ITOps Platform"]
        direction TB
        OBS["🔭 Concert Observe<br/>Full-Stack Observability"]
        PRO["🛡️ Concert Protect<br/>Vulnerabilities & Risk"]
        OPE["⚙️ Concert Resilience<br/>Incident Response"]
        OPT["📊 Concert Optimize<br/>Resources & Cost"]
        WFL["🔄 Concert Workflows<br/>Low-Code Automation"]
        RES["🔁 Concert Resilience<br/>Recovery & Reliability"]
    end

    APP["Applications"] --> CONCERT
    INFRA["Infrastructure"] --> CONCERT
    NET["Network"] --> CONCERT
    CONCERT --> ACTION["✅ Insight → Action"]

    style CONCERT fill:#e8f0fe,stroke:#0043ce,stroke-width:2px
    style OBS fill:#e0f7fa,stroke:#009d9a
    style PRO fill:#fde8e8,stroke:#da1e28
    style OPE fill:#e3f2fd,stroke:#0f62fe
    style OPT fill:#e8f5e9,stroke:#198038
    style WFL fill:#f3e5f5,stroke:#8a3ffc
    style RES fill:#fff3e0,stroke:#ff832b
```

---

## Workshop Modules

| Lab | Module | Description | Duration |
|-----|--------|-------------|----------|
| 🚀 **Lab 0** | Prerequisites | Environment check and access to Concert | 10 min |
| 🏠 **Lab 1** | Introduction | Navigation and main Concert dashboard | 15 min |
| 🛡️ **Lab 2** | Concert Protect | CVE vulnerability management and SBOM | 25 min |
| 🔭 **Lab 3** | Concert Observe | Full-stack observability with IBM Instana | 20 min |
| ⚙️ **Lab 4** | Concert Resilience | Incident management and response | 20 min |
| 📊 **Lab 5** | Concert Optimize | Resource optimization with IBM Turbonomic | 15 min |
| 🔄 **Lab 6** | Concert Workflows | Workflow automation | 15 min |

---

## Environment Architecture

```mermaid
graph TB
    subgraph CLIENT["Your Environment"]
        BROWSER["🌐 Web Browser<br/>(Chrome/Firefox)"]
    end

    subgraph CONCERT_ENV["IBM Concert Environment (Demo)"]
        direction TB
        CONCERT_UI["Concert UI<br/>:12443/platform"]
        API["Concert API"]
        DB["Configuration<br/>Database"]
        AI["AI Engine<br/>IBM Agent"]
        
        subgraph MONITORED["Monitored Applications"]
            APP1["App: RobotShop"]
            APP2["App: BookInfo"]
            APP3["App: Sock Shop"]
        end
    end

    BROWSER -->|HTTPS| CONCERT_UI
    CONCERT_UI --> API
    API --> DB
    API --> AI
    API --> MONITORED

    style CONCERT_ENV fill:#e8f0fe,stroke:#0043ce,stroke-width:2px
    style MONITORED fill:#f4f4f4,stroke:#525252
```

---

## Prerequisites

!!! warning "Before you begin"
    Make sure you have the following available:

- [x] Access to a modern browser (Chrome 90+ or Firefox 88+)
- [x] Access to the Concert environment URL
- [x] Credentials provided by the instructor
- [x] Connection to the lab network

---

## Workshop Security Policy

!!! danger "Security Notice"
    The credentials provided are **exclusively for use in this workshop**. Do not share them outside the lab environment. The environment will be reset at the end of the session.

---

## Workshop Support

If you encounter any issues during the labs:

1. Check the **"Troubleshooting"** section at the end of each lab
2. Ask the instructor for help
3. Review the Concert platform logs at `Settings > Logs`
