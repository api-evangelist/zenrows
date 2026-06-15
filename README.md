# ZenRows (zenrows)

ZenRows is a Spanish web scraping platform headquartered in Madrid that lets developers collect public web data at scale without managing proxies, browsers, or CAPTCHAs. A single API key unlocks four products against a shared 55M+ residential IP pool across 190+ countries: the Universal Scraper API (HTTP scrape with JS rendering, anti-bot bypass, screenshots, CSS/AI extraction, and PDF/markdown output), the Scraping Browser (cloud Playwright/Puppeteer/CDP browser over WebSocket), Residential Proxies (HTTP/SOCKS5 with sticky sessions and country targeting), and a set of vertical Scraper APIs for Amazon, Google, Walmart, Zillow, and Idealista. ZenRows also ships first-party Python, Node.js, and Go SDKs, a Scrapy middleware, deep integrations across Playwright, Puppeteer, Selenium, Scrapy, LangChain, LlamaIndex, OpenAI Agents SDK, Zapier, n8n, Make, Pipedream, Node-RED, MuleSoft, Clay, and an official MCP server (hosted at https://mcp.zenrows.com/mcp and as @zenrows/mcp on npm) exposing scrape and 30+ browser automation tools to AI agents.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/apis.yml)

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

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### ZenRows Universal Scraper API

HTTP scraping API at https://api.zenrows.com/v1/ that fetches any URL with optional JavaScript rendering, anti-bot bypass via Adaptive Stealth Mode, premium residential proxies, country-level geo-targeting, session pinning (up to 10 minutes), custom headers, CSS extractors, AI autoparse, wait/wait_for synchronization, JavaScript instructions, full-page or element screenshots (PNG/JPEG), and output conversion to markdown, plaintext, or PDF. Authentication is by apikey query parameter. Response headers expose Concurrency-Limit, Concurrency-Remaining, X-Request-Cost, X-Request-Id, and Zr-Final-Url for cost and observability.

- **Human URL:** [https://docs.zenrows.com/universal-scraper-api/api-reference](https://docs.zenrows.com/universal-scraper-api/api-reference)

#### Tags

- Web Scraping
- Anti-Bot
- JavaScript Rendering
- Screenshots
- Data Extraction
- AI

#### Properties

- [Documentation](https://docs.zenrows.com/universal-scraper-api/api-reference)
- [Documentation](https://docs.zenrows.com/universal-scraper-api/first-request)
- [Sign Up](https://app.zenrows.com/register)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/openapi/zenrows-universal-scraper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Spectral Rules](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/rules/zenrows-rules.yml)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/json-schema/zenrows-scrape-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/json-structure/zenrows-scrape-request-structure.json)
- [J S O N L D Context](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/json-ld/zenrows-context.jsonld)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ZenRows Scraping Browser

Cloud headless browser exposed over WebSocket at wss://browser.zenrows.com?apikey=KEY, compatible with Playwright, Puppeteer, and the underlying Chrome DevTools Protocol. Each session runs on the ZenRows infrastructure with automatic rotation across 55M+ residential IPs in 190+ countries, country and world-region targeting, configurable session TTL, and 99.9% uptime. Billed per session-hour ($0.09/hr in 30-second increments) plus per-GB bandwidth (from $5.50/GB, discounted to $2.80/GB at Enterprise). Suited to single-page apps, complex user flows, and long-running interactive scraping.

- **Human URL:** [https://docs.zenrows.com/scraping-browser/introduction](https://docs.zenrows.com/scraping-browser/introduction)

#### Tags

- Browser Automation
- Playwright
- Puppeteer
- CDP
- Residential Proxies
- WebSocket

#### Properties

- [Documentation](https://docs.zenrows.com/scraping-browser/introduction)
- [Documentation](https://docs.zenrows.com/scraping-browser/scraping-browser-setup)
- [Documentation](https://docs.zenrows.com/scraping-browser/get-started/playwright)
- [Documentation](https://docs.zenrows.com/scraping-browser/get-started/puppeteer)
- [F A Q](https://docs.zenrows.com/scraping-browser/faq)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ZenRows Residential Proxies

HTTP and SOCKS5 residential proxy network with 55M+ IPs across 190+ countries, username/password authentication, country and world-region targeting (e.g. country-es for Spain), and sticky-session TTL configurable from 30 seconds up to 1 day. Sold by bandwidth rather than request count; intended as a drop-in proxy for any HTTP client, browser, or scraping framework.

- **Human URL:** [https://docs.zenrows.com/residential-proxies/introduction](https://docs.zenrows.com/residential-proxies/introduction)

#### Tags

- Proxies
- Residential Proxies
- HTTP
- SOCKS5
- Geo-Targeting

#### Properties

- [Documentation](https://docs.zenrows.com/residential-proxies/introduction)
- [Documentation](https://docs.zenrows.com/residential-proxies/residential-proxies-setup)
- [Documentation](https://docs.zenrows.com/residential-proxies/get-started/first-request)
- [F A Q](https://docs.zenrows.com/residential-proxies/faq)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ZenRows Scraper APIs

Vertical, structured-data scraper endpoints for major commerce and real-estate sites, sharing the api.zenrows.com authentication and credit model. Covers Amazon (ASIN lookup, discovery), Google (search results), Walmart (discovery, product information, product reviews), Zillow (discovery, property data), and Idealista (discovery, property data, Spanish real-estate focus). Returns parsed JSON rather than raw HTML, with provider-managed selectors that absorb site-side layout changes.

- **Human URL:** [https://docs.zenrows.com/scraper-apis/introduction](https://docs.zenrows.com/scraper-apis/introduction)

#### Tags

- Web Scraping
- Structured Data
- E-Commerce
- Real Estate
- Amazon
- Google
- Walmart
- Zillow
- Idealista

#### Properties

- [Documentation](https://docs.zenrows.com/scraper-apis/introduction)
- [Documentation](https://docs.zenrows.com/scraper-apis/get-started/amazon-asin)
- [Documentation](https://docs.zenrows.com/scraper-apis/get-started/google-search)
- [Documentation](https://docs.zenrows.com/scraper-apis/get-started/zillow-property)
- [Documentation](https://docs.zenrows.com/scraper-apis/get-started/idealista-property)
- [Documentation](https://docs.zenrows.com/scraper-apis/get-started/walmart-product)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ZenRows MCP Server

Official ZenRows Model Context Protocol server that exposes the scraping platform to AI assistants. Available as a remote hosted server at https://mcp.zenrows.com/mcp with OAuth bearer authentication, or locally via the npm package @zenrows/mcp (npx -y @zenrows/mcp). Ships scrape tools for Markdown/HTML/JSON/plaintext/PDF/screenshots and 30+ browser_* tools covering navigation, clicks, form fills, JavaScript execution, cookies, tabs, and persistent sessions.

- **Human URL:** [https://docs.zenrows.com/integrations/mcp/mcp-overview](https://docs.zenrows.com/integrations/mcp/mcp-overview)

#### Tags

- MCP
- AI
- Agents
- LLM

#### Properties

- [Documentation](https://docs.zenrows.com/integrations/mcp/mcp-overview)
- [Documentation](https://docs.zenrows.com/integrations/mcp/claude-desktop)
- [Documentation](https://docs.zenrows.com/integrations/mcp/claude-code)
- [Documentation](https://docs.zenrows.com/integrations/mcp/cursor)
- [Documentation](https://docs.zenrows.com/integrations/mcp/vscode)
- [Source Code](https://github.com/ZenRows/zenrows-mcp)
- [N P M](https://www.npmjs.com/package/@zenrows/mcp)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ZenRows SDKs

First-party SDKs that wrap the Universal Scraper API and Residential Proxies with automatic retries, exponential backoff, concurrency helpers, and ergonomic clients. Official SDKs ship for Python (pip install zenrows), Node.js/TypeScript, Go, and the browser. Sample projects and a Scrapy middleware are published from github.com/ZenRows. All SDKs are MIT-licensed.

- **Human URL:** [https://github.com/ZenRows](https://github.com/ZenRows)

#### Tags

- SDK
- Python
- Node.js
- TypeScript
- Go
- Scrapy

#### Properties

- [Git Hub Org](https://github.com/ZenRows)
- [Python S D K](https://github.com/ZenRows/zenrows-python-sdk)
- [Node J S S D K](https://github.com/ZenRows/zenrows-node-sdk)
- [Go S D K](https://github.com/ZenRows/zenrows-go-sdk)
- [Java Script S D K](https://github.com/ZenRows/browser-js-sdk)
- [Scrapy Middleware](https://github.com/ZenRows/scrapy-zenrows-middleware)
- [Postman Collection](collections/zenrows-universal-scraper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zenrows-universal-scraper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.zenrows.com/)
- [Documentation](https://docs.zenrows.com/)
- [Git Hub Org](https://github.com/ZenRows)
- [Pricing](https://www.zenrows.com/pricing)
- [Sign Up](https://app.zenrows.com/register)
- [Login](https://app.zenrows.com/)
- [Blog](https://www.zenrows.com/blog)
- [Knowledge Base](https://www.zenrows.com/knowledgehub)
- [Status](https://status.zenrows.com/)
- [Changelog](https://eu.intercom.news/zenrows)
- [Error Codes](https://docs.zenrows.com/api-error-codes)
- [Legal](https://www.zenrows.com/legal)
- [Forbidden Sites](https://docs.zenrows.com/forbidden-sites)
- [Academy](https://docs.zenrows.com/zenrows-academy/introduction)
- [L L Ms Txt](https://docs.zenrows.com/llms.txt)
- [LinkedIn](https://www.linkedin.com/company/zenrows)
- [X Twitter](https://twitter.com/ZenRows)
- [Integrations](https://docs.zenrows.com/integrations/overview)
- [Plans And Pricing](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/plans/zenrows-plans-pricing.yml)
- [Rate Limits](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/rate-limits/zenrows-rate-limits.yml)
- [Fin Ops](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/finops/zenrows-finops.yml)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/vocabulary/zenrows-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
