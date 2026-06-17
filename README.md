[Facebook Likes Reactions Scraper](https://apify.com/scrapapi/facebook-likes-reactions-scraper?fpr=data)

## Facebook Likes Reactions Scraper

Facebook Likes Reactions Scraper is a production-ready Facebook reactions scraper that extracts per-post likes and reactions — including who reacted and how — from public Facebook posts. It solves the tedious problem of manually collecting engagement data so you can analyze audiences and benchmarks at scale. Built for marketers, developers, data analysts, and researchers, this Facebook post reactions scraper delivers structured datasets you can export and automate across workflows.

## What is Facebook Likes Reactions Scraper?

Facebook Likes Reactions Scraper is a scalable Facebook reactions extractor that collects detailed engagement from public posts, including reaction type, user name, profile URL, and profile image. This Facebook likes reactions extractor is ideal for content analysis, brand monitoring, competitor research, and social media tracking — enabling you to scrape Facebook post reactions reliably at scale.

## What data / output can you get?

| Data field | Description | Example value |
| --- | --- | --- |
| postId | The decoded feedback/post identifier associated with the reactions | 10117197689958261 |
| facebookUrl | The Facebook post URL that was processed | [https://www.facebook.com/zuck/posts/10117197689958261](https://www.facebook.com/zuck/posts/10117197689958261) |
| reaction | Normalized reaction type | love |
| name | Display name of the reacting user | Jane Doe |
| profileUrl | Link to the user’s Facebook profile | [https://www.facebook.com/janedoe](https://www.facebook.com/janedoe) |
| userProfileImageUrl | Profile picture URL of the reacting user | [https://scontent.xx.fbcdn.net/v/t39.30808-6/abc123.jpg](https://scontent.xx.fbcdn.net/v/t39.30808-6/abc123.jpg) |
| facebookId | Decoded feedback ID tied to the post | 10117197689958261 |
| pageAdLibrary.is_business_page_active | Static flag indicating business page activity (as reported in output) | false |
| pageAdLibrary.id | The ID associated with the user node in the reaction list | 100012345678901 |
| inputUrl | The original input URL (echoed back) | [https://www.facebook.com/zuck/posts/10117197689958261](https://www.facebook.com/zuck/posts/10117197689958261) |

Notes:

- Results are pushed to the Apify dataset, which you can export to JSON or CSV from the OUTPUT tab.
- Some fields (for example, userProfileImageUrl or profileUrl) may be empty strings when not available on the source page.

## Key features

- 🚀 Bold anti-bot resilience with proxy fallback
Automatically rotates between datacenter and residential proxies to handle blocks and keep your Facebook engagement scraper running smoothly.
- 🧠 Dynamic token extraction
Securely negotiates fb_dtsg and doc_id via real requests that mimic human browsers, powering reliable GraphQL calls for reactions retrieval.
- 📈 Batch scraping & bulk automation
Supports bulk URL processing so you can run a large Facebook reactions data scraper job across many posts in one go.
- ⚡ High-concurrency async engine
Built as a Facebook reactions scraper Python actor using aiohttp and asyncio for fast, concurrent requests and pagination handling.
- 📦 Clean, ready-to-use datasets
Structured output with reaction type, user name, profile URL, and profile image — perfect to export Facebook likes to CSV or JSON for downstream analysis.
- 🔁 Robust pagination logic
Automatically follows cursors to collect more reactors until your resultsLimit is met.
- 🧰 Production-ready on Apify
Runs on reliable Apify infrastructure with logs, datasets, and repeatable workflows — a dependable Facebook reactions export tool for teams.

## How to use Facebook Likes Reactions Scraper - step by step

1. Sign in to the Apify Console and open the Facebook Likes Reactions Scraper actor.
2. In the Input, paste one or more Facebook post URLs in the urls field (string list).
3. Set resultsLimit to control how many reactions you want per URL.
4. Optionally configure proxyConfiguration. The actor also handles datacenter and residential fallbacks automatically.
5. Click Start to run. The logs will show connection negotiation, pagination, and saved reactions in real time.
6. When the run finishes, open the OUTPUT tab to view your dataset items.
7. Export results to JSON or CSV for analysis, reporting, or BI pipelines.

Pro tip: Use resultsLimit to cap how many reactors you collect per post when running large bulk jobs.

## Use cases

| Use case | Description |
| --- | --- |
| Brand monitoring – engagement insights | Track how audiences react to competitor or brand posts to benchmark reaction mix and identify top-engaging content. |
| Content performance analysis | Measure reaction breakdowns across multiple posts to correlate creative types with audience sentiment. |
| Influencer vetting – audience engagement | Evaluate real reactions on public posts to gauge engagement quality before partnerships. |
| Market research – sentiment signals | Use love/haha/wow/sad/angry distributions as lightweight sentiment inputs for trend analysis. |
| Data enrichment for analytics | Feed structured reactions into dashboards and export Facebook likes to CSV for SQL/BI workflows. |
| Automation pipelines | Schedule recurring runs on Apify and download Facebook reactions data for reporting jobs or ETL tasks. |
| Academic and social research | Build datasets of public post reactors for engagement pattern studies using a Facebook post reactions scraper. |

## Why choose Facebook Likes Reactions Scraper?

- 🎯 Precision-built for reactions: Focused extraction of reaction type, user identity fields, and profile assets.
- 🌐 Resilient scraping engine: Automated fallback between datacenter and residential proxies for high success rates.
- 📊 Scales to bulk workloads: Process many URLs in a single run with efficient pagination and limits.
- 🐍 Python-based reliability: A Facebook reactions scraper Python actor using aiohttp/asyncio for speed and stability.
- 🔒 Public data only: Designed to collect data from publicly available sources.
- 💾 Easy exports: Download structured datasets from the OUTPUT tab to JSON or CSV without extra tooling.
- 🧱 Better than extensions: Avoid brittle browser plugins; run a production-grade Facebook reactions extractor on Apify.

In short, this is a dependable Facebook likes scraper built for accuracy, scale, and automation on solid infrastructure.

## Is it legal / ethical to use Facebook Likes Reactions Scraper?

Yes, when used responsibly. This tool is designed to collect data only from publicly available sources and does not access private or password-protected content. Always ensure your usage complies with applicable laws and platform terms.

Guidelines:

- Only collect publicly visible data.
- Respect platform terms and applicable regulations (e.g., GDPR, CCPA).
- Avoid using data for spam or invasive activities.
- Consult your legal team for edge cases or jurisdiction-specific questions.

## Input parameters & output format

Example JSON input

```
{
  "urls": [
    "https://www.facebook.com/zuck/posts/10117197689958261",
    "https://www.facebook.com/zuck/posts/pfbid067YZ4YqVJnKvNFQG15s9fBFbbbGTBxYeP21bbEx29grppcz75A1GWbsTyLwbCM8Yl"
  ],
  "resultsLimit": 20,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

Input parameters

- urls (array, required): List one or more Facebook URLs to scrape reactions from. Example: [https://www.facebook.com/zuck/posts/10117197689958261](https://www.facebook.com/zuck/posts/10117197689958261)

- Default: none (must be provided)
- resultsLimit (integer, optional): Maximum number of reactions to collect per URL.

- Default: 20
- proxyConfiguration (object, optional): Proxy settings to bypass restrictions. The scraper automatically handles datacenter and residential fallbacks for maximum success rate.

- Default prefill: {"useApifyProxy": false}

Example JSON output

```
[
  {
    "postId": "10117197689958261",
    "facebookUrl": "https://www.facebook.com/zuck/posts/10117197689958261",
    "reaction": "love",
    "name": "Jane Doe",
    "profileUrl": "https://www.facebook.com/janedoe",
    "userProfileImageUrl": "https://scontent.xx.fbcdn.net/v/t39.30808-6/abc123.jpg",
    "facebookId": "10117197689958261",
    "pageAdLibrary": {
      "is_business_page_active": false,
      "id": "100012345678901"
    },
    "inputUrl": "https://www.facebook.com/zuck/posts/10117197689958261"
  },
  {
    "postId": "10117197689958261",
    "facebookUrl": "https://www.facebook.com/zuck/posts/10117197689958261",
    "reaction": "haha",
    "name": "John Smith",
    "profileUrl": "https://www.facebook.com/johnsmith",
    "userProfileImageUrl": "",
    "facebookId": "10117197689958261",
    "pageAdLibrary": {
      "is_business_page_active": false,
      "id": "100009999999999"
    },
    "inputUrl": "https://www.facebook.com/zuck/posts/10117197689958261"
  }
]
```

Notes:

- reaction is normalized to like, love, haha, wow, sad, or angry.
- Some fields may be empty strings when unavailable on the source post.

## FAQ

### Is there a free trial?

Yes. The listing includes a trial with 120 trial minutes so you can evaluate the scraper before subscribing. Actual availability and limits are managed by Apify at runtime.

### Do I need to provide Facebook cookies?

No. You don’t need to supply cookies in the input. The actor negotiates required tokens automatically to fetch reactions from public posts.

### What input formats are supported for URLs?

Provide a list of Facebook post URLs as strings in the urls array. You can add multiple URLs for bulk processing in one run.

### How many reactions can I scrape per post?

Set resultsLimit to control the maximum number of reactions to collect per URL. The scraper paginates and stops when the limit is reached or there’s no next page.

### Which reaction types are included?

Reactions are normalized to like, love, haha, wow, sad, and angry, based on Facebook’s reaction IDs mapped internally by the actor.

### Can I export the results?

Yes. Open the OUTPUT tab after the run and export the dataset to JSON or CSV. This makes it easy to download Facebook reactions data for analysis.

### Does it work on private or restricted posts?

No. The actor is designed for publicly available content. Private, restricted, or login-gated content is not collected.

### Is this built in Python?

Yes. This is a Facebook reactions scraper Python actor using aiohttp and asyncio for speed, concurrency, and reliability on the Apify platform.

## Closing CTA / Final thoughts

Facebook Likes Reactions Scraper is built to collect structured engagement data from public Facebook posts at scale. With automated proxy fallback, dynamic token handling, and clean datasets, it empowers marketers, developers, analysts, and researchers to move from manual copy-paste to reliable automation. Export Facebook likes to CSV or JSON, run bulk jobs with resultsLimit, and operationalize a dependable Facebook reactions extractor for your workflows. Start scraping smarter engagement signals today.