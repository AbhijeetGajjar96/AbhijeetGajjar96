<a id="readme-top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0c0d10,50:164e63,100:22d3ee&height=160&section=header&text=Abhijeet%20Gajjar&fontColor=f4f4f5&fontSize=42&fontAlignY=32&desc=Software%20Engineer%20%C2%B7%20Backend%20%C2%B7%20Devices%20%C2%B7%20On-Device%20AI&descSize=14&descAlignY=55" alt="Banner" width="100%">

[![Portfolio][portfolio-shield]][portfolio-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
[![GitHub][github-shield]][github-url]
[![Email][email-shield]][email-url]
[![Resume][resume-shield]][resume-url]

</div>

<div align="center">

**Software engineer with six years of experience across backend systems, device integration, and on-device AI.**

Seeking backend or ML engineering roles in Los Angeles &middot; open to hybrid and on-site

<br>

<img src="https://img.shields.io/badge/Available-Full--time%20%C2%B7%20Los%20Angeles-22d3ee?style=for-the-badge&logo=statuspage&logoColor=0c0d10" alt="Available">
<img src="https://img.shields.io/badge/Updated-2026--09--01-0c0d10?style=for-the-badge&logo=github&logoColor=22d3ee" alt="Last updated">

<br><br>

<img src="https://komarev.com/ghpvc/?username=AbhijeetGajjar96&label=Profile%20views&color=22d3ee&style=flat" alt="Profile views">

</div>

---

### Contents

[About](#about) &middot; [Technical Focus](#technical-focus) &middot; [Technology](#technology) &middot; [Experience](#experience) &middot; [Selected Work](#selected-work) &middot; [Education](#education) &middot; [Machine-Readable Endpoints](#machine-readable-endpoints) &middot; [Contact](#contact)

---

## About

| | |
|---|---|
| **Name** | Abhijeet Gajjar |
| **Location** | Artesia, CA (Los Angeles area) |
| **Current role** | Full Stack Engineer, Pilot AI Labs |
| **Experience** | 6 years &mdash; mobile, backend, device integration, AI |
| **Seeking** | Backend engineering, ML engineering, or full-stack roles (hybrid / on-site in LA) |
| **Portfolio** | [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app) |
| **Full CV** | [iabhijeetg.vercel.app/about](https://iabhijeetg.vercel.app/about) |

I began in native iOS development and progressed through backend systems, embedded device integration, and AI engineering. The strongest proof of that trajectory is [Dwelio](https://www.dwelio.app/), a property maintenance platform I designed and delivered independently &mdash; from data model and FastAPI backend through OpenAI agent workflows to released React Native applications on iOS and Android. No team, no handoff; one engineer across every layer.

Across each stage of my career, the common thread has been working close to the end user and close to the hardware, where constraints are concrete and the feedback loop is short.

<p align="right"><a href="#readme-top">top</a></p>

## Technical Focus

### On-Device Inference

Conversion of trained models to Core ML with quantization tuned to mobile memory and compute constraints. Delivered real-time computer vision at **30 fps on iOS** (down from ~8 fps before INT8 quantization) and replaced a hosted inference pipeline with a local one, eliminating per-request server cost and network dependency.

The key architectural decision was choosing INT8 over INT4 quantization: INT4 saved more memory but introduced enough accuracy loss that the object-detection confidence threshold had to drop below a usable level. INT8 kept accuracy within 2% of the float32 baseline while fitting comfortably in the device's memory budget.

### Production Agent Systems

Two years developing Python and FastAPI microservices that decompose natural-language requests into executed tasks using **LangChain and LangGraph** for orchestration. Reduced manual processing overhead by **40%** in a production workflow handling ~200 daily maintenance requests at Propbase.

Early on I let the agent handle steps that were fully deterministic, which made the system slower, more expensive, and less predictable than plain code. Pulling those back and reserving the model for genuinely ambiguous interpretation &mdash; routing intent, not executing known procedures &mdash; is what made the pipeline reliable enough for production traffic.

### Device Integration

BLE peripheral discovery, live sensor telemetry, and offline persistence with automatic state reconciliation after connectivity loss. Delivered cross-platform solutions to **two enterprise clients** at Cygnet Infotech (iOS and Android). Hands-on prototyping with **Raspberry Pi and Texas Instruments** boards over GPIO, I2C, SPI, UART, and USB.

### Quality Engineering

| Metric | Context | Result |
|---|---|---|
| Critical runtime defects resolved | BeLocum &mdash; 2 years, healthcare staffing platform with 100K+ registrations and 10K DAU | **50+** |
| Crash-rate reduction via TDD | Cygnet Infotech &mdash; introduced XCTest across four enterprise IoT client apps | **70%** (from ~12% session crash rate) |
| Crash-rate reduction across applications | Ecosmob &mdash; 18+ production iOS apps over one year | **20%** |
| System stability improvement | BeLocum &mdash; measured via crash-free sessions after systematic log triage | **+50%** |
| Downtime through scaling events | Propbase &mdash; Azure-hosted REST APIs under growing B2B load | **Zero** |

<p align="right"><a href="#readme-top">top</a></p>

## Technology

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

<details>
<summary><strong>Full technology inventory</strong></summary>
<br>

| Category | Tools |
|---|---|
| **Languages** | Swift, Objective-C, Python, TypeScript, Java, Kotlin, C++, SQL, Bash |
| **AI / ML** | LangChain, LangGraph, PyTorch, TensorFlow, Core ML, RAG, vector databases, quantization |
| **Backend** | FastAPI, Flask, Django, Spring Boot, Node.js, REST, GraphQL, WebSockets |
| **Cloud** | AWS (Lambda, S3, API Gateway), Azure, GCP, Docker, Kubernetes, CI/CD |
| **Data** | PostgreSQL, SQLite, Redis, MongoDB, Snowflake, Azure Data Pipelines |
| **Apple** | UIKit, SwiftUI, Core Data, Core Bluetooth, Core ML, Vision, XCTest |
| **Devices** | BLE, Raspberry Pi, Texas Instruments, GPIO, I2C, SPI, UART, USB |

</details>

<p align="right"><a href="#readme-top">top</a></p>

## Experience

| Period | Role | Organization | Focus |
|---|---|---|---|
| 2026 &ndash; present | Full Stack Engineer | Pilot AI Labs | Zero-to-one product in one month, on-device Core ML, Stripe and 3DLOOK API integration |
| 2024 &ndash; 2026 | Software Engineer | Propbase LLC | LLM agent microservices (40% overhead reduction), Azure infrastructure, automated data pipelines |
| 2022 &ndash; 2023 | Software Engineer | Cygnet Infotech | Enterprise IoT for four clients, reusable Swift architecture, 70% crash-rate reduction via TDD |
| 2020 &ndash; 2022 | Software Engineer | BeLocum | Healthcare platform (100K+ registrations, 10K DAU), Obj-C &rarr; Swift migration, ML computer vision |
| 2019 &ndash; 2020 | Software Engineer | Ecosmob Technologies | 18+ production iOS apps, test suites, 20% crash-rate reduction |

<details>
<summary><strong>Pilot AI Labs (current)</strong></summary>
<br>

Delivered a production commerce application from initial concept to release within one month using a serverless AWS Lambda backend. Integrated Stripe payment processing and the 3DLOOK body-measurement API behind REST endpoints with webhook handling. Prototyped on-device Core ML inference to eliminate per-request hosting costs.

</details>

<details>
<summary><strong>BeLocum &mdash; incremental migration</strong></summary>
<br>

Replaced a legacy Objective-C codebase with Swift through incremental module bridging while the product remained in continuous release. Runtime efficiency improved by 20%, and the platform supported a launch reaching 100,000+ registrations and 10,000 daily active users.

</details>

<p align="right"><a href="#readme-top">top</a></p>

## Selected Work

| Project | Description | Technology | Links |
|---|---|---|---|
| **Dwelio** | AI property maintenance platform &mdash; delivered solo from data model to production. Automated request intake, vendor sourcing and negotiation, bidding, and completion. One engineer across backend, agent, and mobile. | FastAPI, PostgreSQL, OpenAI, React Native, AWS | [Web](https://www.dwelio.app/) |
| **Real-Time ML Object Detection** | End-to-end computer vision pipeline: PyTorch &rarr; TensorFlow &rarr; Core ML, INT8 quantized for 30 fps on-device inference. | PyTorch, TensorFlow, Core ML | [GitHub](https://github.com/AbhijeetGajjar96) |
| **Bluetooth IoT Sensor Dashboard** | Cross-platform device monitoring for two enterprise clients. BLE peripheral discovery, live telemetry, offline persistence, automatic state reconciliation on reconnect. | Swift, Kotlin, Core Bluetooth, SQLite | &mdash; |
| **Embedded Sensor Prototyping** | Functional prototypes on Raspberry Pi and TI boards, interfacing sensors over GPIO, I2C, SPI, UART, and USB. | Python, Embedded Linux | [GitHub](https://github.com/AbhijeetGajjar96) |
| **iCyclop** | AI pill counting via computer vision, PyTorch &rarr; Core ML. | PyTorch, Core ML, Swift | [App Store](https://apps.apple.com/ca/app/icyclop/id1621270285) |
| **BeLocum** | Healthcare staffing marketplace &mdash; 100K+ registrations, 10K DAU. Led Obj-C &rarr; Swift migration. | Swift, PyTorch, TensorFlow | [App Store](https://apps.apple.com/ca/app/belocum/id1263903693) |

More projects and live apps: [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app) &middot; [Projects JSON](https://iabhijeetg.vercel.app/api/projects)

<p align="right"><a href="#readme-top">top</a></p>

## Education

| Degree | Institution | Year | Detail |
|---|---|---|---|
| **M.S. Information Technology** | Westcliff University, Irvine, CA | 2025 | GPA 4.0 |
| **B.E. Information Technology** | Gujarat Technological University, India | 2017 | |

<p align="right"><a href="#readme-top">top</a></p>

## Machine-Readable Endpoints

Structured data for automated evaluation. No scraping required.

| Method | Endpoint | Description |
|---|---|---|
| `GET` | [`/api/resume`](https://iabhijeetg.vercel.app/api/resume) | Structured r&eacute;sum&eacute; as JSON |
| `GET` | [`/api/projects`](https://iabhijeetg.vercel.app/api/projects) | Selected work records |
| `GET` | [`/llms.txt`](https://iabhijeetg.vercel.app/llms.txt) | Plain-language summary for AI agents |

<p align="right"><a href="#readme-top">top</a></p>

## Roadmap

- [x] Production LLM agent systems with LangChain and LangGraph
- [x] On-device inference with Core ML and model quantization
- [x] BLE device integration with offline state reconciliation
- [x] Agent-ready portfolio with structured API endpoints
- [ ] Build an MCP server for device telemetry with an evaluation harness running in CI
- [ ] Run a quantized 7B language model on an M-series Mac Mini as a local API replacement

<p align="right"><a href="#readme-top">top</a></p>

## Contact

| | |
|---|---|
| **Email** | [gajjarabhijeet@gmail.com](mailto:gajjarabhijeet@gmail.com) |
| **LinkedIn** | [linkedin.com/in/abhijeetgajjar](https://www.linkedin.com/in/abhijeetgajjar/) |
| **Portfolio** | [iabhijeetg.vercel.app](https://iabhijeetg.vercel.app) |

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0c0d10,100:22d3ee&height=100&section=footer" width="100%" alt="">

<p align="right"><a href="#readme-top">top</a></p>

<!-- Shields -->
[portfolio-shield]: https://img.shields.io/badge/-Portfolio-22d3ee.svg?style=for-the-badge&logo=googlechrome&logoColor=0c0d10
[portfolio-url]: https://iabhijeetg.vercel.app
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-0A66C2.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url]: https://www.linkedin.com/in/abhijeetgajjar/
[github-shield]: https://img.shields.io/badge/-GitHub-181717.svg?style=for-the-badge&logo=github&logoColor=white
[github-url]: https://github.com/AbhijeetGajjar96
[email-shield]: https://img.shields.io/badge/-Email-EA4335.svg?style=for-the-badge&logo=gmail&logoColor=white
[email-url]: mailto:gajjarabhijeet@gmail.com
[resume-shield]: https://img.shields.io/badge/-R%C3%A9sum%C3%A9-0c0d10.svg?style=for-the-badge&logo=adobeacrobatreader&logoColor=22d3ee
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
