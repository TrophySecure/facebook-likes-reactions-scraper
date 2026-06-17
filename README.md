[Facebook Likes Reactions Scraper](https://apify.com/api-empire/facebook-likes-reactions-scraper?fpr=data)

# Facebook Likes and Reactions Scraper

A robust and scalable Apify actor designed to scrape reactions (like, love, haha, wow, sad, angry) and user profiles from Facebook posts.

## Why Choose Us?

- Completely automated scaling and retry mechanisms.
- Smart fallback proxies to handle blocking from Facebook.
- Fast and highly concurrent web scraping.

## Key Features

- Supports extracting all reaction types from a given post dynamically.
- Handles Javascript token extraction dynamically natively simulating human browsers.
- Automatically handles Datacenter and Residential proxy fallback mechanisms.
- Supports bulk URL processing.

## Input Example

You can configure the following input variables in JSON form:

```
{
  "urls": [{"url": "https://www.facebook.com/zuck/posts/10117197689958261"}],
  "resultsLimit": 100,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

- `urls`: List of Facebook post URLs to scrape.
- `resultsLimit`: The maximum number of reactions to extract per URL.
- `proxyConfiguration`: Default proxy configurations (fallback logic is handled automatically internally).

## Output Example

Returns structured JSON dataset items containing detailed reaction lists:

```
{
    "postId": "10117197689958261",
    "facebookUrl": "https://www.facebook.com/zuck/posts/pfbid067YZ4Yq... ",
    "reaction": "love",
    "name": "Soleio",
    "profileUrl": "https://www.facebook.com/soleio",
    "facebookId": "10117197689958261",
    "inputUrl": "https://www.facebook.com/zuck/posts/10117197689958261"
}
```

## 🚀 How to Use the Actor (via Apify Console)

1. Log in at [https://console.apify.com](https://console.apify.com) and go to Actors.
2. Find your actor and click it.
3. Configure inputs (URLs, Limit).
4. Run the actor.
5. Monitor logs in real time.
6. Access results in the OUTPUT tab.
7. Export results to JSON or CSV.

## Cautions

- Data is collected only from publicly available sources.
- No data is taken from private accounts or password-protected content.
- The end user is responsible for ensuring legal compliance (spam laws, privacy, data protection, etc.).

## What are other Facebook scraping tools?

If you want to scrape specific Facebook data, you can use any of the dedicated scrapers below for faster and more targeted results.

| Scraper Name | Scraper Name |
| --- | --- |
| [Facebook Ads Library Scraper](https://apify.com/api-empire/facebook-ads-library-scraper) | [Facebook Page Lead Scraper](https://apify.com/api-empire/facebook-page-lead-scraper) |
| [Facebook B2b Email Scraper](https://apify.com/api-empire/facebook-b2b-email-scraper) | [Facebook Page Phone Number Scraper](https://apify.com/api-empire/facebook-page-phone-number-scraper) |
| [Facebook B2b Lead Scraper](https://apify.com/api-empire/facebook-b2b-lead-scraper) | [Facebook Page Posts Scraper](https://apify.com/api-empire/facebook-page-posts-scraper) |
| [Facebook B2b Phone Number Scraper](https://apify.com/api-empire/facebook-b2b-phone-number-scraper) | [Facebook Pages Scraper](https://apify.com/api-empire/facebook-pages-scraper) |
| [Facebook Comments Scraper](https://apify.com/api-empire/facebook-comments-scraper) | [Facebook Phone Number Scraper](https://apify.com/api-empire/facebook-phone-number-scraper) |
| [Facebook Email Scraper](https://apify.com/api-empire/facebook-email-scraper) | [Facebook Photos Scraper](https://apify.com/api-empire/facebook-photos-scraper) |
| [Facebook Event Search Scraper](https://apify.com/api-empire/facebook-event-search-scraper) | [Facebook Posts Scraper](https://apify.com/api-empire/facebook-posts-scraper) |
| [Facebook Events Scraper](https://apify.com/api-empire/facebook-events-scraper) | [Facebook Posts Search Scraper](https://apify.com/api-empire/facebook-posts-search-scraper) |
| [Facebook Followers & Following Scraper](https://apify.com/api-empire/facebook-followers-following-scraper) | [Facebook Profile Email Scraper](https://apify.com/api-empire/facebook-profile-email-scraper) |
| [Facebook Followers Scraper](https://apify.com/api-empire/facebook-followers-scraper) | [Facebook Profile Lead Scraper](https://apify.com/api-empire/facebook-profile-lead-scraper) |
| [Facebook Group Member Scraper](https://apify.com/api-empire/facebook-group-member-scraper) | [Facebook Profile Phone Number Scraper](https://apify.com/api-empire/facebook-profile-phone-number-scraper) |
| [Facebook Group Post Scraper](https://apify.com/api-empire/facebook-group-post-scraper) | [Facebook Reels Scraper](https://apify.com/api-empire/facebook-reels-scraper) |
| [Facebook Group Posts And Details Scraper](https://apify.com/api-empire/facebook-group-posts-and-details-scraper) | [Facebook Reviews Scraper](https://apify.com/api-empire/facebook-reviews-scraper) |
| [Facebook Group Profile Scraper](https://apify.com/api-empire/facebook-group-profile-scraper) | [Facebook Search Scraper](https://apify.com/api-empire/facebook-search-scraper) |
| [Facebook Groups Posts Scraper](https://apify.com/api-empire/facebook-groups-posts-scraper) | [Facebook Url To Id Scraper](https://apify.com/api-empire/facebook-url-to-id-scraper) |
| [Facebook Groups Scraper](https://apify.com/api-empire/Facebook-Groups-Scraper) | [Facebook User Search Scraper](https://apify.com/api-empire/Facebook-User-Search-Scraper) |
| [Facebook Groups Search Scraper](https://apify.com/api-empire/facebook-groups-search-scraper) | [Facebook Video Search Scraper](https://apify.com/api-empire/facebook-video-search-scraper) |
| [Facebook Lead Scraper](https://apify.com/api-empire/facebook-lead-scraper) | [Facebook Video Transcript Extractor](https://apify.com/api-empire/facebook-video-transcript-extractor) |
| [Facebook Marketplace Scraper](https://apify.com/api-empire/facebook-marketplace-scraper) | [Facebook Videos Scraper](https://apify.com/api-empire/facebook-videos-scraper) |
| [Facebook Page Email Scraper](https://apify.com/api-empire/facebook-page-email-scraper) |  |