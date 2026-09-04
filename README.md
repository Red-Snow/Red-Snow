<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/hero-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/hero-light.svg">
  <img alt="Red-Snow — Offensive Security · Agentic AI · Signal Intelligence" src="./assets/hero-dark.svg" width="100%">
</picture>

<br/>

[![Followers](https://img.shields.io/github/followers/Red-Snow?style=flat-square&logo=github&color=FF3333&labelColor=0d1117&label=followers)](https://github.com/Red-Snow?tab=followers)
[![Views](https://komarev.com/ghpvc/?username=Red-Snow&style=flat-square&color=FF3333&labelColor=0d1117&label=profile+views)](https://github.com/Red-Snow)
[![Focus](https://img.shields.io/badge/focus-AI%20%C3%97%20offensive%20security-FF3333?style=flat-square&labelColor=0d1117)](#featured-work)
[![Stack](https://img.shields.io/badge/stack-Python%20%C2%B7%20TypeScript%20%C2%B7%20MCP-FF3333?style=flat-square&labelColor=0d1117)](#toolkit)

</div>

---

```console
$ whoami
Red-Snow — offensive security engineer · AI tooling builder

$ cat ./focus.md
[1] PhantomStrike ........ AI agents that run real penetration tests
[2] AI-Malware-Analyzer .. browser-native DFIR, zero backend
[3] Research ............. Conformer networks for physiological signals
```

I build the layer between AI agents and real security work — MCP servers, structured tool
output, and forensic pipelines that return evidence instead of guesses. On the research side:
convolution-augmented Transformers for physiological signal analysis.

---

## Featured Work

<table>
<tr>
<td width="50%" valign="top">

### ⚡ [PhantomStrike](https://github.com/Red-Snow/phantomstrike)

An MCP server that hands any AI agent a full Kali toolchain.
Natural language in, structured multi-step pentest out.

<sub>`Python` · `FastAPI` · `MCP` · `Docker`</sub>

[![Stars](https://img.shields.io/github/stars/Red-Snow/phantomstrike?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike/stargazers)
[![Updated](https://img.shields.io/github/last-commit/Red-Snow/phantomstrike?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/phantomstrike/commits)

</td>
<td width="50%" valign="top">

### 🔬 [AI-Malware-Analyzer](https://github.com/Red-Snow/AI-Malware-Analyzer)

A complete DFIR workflow that never leaves the browser tab —
PE parsing, IOC extraction, ATT&CK mapping, PDF evidence.

<sub>`JavaScript` · `10+ LLM engines` · `zero-backend`</sub>

[![Stars](https://img.shields.io/github/stars/Red-Snow/AI-Malware-Analyzer?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/AI-Malware-Analyzer/stargazers)
[![Updated](https://img.shields.io/github/last-commit/Red-Snow/AI-Malware-Analyzer?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/AI-Malware-Analyzer/commits)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🕵️ [StegInsight-Forensics](https://github.com/Red-Snow/StegInsight-Forensics)

Steganography detection across text, image and audio/video
carriers, built for fast forensic triage.

<sub>`TypeScript` · `DSP` · `entropy analysis`</sub>

[![Stars](https://img.shields.io/github/stars/Red-Snow/StegInsight-Forensics?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/StegInsight-Forensics/stargazers)
[![Updated](https://img.shields.io/github/last-commit/Red-Snow/StegInsight-Forensics?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/StegInsight-Forensics/commits)

</td>
<td width="50%" valign="top">

### 🌐 [redsnow-recon-toolkit](https://github.com/Red-Snow/redsnow-recon-toolkit)

A browser-based recon and OSINT lab — interactive threat
analysis, simulated probes, and an AI cyber mentor.

<sub>`TypeScript` · `OSINT` · `LLM`</sub>

[![Stars](https://img.shields.io/github/stars/Red-Snow/redsnow-recon-toolkit?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/redsnow-recon-toolkit/stargazers)
[![Updated](https://img.shields.io/github/last-commit/Red-Snow/redsnow-recon-toolkit?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/redsnow-recon-toolkit/commits)

</td>
</tr>
</table>

---

## How PhantomStrike Works

> One sentence from the operator becomes a chained, multi-tool engagement —
> and comes back as parsed JSON, not scrollback.

```mermaid
flowchart LR
    U(["Operator"]) -->|plain English| A["AI Agent<br/>Claude · Cursor · Copilot · Gemini"]
    A <-->|MCP| P["PhantomStrike<br/>FastAPI · async job queue"]
    P --> R["Recon<br/>nmap · rustscan · masscan"]
    P --> W["Web<br/>nuclei · sqlmap · ffuf · nikto"]
    P --> O["OSINT<br/>subfinder · amass"]
    P --> S["run_kali_shell<br/>any Kali command"]
    R --> J["Structured JSON<br/>+ SQLite scan history"]
    W --> J
    O --> J
    S --> J
    J -->|findings| A

    classDef core stroke:#FF3333,stroke-width:2px
    classDef tool stroke:#8B949E,stroke-width:1px
    class A,P,J core
    class R,W,O,S tool
```

```text
"Scan 192.168.1.1 for open ports, then audit every web service for SQLi."

  → nmap        discovers 22, 80, 8080
  → nuclei      fingerprints two web stacks
  → sqlmap      confirms injection on /search?q=
  → report      severity-ranked JSON ✓
```

|  | |
|:--|:--|
| **Deploys as** | All-in-Kali · Split (Host + VM) · Docker |
| **Speaks to** | Claude Desktop · Cursor · VS Code + Copilot · Gemini CLI · any MCP client |
| **Ships with** | 12 structured plugins · async job queue · SQLite history · OpenAPI docs |
| **Escape hatch** | `run_kali_shell` — any Kali command, driven by the agent |

<div align="center">

[![Explore PhantomStrike](https://img.shields.io/badge/explore_PhantomStrike-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike)
&nbsp;
[![Explore AI Malware Analyzer](https://img.shields.io/badge/explore_AI--Malware--Analyzer-0d1117?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/AI-Malware-Analyzer)

</div>

---

## Toolkit

<table>
<tr><td valign="middle" width="130"><b>Offensive</b></td><td>

![Kali](https://img.shields.io/badge/Kali-557C94?style=flat-square&logo=kalilinux&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logo=metasploit&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp-FF6633?style=flat-square&logo=portswigger&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-214478?style=flat-square&logo=nmap&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C7192E?style=flat-square)

</td></tr>
<tr><td valign="middle"><b>AI / ML</b></td><td>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

</td></tr>
<tr><td valign="middle"><b>Platform</b></td><td>

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</td></tr>
<tr><td valign="middle"><b>Agents</b></td><td>

![MCP](https://img.shields.io/badge/Model_Context_Protocol-6B46C1?style=flat-square)
![Claude](https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white)

</td></tr>
</table>

---

## Current Work

<table>
<tr>
<td width="50%" valign="top">

**Agentic security & forensics**

Autonomous recon → exploitation → reporting, with every tool
returning structured output an agent can actually reason over.

- LLM tool-chaining for pentest workflows
- Natural-language execution layers over real binaries
- Hidden-data detection across carriers

</td>
<td width="50%" valign="top">

**Physiological deep learning**

Convolution-augmented Transformer (Conformer) architectures for
signal processing and assessment.

- Automated signal decomposition
- Hybrid neural architectures
- Cross-validation on expansive datasets

</td>
</tr>
</table>

<div align="center">

<img src="https://streak-stats.demolab.com?user=Red-Snow&theme=dark&hide_border=true&background=0D1117&border=FF3333&ring=FF3333&fire=FF6B6B&currStreakLabel=FF3333&sideLabels=8B949E&dates=6E7681&currStreakNum=F0F6FC&sideNums=F0F6FC" width="62%" alt="Contribution streak"/>

</div>

---

<div align="center">

[![GitHub](https://img.shields.io/badge/@Red--Snow-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow)
[![Open an issue](https://img.shields.io/badge/open_an_issue-0d1117?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike/issues)

<sub>*"The quieter you become, the more you are able to hear."*</sub>

</div>
