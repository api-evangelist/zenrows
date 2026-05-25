# ZenRows

ZenRows is a Spanish web scraping platform headquartered in Madrid that lets developers collect public web data at scale without managing proxies, browsers, or CAPTCHAs. A single API key unlocks four products against a shared pool of 55M+ residential IPs across 190+ countries: the **Universal Scraper API** (HTTP scrape with JS rendering, anti-bot bypass, screenshots, CSS/AI extraction, PDF/markdown output), the **Scraping Browser** (cloud Playwright/Puppeteer/CDP browser over WebSocket), **Residential Proxies** (HTTP/SOCKS5 with sticky sessions and country targeting), and a set of vertical **Scraper APIs** for Amazon, Google, Walmart, Zillow, and Idealista. ZenRows also ships first-party Python, Node.js, and Go SDKs, a Scrapy middleware, deep integrations across Playwright, Puppeteer, Selenium, Scrapy, LangChain, LlamaIndex, OpenAI Agents SDK, Zapier, n8n, Make, Pipedream, Node-RED, MuleSoft, Clay, and an official MCP server (`@zenrows/mcp` on npm and hosted at `https://mcp.zenrows.com/mcp`) exposing scrape and 30+ browser automation tools to AI agents like Anthropic Claude.

**Human URL:** https://www.zenrows.com/
**Developer Documentation:** https://docs.zenrows.com/
**APIs.yml:** https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/apis.yml

## Scope

- **Type:** Provider
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Web Scraping
- Data Extraction
- Anti-Bot
- Proxies
- Residential Proxies
- Browser Automation
- Screenshots
- CAPTCHA
- AI
- MCP
- Spain

## APIs

| API | Description |
|-----|-------------|
| [Universal Scraper API](https://docs.zenrows.com/universal-scraper-api/api-reference) | HTTP scrape at `api.zenrows.com/v1/` with JS rendering, anti-bot, premium proxy, extraction, screenshots, markdown/PDF/JSON |
| [Scraping Browser](https://docs.zenrows.com/scraping-browser/introduction) | Cloud Playwright/Puppeteer/CDP browser over `wss://browser.zenrows.com` |
| [Residential Proxies](https://docs.zenrows.com/residential-proxies/introduction) | HTTP/SOCKS5 residential proxy with country targeting and sticky sessions |
| [Scraper APIs](https://docs.zenrows.com/scraper-apis/introduction) | Structured-data scrapers for Amazon, Google, Walmart, Zillow, Idealista |
| [MCP Server](https://docs.zenrows.com/integrations/mcp/mcp-overview) | Official ZenRows MCP server (`@zenrows/mcp`) for AI agents |
| [SDKs](https://github.com/ZenRows) | Python, Node.js, Go, browser, and Scrapy middleware |

## Artifacts

### OpenAPI Specifications

| File | Description |
|------|-------------|
| [openapi/zenrows-universal-scraper-openapi.yml](openapi/zenrows-universal-scraper-openapi.yml) | ZenRows Universal Scraper API (GET and POST scrape) |

### Spectral Rules

| File | Description |
|------|-------------|
| [rules/zenrows-rules.yml](rules/zenrows-rules.yml) | ZenRows API conventions and linting ruleset |

### Capabilities

| File | Description |
|------|-------------|
| [capabilities/universal-scraper.yaml](capabilities/universal-scraper.yaml) | Naftiko capability for the Universal Scraper API (HTTP + REST + MCP) |

### JSON Schema

| File | Description |
|------|-------------|
| [json-schema/zenrows-scrape-response-schema.json](json-schema/zenrows-scrape-response-schema.json) | Schema for the Universal Scraper API JSON response envelope |

### JSON Structure

| File | Description |
|------|-------------|
| [json-structure/zenrows-scrape-request-structure.json](json-structure/zenrows-scrape-request-structure.json) | Structural map of every Universal Scraper API query parameter |

### JSON-LD

| File | Description |
|------|-------------|
| [json-ld/zenrows-context.jsonld](json-ld/zenrows-context.jsonld) | JSON-LD context for ZenRows scrape, browser, and proxy vocabulary |

### Examples

| File | Description |
|------|-------------|
| [examples/zenrows-scrape-url-example.json](examples/zenrows-scrape-url-example.json) | End-to-end scrape with JS rendering, premium proxy, CSS extractor, JSON response |

### Vocabulary

| File | Description |
|------|-------------|
| [vocabulary/zenrows-vocabulary.yml](vocabulary/zenrows-vocabulary.yml) | Web scraping domain vocabulary and taxonomy |

### Plans, Rate Limits, FinOps

| File | Description |
|------|-------------|
| [plans/zenrows-plans-pricing.yml](plans/zenrows-plans-pricing.yml) | API Commons Plans 0.1 — Free Trial through Enterprise plus Scraping Browser metered add-on |
| [rate-limits/zenrows-rate-limits.yml](rate-limits/zenrows-rate-limits.yml) | API Commons Rate Limits 0.1 — plan concurrency caps and feature budgets |
| [finops/zenrows-finops.yml](finops/zenrows-finops.yml) | FOCUS 1.3-aligned FinOps shape for ZenRows subscription + Scraping Browser metered usage |

## Links

- **Website:** https://www.zenrows.com/
- **Documentation:** https://docs.zenrows.com/
- **GitHub Org:** https://github.com/ZenRows
- **Pricing:** https://www.zenrows.com/pricing
- **Status:** https://status.zenrows.com/
- **Changelog:** https://eu.intercom.news/zenrows
- **Blog:** https://www.zenrows.com/blog
- **Error Codes:** https://docs.zenrows.com/api-error-codes
- **LLMs.txt:** https://docs.zenrows.com/llms.txt

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
