<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF0000,50:8B0000,100:0d1117&height=240&section=header&text=Red-Snow&fontSize=100&fontColor=ffffff&fontAlignY=42&desc=Offensive%20Security%20%E2%80%A2%20Agentic%20AI%20%E2%80%A2%20Deep%20Learning&descAlignY=62&descSize=18&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1500&color=FF3333&center=true&vCenter=true&width=820&lines=Building+autonomous+offensive+security;Shipping+AI-native+pentesting+%26+DFIR+tooling;Decoding+physiology+with+deep+learning;Automate+the+boring.+Hack+the+rest.)](https://github.com/Red-Snow)

[![Followers](https://img.shields.io/github/followers/Red-Snow?style=for-the-badge&logo=github&color=FF3333&labelColor=0d1117&label=FOLLOWERS)](https://github.com/Red-Snow?tab=followers)
[![Views](https://komarev.com/ghpvc/?username=Red-Snow&style=for-the-badge&color=FF3333&labelColor=0d1117&label=VIEWS)](https://github.com/Red-Snow)
[![Focus](https://img.shields.io/badge/FOCUS-AI%20%C3%97%20SECURITY-FF3333?style=for-the-badge&labelColor=0d1117)](https://github.com/Red-Snow?tab=repositories)

</div>

---

## Terminal

```python
class Operator:
    alias   = "Red-Snow"
    status  = "Active"
    domain  = ["Offensive Security", "AI Engineering", "Signal Processing"]

    focus = {
        "building"    : "PhantomStrike — AI-powered MCP pentesting framework",
        "shipping"    : "AI-Malware-Analyzer — browser-native DFIR platform",
        "researching" : "Conformer networks for physiological signal analysis",
        "exploring"   : "LLM tool-chaining for autonomous vulnerability discovery",
    }

    interests  = ["Red Teaming", "Deep Learning", "OSINT", "Steganalysis"]
    directives = ["Stay quiet", "Listen close", "Automate everything"]
```

> Operating at the intersection of **cybersecurity** and **artificial intelligence** — designing
> models that decode complex signals by day, building tools that let AI agents run autonomous
> penetration tests by night.

---

## Operations

<table>
<tr>
<td width="50%" valign="top">

### [PhantomStrike](https://github.com/Red-Snow/phantomstrike)

MCP server that hands any AI agent a full Kali toolchain — natural
language in, structured multi-step pentest out.

`Python` · `FastAPI` · `MCP` · `Docker`

[![Stars](https://img.shields.io/github/stars/Red-Snow/phantomstrike?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/Red-Snow/phantomstrike?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/phantomstrike/commits)

</td>
<td width="50%" valign="top">

### [AI-Malware-Analyzer](https://github.com/Red-Snow/AI-Malware-Analyzer)

100% client-side DFIR platform — PE parsing, IOC extraction,
MITRE ATT&CK mapping, PDF evidence reports.

`JavaScript` · `10+ LLM engines` · `Zero-backend`

[![Stars](https://img.shields.io/github/stars/Red-Snow/AI-Malware-Analyzer?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/AI-Malware-Analyzer/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/Red-Snow/AI-Malware-Analyzer?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/AI-Malware-Analyzer/commits)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [StegInsight-Forensics](https://github.com/Red-Snow/StegInsight-Forensics)

Steganography detection across text, image and audio/video
carriers, built for forensic triage.

`TypeScript` · `DSP` · `Entropy analysis`

[![Stars](https://img.shields.io/github/stars/Red-Snow/StegInsight-Forensics?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/StegInsight-Forensics/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/Red-Snow/StegInsight-Forensics?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/StegInsight-Forensics/commits)

</td>
<td width="50%" valign="top">

### [redsnow-recon-toolkit](https://github.com/Red-Snow/redsnow-recon-toolkit)

Browser-based recon and OSINT simulation lab with interactive
threat analysis and an AI cyber mentor.

`TypeScript` · `OSINT` · `LLM`

[![Stars](https://img.shields.io/github/stars/Red-Snow/redsnow-recon-toolkit?style=flat-square&logo=github&color=FF3333&labelColor=0d1117)](https://github.com/Red-Snow/redsnow-recon-toolkit/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/Red-Snow/redsnow-recon-toolkit?style=flat-square&color=FF3333&labelColor=0d1117&label=updated)](https://github.com/Red-Snow/redsnow-recon-toolkit/commits)

</td>
</tr>
</table>

---

## PhantomStrike — AI-Powered MCP Pentesting Framework

<div align="center">

> Connect **any MCP-compatible AI agent** to a full Kali Linux environment.<br/>
> Natural language → structured, multi-step penetration tests. No terminal switching. No manual chaining.

</div>

```text
 User   →  "Scan 192.168.1.1 for open ports, then audit all web services for SQLi."
 Agent  →  nmap (recon) → nikto (web audit) → sqlmap (injection) → structured report ✓
```

<table>
<tr>
<td width="50%" valign="top">

**Supported AI clients**
- Claude Desktop (macOS + Windows)
- Cursor IDE (all platforms)
- VS Code + GitHub Copilot
- Gemini CLI
- Any MCP-compatible agent

</td>
<td width="50%" valign="top">

**Key capabilities**
- 12 structured plugins — parsed JSON output
- `run_kali_shell` — any Kali command via AI
- All-in-Kali · Split (Host+VM) · Docker deploy
- Async job queue · SQLite scan history
- FastAPI backend · OpenAPI docs

</td>
</tr>
</table>

| Category | Tools |
|:--|:--|
| **Network** | `nmap` · `rustscan` · `masscan` |
| **Web App** | `nuclei` · `gobuster` · `sqlmap` · `ffuf` · `nikto` |
| **OSINT** | `subfinder` · `amass` |
| **Password** | `hydra` |
| **Cloud** | `trivy` |

<div align="center">

[![View PhantomStrike](https://img.shields.io/badge/→%20%20PhantomStrike%20on%20GitHub-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike)

</div>

---

## AI-Malware-Analyzer — Browser-Native Forensic Intelligence

<div align="center">

> A full DFIR workflow that never leaves the browser tab.<br/>
> Analyzes binaries, extracts IOCs, maps MITRE ATT&CK, and generates professional forensic reports.

</div>

```text
 User   →  Uploads a suspicious executable
 Agent  →  Strings / PE headers → family classification → MITRE mapping → VirusTotal → PDF report ✓
```

<table>
<tr>
<td width="50%" valign="top">

**Analysis engines**
- Google Gemini (Flash · Pro · Lite)
- OpenAI (GPT-4o · Turbo)
- Anthropic Claude (Opus · Sonnet · Haiku)
- Groq (Llama 3.3, ultra-fast)
- DeepSeek · xAI Grok · Mistral · Qwen

</td>
<td width="50%" valign="top">

**Key capabilities**
- 100% client-side — no server, no upload
- PE header parsing & entropy analysis
- Offline malware KB (25+ families)
- VirusTotal hash enrichment
- A4 PDF reports · chain-of-custody tracking

</td>
</tr>
</table>

<div align="center">

[![View AI Malware Analyzer](https://img.shields.io/badge/→%20%20AI%20Malware%20Analyzer%20on%20GitHub-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/AI-Malware-Analyzer)

</div>

---

## Arsenal

<div align="center">

**Security & Offensive**

![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=portswigger&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-214478?style=for-the-badge&logo=nmap&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C7192E?style=for-the-badge&labelColor=0d1117)

**AI & Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**Backend & Infrastructure**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**Agent Ecosystem**

![MCP](https://img.shields.io/badge/Model_Context_Protocol-6B46C1?style=for-the-badge&labelColor=0d1117)
![Claude](https://img.shields.io/badge/Claude-CC785C?style=for-the-badge&labelColor=0d1117)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

</div>

---

## Telemetry

<div align="center">

<img src="https://streak-stats.demolab.com?user=Red-Snow&theme=dark&background=0d1117&border=FF3333&ring=FF3333&fire=FF6666&currStreakLabel=FF3333&sideLabels=c9d1d9&dates=888888&currStreakNum=ffffff&sideNums=ffffff" width="70%"/>

</div>

---

## Signal Intelligence

<table>
<tr>
<td width="50%" valign="top">

### Physiological Deep Learning
Convolution-augmented Transformer (Conformer) architectures for physiological
signal processing and assessment.

- Automated signal decomposition
- Cross-validation on expansive datasets
- Hybrid neural network architectures

</td>
<td width="50%" valign="top">

### Agentic Security & Forensics
AI-native offensive security and forensic analysis platforms — from autonomous
recon to hidden-data detection.

- LLM tool-chaining for pentest workflows
- Natural-language execution layers
- Steganography detection across carriers

</td>
</tr>
</table>

---

<div align="center">

### Connect

[![GitHub](https://img.shields.io/badge/GitHub-Red--Snow-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow)
[![Open an Issue](https://img.shields.io/badge/Open%20an%20Issue-FF3333?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/Red-Snow/phantomstrike/issues)

<br/>

*"The quieter you become, the more you are able to hear."*

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:8B0000,100:FF0000&height=130&section=footer&animation=fadeIn" width="100%"/>

</div>
