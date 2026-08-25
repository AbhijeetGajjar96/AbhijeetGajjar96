<a id="readme-top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0c0d10,50:164e63,100:22d3ee&height=160&section=header&text=Abhijeet%20Gajjar&fontColor=f4f4f5&fontSize=42&fontAlignY=32&desc=iOS%20%E2%86%92%20Full-Stack%20AI%20Engineer%20%C2%B7%20LA&descSize=15&descAlignY=55" alt="Banner" width="100%">

[![Portfolio][portfolio-shield]][portfolio-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
[![GitHub][github-shield]][github-url]
[![Email][email-shield]][email-url]
[![Resume][resume-shield]][resume-url]

<h1>Abhijeet Gajjar</h1>

<p>
  <strong>iOS engineer turned full-stack AI engineer.</strong>
  <br>
  I build backend services, LLM agent systems, and software that talks to physical devices.
  <br><br>
  📍 Artesia / Los Angeles, CA · ⏰ America/Los_Angeles · 📅 6 years · 🎓 M.S. Information Technology
</p>

<!-- Status: regenerate the date when you push an update -->
<p>
  <img src="https://img.shields.io/badge/Status-Open%20to%20work%20%C2%B7%20LA%20full--time-22d3ee?style=for-the-badge&logo=statuspage&logoColor=0c0d10" alt="Open to work">
  <img src="https://img.shields.io/badge/Last%20updated-2026--08--25%2014%3A01%20PDT-0c0d10?style=for-the-badge&logo=github&logoColor=22d3ee" alt="Last updated">
  <img src="https://img.shields.io/badge/Timezone-PDT%20(UTC--7)-71717a?style=for-the-badge&logo=clockify&logoColor=white" alt="Timezone">
</p>

<img src="https://komarev.com/ghpvc/?username=AbhijeetGajjar96&label=Profile%20views&color=22d3ee&style=flat" alt="Profile views">

</div>

<details open>
  <summary><strong>Table of Contents</strong></summary>
  <ol>
    <li><a href="#now">Now</a></li>
    <li><a href="#about-me">About Me</a></li>
    <li>
      <a href="#what-i-work-on">What I Work On</a>
      <ul>
        <li><a href="#on-device-inference">On-Device Inference</a></li>
        <li><a href="#llm-agents-in-production">LLM Agents in Production</a></li>
        <li><a href="#devices-and-low-level-integration">Devices &amp; Low-Level Integration</a></li>
        <li><a href="#debugging">Debugging</a></li>
      </ul>
    </li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#selected-work">Selected Work</a></li>
    <li><a href="#how-i-work">How I Work</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#agent-readable">Agent-Readable</a></li>
    <li><a href="#github-activity">GitHub Activity</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## Now

| | |
|---|---|
| **Looking for** | Full-time software / AI engineering roles in the **Los Angeles area** |
| **Available** | Yes — open to work |
| **Local time zone** | America/Los_Angeles (PDT / UTC−7 in summer) |
| **Last README refresh** | **2026-08-25 · 14:01 PDT** |
| **Current seat** | Full Stack Engineer, Pilot AI Labs (2026 – Present) |
| **Best intro** | Email or LinkedIn with a one-paragraph problem brief |

> Prefer a machine-readable résumé? Use the [agent endpoints](#agent-readable) below — same facts as [iabhijeetg.vercel.app/about](https://iabhijeetg.vercel.app/about).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## About Me

Six years across mobile and backend. I started in native iOS at an IT services firm building client applications, spent two years at a healthcare staffing startup as the direct technical contact for customers and the founder, delivered enterprise IoT engagements across four clients, then moved into backend systems and AI.

The through-line is that I like being close to two things: the customer, and the hardware. Most of my best work has come from being in the room when a problem was described, or close enough to the metal to know why something was slow.

| At a glance | |
|---|---|
| Full name | Abhijeet Gajjar |
| Based | Artesia, CA · Los Angeles area |
| Role | Software Engineer · Backend · Devices · On-device AI |
| Years | 6 (mobile → backend → devices / AI) |
| Portfolio | [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app) |
| About / CV | [iabhijeetg.vercel.app/about](https://iabhijeetg.vercel.app/about) |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## What I Work On

### On-Device Inference

Getting models to run where the data already is. I convert trained models to Core ML, quantize them to fit mobile memory and compute budgets, and measure what the compression actually costs in accuracy. Shipped real-time computer vision at **30fps on iOS**, and replaced a hosted inference pipeline with a local one — removing per-request server cost and network dependency from the critical path.

The interesting constraint is that mobile hardware doesn't forgive. A model that runs fine on a GPU will thermal-throttle a phone into unusability. Most of the work is deciding what to give up.

### LLM Agents in Production

Two years building Python and FastAPI microservices that decompose natural-language requests into executed tasks, using **LangChain and LangGraph** for agent orchestration. Cut manual processing overhead **40%** in a live business workflow.

The demo was never the hard part. The hard part was scoping — early on I let the agent handle steps that were fully deterministic, which made the system slower, more expensive, and less predictable than plain code. Pulling those back and reserving the model for genuinely ambiguous interpretation is what made it reliable.

Second hardest: knowing *why* a run failed. Reading logs and inferring intent is not observability.

### Devices and Low-Level Integration

BLE peripheral discovery and connection management, live sensor telemetry, and offline persistence that reconciles buffered state automatically after connectivity loss. Delivered to **two enterprise clients** across iOS and Android.

Hardware prototyping on **Raspberry Pi and Texas Instruments** boards — interfacing sensors and peripherals over GPIO, I2C, SPI, UART/serial, and USB, processing device data in Python on embedded Linux.

### Debugging

The part of the job I actually enjoy. Unexpected failures in live systems are the most interesting problem in software, because the answer is always somewhere you didn't think to look.

| Metric | Result |
|---|---|
| Critical runtime defects root-caused | **50+** |
| Crash-rate reduction via TDD | **70%** |
| Crash-rate reduction across 10+ apps | **20%** |
| System stability improvement | **50%** |
| Downtime through scaling events | **Zero** |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Built With

[![Swift][swift-shield]][swift-url]
[![Python][python-shield]][python-url]
[![TypeScript][ts-shield]][ts-url]
[![FastAPI][fastapi-shield]][fastapi-url]
[![PyTorch][pytorch-shield]][pytorch-url]
[![LangChain][langchain-shield]][langchain-url]
[![Core ML][coreml-shield]][coreml-url]
[![Docker][docker-shield]][docker-url]
[![PostgreSQL][pg-shield]][pg-url]
[![AWS][aws-shield]][aws-url]
[![Azure][azure-shield]][azure-url]
[![Bluetooth][ble-shield]][ble-url]

```
Languages    Swift · Objective-C · Python · TypeScript · Java · Kotlin · C++ · SQL · Bash
AI / ML      LangChain · LangGraph · PyTorch · TensorFlow · Core ML · RAG · Vector DBs
             Prompt engineering · Fine-tuning · Quantization · On-device inference
Backend      FastAPI · Flask · Django · Spring Boot · Node.js · REST · GraphQL · WebSockets
Cloud        AWS (Lambda, S3, API Gateway) · Azure · GCP · Docker · Kubernetes · CI/CD
Data         PostgreSQL · SQLite · Redis · MongoDB · Snowflake · Azure Data Pipelines
Apple        UIKit · SwiftUI · Core Data · Core Bluetooth · Core ML · Vision · XCTest
Devices      BLE · Raspberry Pi · Texas Instruments · GPIO · I2C · SPI · UART · USB
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Experience

| Period | Role | Focus |
|---|---|---|
| **2026 –** | Full Stack Engineer, Pilot AI Labs | Zero-to-one product, on-device Core ML, payments and vendor API integration |
| **2024 – 26** | Software Engineer, Propbase | LLM agent microservices, Azure infrastructure, data pipelines |
| **2022 – 23** | Software Engineer, Cygnet Infotech | Enterprise IoT, reusable Swift architecture across four clients |
| **2020 – 22** | iOS Developer, BeLocum | Healthcare staffing platform, Objective-C → Swift migration, ML computer vision |
| **2019 – 20** | Junior iOS Developer, Ecosmob | 10+ production iOS apps, test suites, REST integration |

<details>
<summary><strong>A migration I'm proud of</strong></summary>

<br>

At BeLocum I replaced a legacy Objective-C codebase with a Swift implementation **without disrupting users** — bridging modules incrementally while the product stayed in continuous release. Runtime efficiency improved 20%, and the platform supported a launch reaching 100,000+ registrations and 10,000 daily active users.

Rewrites that stop the world are easy to plan and hard to survive. Doing it module by module, under live traffic, with both languages coexisting, is slower and considerably less glamorous — and it's the only version that actually ships.

</details>

<details>
<summary><strong>What I'm doing now (Pilot AI Labs)</strong></summary>

<br>

Shipped a production commerce application from zero to release in one month against a serverless AWS Lambda backend. Integrated Stripe and the 3DLOOK body-measurement API behind REST endpoints with webhook handling. Prototyped on-device Core ML inference to remove per-request hosting cost.

</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Selected Work

| | Project | Description | Stack |
|---|---|---|---|
| 📡 | **Bluetooth IoT Sensor Dashboard** | Cross-platform device monitoring delivered to two enterprise clients. Peripheral discovery, live telemetry, offline persistence, automatic state reconciliation on reconnect. | Swift · Kotlin · Core Bluetooth · SQLite |
| 👁️ | **Real-Time ML Object Detection** | End-to-end computer vision pipeline converted to Core ML for on-device inference at 30fps, with quantization tuned to hardware constraints. | PyTorch · TensorFlow · Core ML |
| 🔌 | **Embedded Sensor Prototyping** | Hardware prototypes on Raspberry Pi and TI boards, interfacing sensors over GPIO, I2C, SPI, UART/serial, and USB. | Python · Embedded Linux |
| 🏠 | **Dwelio** | Solo end-to-end AI property maintenance — request intake, vendor sourcing, bidding, completion. Live on web + TestFlight + Play. | FastAPI · PostgreSQL · OpenAI · React Native · AWS |

More live apps and notes: [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app) · [Selected work JSON](https://iabhijeetg.vercel.app/api/projects)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## How I Work

**Test-driven where it counts.** TDD with XCTest is how I got crash rates down 70% — not by writing tests after the fact.

**AI tooling, deliberately.** I code mostly in Cursor and keep a markdown file in each repo describing architecture, conventions, and the current task, so I feed a compact written summary instead of re-explaining the codebase every session. Cheaper in tokens and more consistent in output, because the model works from stated constraints rather than whatever it inferred from recent files.

I don't merge generated code I couldn't defend in review. It's strongest on scaffolding, tests, and unfamiliar APIs; weakest on business logic I haven't fully specified — which usually means my requirements were vague, not that the model failed.

**Close to the customer.** At BeLocum I ran discovery on live problems directly with customers and the founder, then came back with two or three implementation approaches and their tradeoffs so they could choose against their own priorities.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Roadmap

- [x] Production LLM agent systems with LangChain and LangGraph
- [x] On-device inference with Core ML and model quantization
- [x] BLE device integration with offline state reconciliation
- [x] Public agent-ready portfolio (`/api/resume`, `/api/projects`, `/llms.txt`)
- [ ] MCP servers with evaluation harnesses running in CI
- [ ] Diffusion models for computer vision
- [ ] On-device LLM inference on constrained hardware

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Education

**M.S. Information Technology** — Westcliff University, Irvine, CA · 2025 · GPA 4.0

**B.E. Information Technology** — Gujarat Technological University, India · 2017

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Agent-Readable

Same source of truth as the site — no scraping required.

| Method | Endpoint | What you get |
|---|---|---|
| `GET` | https://iabhijeetg.vercel.app/api/resume | Structured résumé JSON |
| `GET` | https://iabhijeetg.vercel.app/api/projects | Selected work records |
| `GET` | https://iabhijeetg.vercel.app/llms.txt | Plain-language hire brief |
| `POST` | https://iabhijeetg.vercel.app/api/hire | Book an intro (`name`, `contact`, `brief`) |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## GitHub Activity

Commit calendar and profile cards for [@AbhijeetGajjar96](https://github.com/AbhijeetGajjar96).

<p align="center">
  <img src="https://ghchart.rshah.org/22d3ee/AbhijeetGajjar96" alt="GitHub contribution calendar" width="100%">
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=AbhijeetGajjar96&theme=github_dark" alt="Profile details" width="100%">
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=AbhijeetGajjar96&theme=github_dark" height="180" alt="GitHub stats">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=AbhijeetGajjar96&theme=github_dark" height="180" alt="Repos per language">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=AbhijeetGajjar96&theme=github_dark" height="180" alt="Most commit language">
</p>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

**Abhijeet Gajjar** — open to work in Los Angeles · reply within a day or two when I can

- Email: [gajjarabhijeet@gmail.com](mailto:gajjarabhijeet@gmail.com)
- Phone: [(562) 215-3250](tel:+15622153250)
- LinkedIn: [linkedin.com/in/abhijeetgajjar](https://www.linkedin.com/in/abhijeetgajjar/)
- Portfolio: [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0c0d10,100:22d3ee&height=100&section=footer" width="100%" alt="">

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- Shields -->
[portfolio-shield]: https://img.shields.io/badge/-Portfolio-22d3ee.svg?style=for-the-badge&logo=googlechrome&logoColor=0c0d10
[portfolio-url]: https://iabhijeetg.vercel.app
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-0A66C2.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url]: https://www.linkedin.com/in/abhijeetgajjar/
[github-shield]: https://img.shields.io/badge/-GitHub-181717.svg?style=for-the-badge&logo=github&logoColor=white
[github-url]: https://github.com/AbhijeetGajjar96
[email-shield]: https://img.shields.io/badge/-Email-EA4335.svg?style=for-the-badge&logo=gmail&logoColor=white
[email-url]: mailto:gajjarabhijeet@gmail.com
[resume-shield]: https://img.shields.io/badge/-Resume-0c0d10.svg?style=for-the-badge&logo=adobeacrobatreader&logoColor=22d3ee
[resume-url]: https://iabhijeetg.vercel.app/about
[swift-shield]: https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white
[swift-url]: https://swift.org
[python-shield]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[python-url]: https://python.org
[ts-shield]: https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white
[ts-url]: https://typescriptlang.org
[fastapi-shield]: https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white
[fastapi-url]: https://fastapi.tiangolo.com
[pytorch-shield]: https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white
[pytorch-url]: https://pytorch.org
[langchain-shield]: https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white
[langchain-url]: https://www.langchain.com
[coreml-shield]: https://img.shields.io/badge/Core%20ML-000000?style=for-the-badge&logo=apple&logoColor=white
[coreml-url]: https://developer.apple.com/documentation/coreml
[docker-shield]: https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
[docker-url]: https://docker.com
[pg-shield]: https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white
[pg-url]: https://postgresql.org
[aws-shield]: https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white
[aws-url]: https://aws.amazon.com
[azure-shield]: https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white
[azure-url]: https://azure.microsoft.com
[ble-shield]: https://img.shields.io/badge/Bluetooth%20LE-0082FC?style=for-the-badge&logo=bluetooth&logoColor=white
[ble-url]: https://www.bluetooth.com

<!--
  IMAGES — optional project thumbs
  1. Add images/ble-thumb.png, images/ml-thumb.png, images/embedded-thumb.png
  2. Or paste GitHub user-attachments CDN URLs from an issue draft
  3. Keep under 200KB each
-->
