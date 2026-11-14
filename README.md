# Awesome-Public-Private-API-Directory

# Awesome Public & Private API Directory

> A curated list of top Public and Private API Directory platforms — both SaaS/Hosted commercial API networks and open-source alternatives for discovering, cataloging, and governing APIs.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Postman API Network](#postman-api-network)
  - [RapidAPI](#rapidapi)
  - [APIs.guru](#apisguru)
  - [ProgrammableWeb](#programmableweb)
- [Open-Source Software](#-open-source-software)
  - [APIs.guru OpenAPI Directory](#apisguru-openapi-directory)
  - [Public APIs (public-apis)](#public-apis-public-apis)
  - [API Hub](#api-hub)
  - [Apinf](#apinf)
  - [Apivault](#apivault)
  - [openapi-directory-mcp](#openapi-directory-mcp)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Public and Private API Directory platforms. These are not open-source but are included as reference points for feature comparison.

### Postman API Network
**Type:** API discovery and collaboration within Postman ecosystem
Postman API Network is the public directory within the Postman platform, allowing developers to discover and explore APIs published by organizations. It integrates directly with Postman's API client, collections, and workspaces, making it the natural discovery layer for teams already using Postman for API development and testing.

### RapidAPI
**Type:** Commercial API marketplace and hub
RapidAPI is one of the largest commercial API marketplaces, connecting developers with thousands of APIs across categories. It provides a unified billing layer, API key management, and usage analytics. It is the primary commercial reference for API monetization and discovery, though it is entirely proprietary.

### APIs.guru
**Type:** Community-driven machine-readable API directory
APIs.guru provides a searchable directory of public API definitions in OpenAPI format, described as a "Wikipedia for Web APIs" [citation:9][citation:13]. It hosts **2,529 API descriptions** covering **108,837 endpoints**, with weekly updates and automatic conversion to OpenAPI 3.0 [citation:9]. All data is accessible via a REST API. While the directory itself is a hosted service, the underlying data is community-maintained and open [citation:4].

### ProgrammableWeb
**Type:** Legacy API directory and research resource
ProgrammableWeb is a long-standing directory of APIs, mashups, and SDKs, widely used for API research and discovery. It is a reference resource rather than an interactive platform, with a catalog that has been maintained for over a decade.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Public and Private API Directory tools. The open-source ecosystem spans **machine-readable API definition directories**, **curated public API lists**, **self-hosted OpenAPI portals**, and **AI-agent-accessible catalogs**.

### APIs.guru OpenAPI Directory
**Stack:** JavaScript / YAML / JSON | **License:** CC0-1.0 (data) [citation:3][citation:4]
The **openapi-directory** repository is the open-source data layer behind APIs.guru, containing a comprehensive collection of REST API definitions in OpenAPI 2.0/3.x format [citation:4]. Key characteristics:
- **4,533 GitHub stars** and **739 forks**, making it the most-starred open-source API directory [citation:3]
- **Community-driven**: anyone can add or change an API, not just the owner [citation:4]
- **Automated weekly updates** from original sources, with validation before commit [citation:4]
- **Machine-readable**: all data accessible through a REST API, discouraging direct GitHub raw links [citation:4]
- **Integrations**: used by HTTP Toolkit, Apideck, Microsoft Kiota, and others [citation:4]

**Best for:** Developers needing a comprehensive, machine-readable collection of OpenAPI definitions for code generation, testing, and API discovery.

### Public APIs (public-apis)
**Stack:** Markdown / GitHub | **License:** Open Source (MIT) [citation:5]
The **public-apis** repository is a collective list of free APIs, organized by category (Animals, Anime, Blockchain, Finance, Health, Music, News, Sports, Test Data, Text Analysis, and more) . It is one of the most popular open-source API directories, with a simple Markdown format that lists API name, description, authentication type (apiKey, OAuth, or none), HTTPS support, and CORS status . It is a **curated list** rather than a machine-readable directory or interactive portal.

**Best for:** Developers wanting a curated, human-readable list of free APIs for side projects and prototyping, particularly for discovering APIs with no authentication requirements.

### API Hub
**Stack:** TypeScript / Next.js / Docker | **License:** MIT [citation:1]
API Hub (dukex/api-hub) is a **simple OpenAPI discovery portal** for creating an elegant API portal from your OpenAPI specifications with minimal configuration [citation:1]. Key features:
- **API discovery**: searchable and filterable list of APIs by name, team, and metadata
- **Interactive documentation**: Swagger UI-powered API docs
- **AI-powered summaries**: automatic API summaries using Google Gemini (requires `GEMINI_API_KEY`)
- **Simple configuration**: just provide OpenAPI URLs and names in `specs/apis.json`

Deploys via Docker with a single command [citation:1].
**Best for:** Teams wanting a self-hosted, lightweight API portal for their internal or public OpenAPI specs, accepting a minimal configuration-driven approach.

### Apinf
**Stack:** JavaScript | **License:** Open Source [citation:8][citation:12]
Apinf is an **open-source API management platform** with multi-proxy and protocol support [citation:8]. It provides API catalog functionality alongside management capabilities. **Important:** The project was last pushed almost 3 years ago (as of the ecosystem data), so maintenance status should be verified before adoption [citation:8].

**Best for:** Teams exploring an older open-source API management platform with catalog features, accepting the maintenance risk.

### Apivault
**Stack:** (Check repository) | **License:** Open Source [citation:12]
Apivault is an open-source **directory and gateway for discovering public APIs**, cataloging thousands of free and public APIs across **51 categories** including animals, anime, blockchain, cryptocurrency, finance, health, music, news, and weather [citation:12]. It is an independent third-party profile by API Evangelist. It is actively maintained (updated October 2026) [citation:12].

**Best for:** Developers wanting a self-hosted or open directory with broad category coverage for public API discovery, accepting a younger project than APIs.guru.

### openapi-directory-mcp
**Stack:** TypeScript / MCP | **License:** Open Source 
openapi-directory-mcp exposes the APIs.guru directory to AI agents (Claude Code, Windsurf) through **22 MCP tools and prompts**, including API discovery, integration guide generation, code generation, auth implementation, and test suite creation . It also supports **importing custom OpenAPI specifications** as first-class citizens alongside the public directory, with security scanning and hierarchical storage . This bridges the gap between API directories and AI-assisted development workflows.

**Best for:** Developers using AI coding agents wanting direct access to the APIs.guru directory within their IDE or agent session, particularly for code generation and integration guidance.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Machine-Readable | Self-Hosted | AI/MCP | Best For |
|----------|---------|-------|------------------|-------------|--------|----------|
| **Postman API Network** | Proprietary | Cloud | (Postman format) | ❌ | ❌ | Postman ecosystem discovery |
| **RapidAPI** | Proprietary | Cloud | (Proprietary) | ❌ | ❌ | Commercial API marketplace |
| **APIs.guru (hosted)** | CC0 (data) | Cloud | ✅ OpenAPI | (Data) | ❌ | Machine-readable directory |
| **APIs.guru OpenAPI Directory** | CC0-1.0 | YAML/JSON | ✅ OpenAPI | ✅ (Data) | ❌ | 4,533-star OSS directory |
| **Public APIs** | MIT | Markdown | ❌ (Curated list) | ✅ | ❌ | Free API discovery |
| **API Hub** | MIT | TypeScript/Docker | ✅ OpenAPI | ✅ | ✅ Gemini | Self-hosted OpenAPI portal |
| **Apivault** | Open Source | (Check) | (Check) | ✅ | ❌ | 51-category public API directory |
| **openapi-directory-mcp** | Open Source | TypeScript/MCP | ✅ OpenAPI | ✅ (MCP) | ✅ MCP | AI-agent API discovery |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Public or Private API Directory tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem for **API directories** is **strongest for machine-readable OpenAPI collections**. **APIs.guru OpenAPI Directory** is the most established open-source directory with 4,533 stars and CC0 licensing, providing 2,529 API descriptions updated weekly [citation:3][citation:4]. **Public APIs** is the most accessible curated list for discovering free APIs . For self-hosted portals, **API Hub** offers a minimal MIT-licensed Docker deployment [citation:1], while **openapi-directory-mcp** uniquely bridges API discovery to AI coding agents via MCP .

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
