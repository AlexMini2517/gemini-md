On this PC Python is installed and managed through `uv`.
When making git commits, always write in the english language and follow the latest standards to write the commit message.

For web scraping, fetching, and web page inspection:
- Never use curl, Invoke-WebRequest, or unstealthed HTTP requests to visit target websites or read URLs.
- Always use the installed Scrapling MCP tools (or `scrapling` CLI with `--ai-targeted`) to fetch and extract content cleanly.
- For dynamic pages, JavaScript rendering, or sites protected by anti-bot/Cloudflare, leverage Scrapling's stealth browser capabilities (e.g. `browser_fetch`, `solve_cloudflare=True`).
- When writing Python code or scripts that involve web scraping, parsing, or crawling, use Scrapling (`scrapling.fetchers`, `scrapling.spiders`, `scrapling.parser`) as the primary framework instead of BeautifulSoup, Selenium, or raw Requests.