# SEO — 0 to 100 Complete Reference

> 🌐 **Language:** English | [فارسی](README.fa.md)
> یه مرجع کامل از صفر تا صد سئو + GEO (Generative Engine Optimization)

---

## 📌 Table of Contents

1. [What is SEO](#1-what-is-seo)
2. [How Search Engines Work](#2-how-search-engines-work)
3. [Keyword Research](#3-keyword-research)
4. [On-Page SEO](#4-on-page-seo)
5. [Technical SEO](#5-technical-seo)
6. [Content Strategy](#6-content-strategy)
7. [Off-Page SEO & Link Building](#7-off-page-seo--link-building)
8. [Local SEO](#8-local-seo)
9. [E-commerce SEO](#9-e-commerce-seo)
10. [International SEO](#10-international-seo)
11. [Core Web Vitals](#11-core-web-vitals)
12. [Google Algorithms](#12-google-algorithms)
13. [SERP Features](#13-serp-features)
14. [Analytics & Measurement](#14-analytics--measurement)
15. [SEO Hat Types](#15-seo-hat-types)
16. [GEO — Generative Engine Optimization](#16-geo--generative-engine-optimization)
17. [Tools](#17-tools)

---

## 1. What is SEO

**Search Engine Optimization** = improving a website's visibility in **organic (unpaid)** search results.

- Google's core principle: **user satisfaction = Google's satisfaction**
- SEO is a long-term process — results take weeks to months
- Don't try to trick Google — short-term gains lead to long-term penalties
- SEO vs SEM vs ASO:

| Type | Cost | Speed | Channel |
|------|------|-------|---------|
| **SEO** | Time | Weeks–Months | Google/Bing organic |
| **SEM** | Money (PPC) | Immediate | Google Ads |
| **ASO** | Time | Weeks | App Store / Google Play |

---

## 2. How Search Engines Work

### 2.1 Crawling
Googlebot discovers and fetches pages across the web.

- **URL Discovery**: sitemaps, internal links, external links, redirects
- **Crawl Budget**: Google limits crawls per site — don't waste it on low-value pages (paginated, filtered, duplicate URLs)
- Control crawling via: `robots.txt`, `noindex` meta tag, `X-Robots-Tag` header
- **Crawl frequency** depends on: page authority, update frequency, server speed

### 2.2 Indexing
Google processes crawled pages and stores them in its index.

- Extracts: text content, links, images, structured data, metadata
- Runs rendering (JavaScript pages rendered separately — can cause delay)
- **Indexed ≠ Ranked** — must pass quality threshold to appear in results
- Check: `site:yourdomain.com` | Google Search Console → Coverage

### 2.3 Ranking
Google decides order of results for a query using 200+ signals.

- **Relevance**: does content match search intent?
- **Authority**: how trusted is the site/page?
- **Experience**: is the page fast, stable, mobile-friendly?
- **Freshness**: newer content preferred for news/time-sensitive queries
- **Personalization**: device, language, location, search history

---

## 3. Keyword Research

### 3.1 Keyword Types by Length

| Type | Example | Volume | Competition | Intent |
|------|---------|--------|-------------|--------|
| **Short-tail** | "shoes" | Very High | Very High | Unclear |
| **Mid-tail** | "running shoes men" | Medium | Medium | Clearer |
| **Long-tail** | "best running shoes for flat feet 2024" | Low | Low | High |

> Long-tail = easier to rank + higher conversion rate

### 3.2 Search Intent (Most Important Factor)

| Intent | What User Wants | Example | Best Content |
|--------|----------------|---------|--------------|
| **Informational** | Learn something | "how to do SEO" | Blog, Guide |
| **Navigational** | Find specific site | "Gmail login" | Homepage, App |
| **Commercial** | Compare before buying | "best SEO tools" | Comparison, Review |
| **Transactional** | Buy/Act now | "buy Ahrefs" | Product page, Landing page |

> **Match your content type to the intent** — wrong content type = won't rank even with keywords

### 3.3 Keyword Metrics

- **Search Volume**: monthly searches — from tools like Ahrefs, GSC
- **Keyword Difficulty (KD)**: 0–100, how hard to rank (Ahrefs/SEMrush)
- **CPC**: cost per click in ads — higher CPC = more commercial value
- **CTR**: click-through rate from SERP — featured snippets steal clicks
- **Trend**: seasonal or declining? (use Google Trends)

### 3.4 Keyword Strategy

- **Seed Keywords**: broad starting terms related to your niche
- **LSI / Semantic Keywords**: related terms Google expects to see together
- **Topic Clusters**: group keywords around one pillar topic
- **Cannibalization**: two pages targeting same keyword = compete with each other → merge or differentiate
- **Negative Keywords** (SEM): exclude irrelevant search terms from paid ads

### 3.5 Research Process

1. Brainstorm seed keywords
2. Expand via tools (Ahrefs, SEMrush, Google Suggest, PAA, Related Searches)
3. Analyze competitors' ranking keywords
4. Filter by intent, volume, difficulty
5. Map each keyword to one page (keyword-to-page mapping)

---

## 4. On-Page SEO

### 4.1 Title Tag
- Most important on-page ranking factor
- Appears in SERP and browser tab
- Length: **50–60 chars** (truncated beyond 600px width)
- Format: `Primary Keyword — Secondary | Brand`
- Put keyword near the beginning
- Every page needs unique title

### 4.2 Meta Description
- Not a direct ranking factor — but affects **CTR**
- Length: **150–160 chars**
- Should include keyword (Google bolds it in SERP)
- Write as an ad — compelling reason to click

### 4.3 Heading Structure

```
H1 — One per page, main topic keyword
  H2 — Major sections
    H3 — Sub-sections
      H4 — Details (rare)
```

- H1 must contain primary keyword
- Headings help Google understand page structure
- Don't skip levels (H1 → H3 without H2)

### 4.4 URL Structure
- Short and descriptive: `/seo-guide/` not `/page?id=123`
- Use hyphens, not underscores: `on-page-seo` not `on_page_seo`
- Include keyword in URL
- Avoid dates unless content is news/time-sensitive
- Keep URL depth shallow: domain.com/category/page (max 3 levels)

### 4.5 Keyword Usage in Content
- Primary keyword in: title, H1, first 100 words, URL, meta desc
- Use naturally — don't stuff
- Density: ~1–2% is fine — focus on natural usage
- Use synonyms and related terms (LSI) throughout
- Bold important terms occasionally

### 4.6 Image Optimization
- **Alt text**: describes image for crawlers + accessibility — include keyword where natural
- **File name**: `red-running-shoes.jpg` not `IMG_4523.jpg`
- **Format**: WebP preferred, then JPEG for photos, PNG for logos
- **Lazy loading**: `loading="lazy"` attribute
- **Dimensions**: specify width/height to prevent CLS
- **Compress**: use TinyPNG, Squoosh, or server-side compression

### 4.7 Internal Linking
- Links between your own pages pass **link equity (PageRank)**
- Use **keyword-rich anchor text** (not "click here")
- Link from high-authority pages to pages you want to rank
- Flat structure: every page reachable in 3 clicks from homepage
- Avoid orphan pages (pages with no internal links pointing to them)

### 4.8 Canonical Tags
```html
<link rel="canonical" href="https://domain.com/preferred-url/" />
```
- Tells Google which version of a page is the "original"
- Use when: URL parameters, pagination, www vs non-www, HTTP vs HTTPS
- Prevents duplicate content penalty

### 4.9 Open Graph & Social Tags
```html
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:image" content="..." />
<meta name="twitter:card" content="summary_large_image" />
```
- Controls how page appears when shared on social media
- Good OG image = higher social CTR = more traffic = indirect SEO signal

### 4.10 Schema Markup (Structured Data)
Adds machine-readable context to content — enables Rich Results in SERP.

| Schema Type | Rich Result |
|-------------|-------------|
| `Article` | Author, date in result |
| `FAQPage` | Expandable Q&A under result |
| `HowTo` | Step-by-step instructions in SERP |
| `Product` | Price, availability, rating stars |
| `Review` | Star ratings |
| `LocalBusiness` | Address, hours, phone |
| `BreadcrumbList` | Breadcrumb trail in URL |
| `VideoObject` | Video thumbnail in SERP |
| `JobPosting` | Job listings feature |
| `Recipe` | Ingredients, time, calories |

- Format: JSON-LD (preferred), Microdata, RDFa
- Validate: Google Rich Results Test

---

## 5. Technical SEO

### 5.1 Crawlability

- **robots.txt**: at `domain.com/robots.txt` — `Disallow: /admin/` blocks crawlers
- **Meta robots**: `<meta name="robots" content="noindex, nofollow" />` per page
- **Crawl traps**: infinite pagination, session IDs in URLs, faceted navigation — block these
- **XML Sitemap**: submit to Google Search Console — lists all important URLs
- **Sitemap index**: one file linking to multiple sitemaps (if >50k URLs)

### 5.2 Indexability

- `noindex` = page won't be indexed (use for: thank-you pages, admin, internal search)
- `nofollow` = don't follow links on page (rarely needed)
- **Soft 404**: page returns 200 status but has "not found" content — Google ignores it
- **Duplicate content**: same content on multiple URLs — use canonical or 301 redirect
- **Thin content**: very little useful text — add depth or noindex

### 5.3 Site Architecture

- **Silo Structure**: cluster related content together under topic hubs
- **Flat Architecture**: homepage → category → page (3 levels max)
- **Breadcrumbs**: improve navigation + SERP display
- **Hub & Spoke / Topic Clusters**: one pillar page + many related pages linking to/from it

### 5.4 Redirects

| Type | Code | Use Case | Link Equity |
|------|------|----------|-------------|
| **Permanent** | 301 | Page moved permanently | ~90% passed |
| **Temporary** | 302 | Page moved temporarily | Not passed |
| **Gone** | 410 | Page deleted permanently | Faster deindex |
| **Redirect chain** | — | Avoid A→B→C — go direct | Equity lost each hop |

### 5.5 HTTPS

- Google confirmed HTTPS as ranking signal
- All pages must be HTTPS — including images/scripts (mixed content breaks it)
- Redirect all HTTP to HTTPS with 301
- Use HSTS header for stronger enforcement

### 5.6 Mobile Optimization

- **Mobile-First Indexing**: Google indexes mobile version — desktop is secondary
- Responsive design preferred over separate m. subdomain
- Font size ≥ 16px, tap targets ≥ 48px
- No horizontal scroll, no Flash
- Test: Google Mobile-Friendly Test

### 5.7 Page Speed

- Direct ranking factor since 2010, Core Web Vitals since 2021
- Key improvements:
  - Enable **GZIP/Brotli** compression
  - Use **CDN** (Cloudflare, BunnyCDN)
  - **Browser caching** (cache-control headers)
  - **Minify** CSS/JS/HTML
  - Eliminate **render-blocking resources** (defer/async JS)
  - Optimize **Critical Rendering Path**
  - Use **lazy loading** for images below fold
  - Reduce **server response time** (TTFB < 200ms)

### 5.8 JavaScript SEO

- Googlebot renders JS but with **delay** — may take days to weeks
- Don't put critical content in JS-only — use SSR or pre-rendering
- Internal links in JS are crawlable but slower
- Test: fetch as Google in GSC, or view page source vs rendered source

### 5.9 Log File Analysis

- Crawl log = raw data on exactly which pages Googlebot visited and when
- Identifies: wasted crawl budget, crawl frequency of important pages, server errors seen by bot
- Tools: Screaming Frog Log Analyzer, Splunk

### 5.10 Hreflang (International)

```html
<link rel="alternate" hreflang="en" href="https://domain.com/en/page/" />
<link rel="alternate" hreflang="fa" href="https://domain.com/fa/page/" />
<link rel="alternate" hreflang="x-default" href="https://domain.com/" />
```
- Tells Google which language/country version to show to which users
- Must be bidirectional (every page must reference all its alternates)

---

## 6. Content Strategy

### 6.1 E-E-A-T (Quality Framework)

| Letter | Meaning | How to Show It |
|--------|---------|----------------|
| **E** | Experience | First-hand experience, case studies, personal examples |
| **E** | Expertise | Author credentials, depth of content, accurate info |
| **A** | Authoritativeness | Backlinks from authorities, brand mentions, citations |
| **T** | Trustworthiness | HTTPS, About page, Contact, Privacy, accurate claims |

- YMYL (Your Money Your Life) sites (health, finance, law) need highest E-E-A-T
- Author bio pages with real credentials significantly help

### 6.2 Content Types

| Type | Purpose | SEO Value |
|------|---------|-----------|
| **Pillar Pages** | Comprehensive topic overview | High — attracts many keywords |
| **Cluster Pages** | Deep-dive into subtopics | Medium — feeds pillar |
| **Blog Posts** | Fresh content, long-tail keywords | High for traffic |
| **Landing Pages** | Conversion focus | High for commercial keywords |
| **FAQs** | Answer quick questions | PAA features, voice search |
| **Case Studies** | Show results/experience | Trust + E-E-A-T |
| **Comparison Pages** | X vs Y | Commercial intent, high conversion |
| **Glossary** | Define terms | Topical authority, featured snippets |

### 6.3 Content Quality Signals

- **Length**: no magic number — match competitor depth for that query
- **Freshness**: update old content regularly (especially statistics, dates)
- **Originality**: no copied or spun content
- **Multimedia**: images, video, infographics increase dwell time
- **Readability**: short paragraphs, subheadings, bullet points
- **Topical coverage**: answer all related questions in one place
- **Dwell Time**: how long user stays on page before returning to Google (indirect signal)

### 6.4 Content Optimization Process

1. Search your target keyword in Google
2. Analyze top 10 results — what topics do they cover?
3. Check People Also Ask for subtopics
4. Write content that covers all angles + something extra
5. Use keyword in natural context throughout
6. Add internal links to/from related pages
7. Update content every 6–12 months

### 6.5 Featured Snippet Optimization

- Featured snippets = **Position 0** — above all other organic results
- Google pulls snippets from pages ranking in top 10
- Types: paragraph, list, table, video
- How to target:
  - Answer a question directly in 40–60 words
  - Use a heading that IS the question
  - Follow with a clear, concise answer
  - Use lists/tables for list-type snippets

---

## 7. Off-Page SEO & Link Building

### 7.1 Why Backlinks Matter

- Links = votes of confidence from other sites
- More high-quality links = higher authority = higher rankings
- **Quality > Quantity**: one link from NYT > 1000 links from random blogs

### 7.2 Link Metrics

| Metric | Tool | What It Measures |
|--------|------|-----------------|
| **Domain Rating (DR)** | Ahrefs | Overall domain backlink strength (0–100) |
| **Domain Authority (DA)** | Moz | Similar to DR (0–100) |
| **Page Authority (PA)** | Moz | Individual page strength |
| **Trust Flow** | Majestic | Quality of links |
| **Citation Flow** | Majestic | Quantity of links |
| **Spam Score** | Moz | Likelihood of penalization (keep low) |

### 7.3 Types of Links

| Type | SEO Value | Description |
|------|-----------|-------------|
| **Editorial** | Highest | Natural links others chose to give |
| **Guest Post** | High | You write content on another site |
| **Resource Page** | High | Listed as useful resource |
| **Broken Link** | High | Replace a dead link with yours |
| **HARO/PR** | High | Quoted in media/press |
| **Directory** | Low-Medium | Business/niche directories |
| **Forum** | Low | Profile/comment links |
| **Social** | Minimal | No-follow but drives traffic |

### 7.4 Link Building Strategies

- **Guest Posting**: write articles for relevant blogs in your niche
- **Skyscraper Technique**: find top-linked content → make better version → outreach
- **Broken Link Building**: find dead links on relevant sites → offer your page as replacement
- **Resource Page Outreach**: find "useful links" pages and pitch your content
- **HARO (Help a Reporter Out)**: answer journalist queries → get quoted → earn link
- **Digital PR**: create link-worthy assets (studies, data, tools, infographics)
- **Unlinked Mentions**: find sites that mention your brand but don't link → ask for link
- **Competitor Analysis**: see who links to competitors → pitch them too

### 7.5 Link Attributes

```html
<a href="..." rel="dofollow">Passes equity</a>   <!-- default -->
<a href="..." rel="nofollow">No equity passed</a>
<a href="..." rel="sponsored">Paid link</a>
<a href="..." rel="ugc">User-generated content</a>
```

### 7.6 Toxic Links & Disavow

- Bad links from spam sites can harm rankings
- Use Google's **Disavow Tool** to tell Google to ignore specific links
- Only use if you have clear evidence of harmful links (Google rarely needs this)

### 7.7 Brand Signals (Off-Page)

- Brand mentions (even without link) — Google recognizes entity associations
- Social media presence and follower count
- Reviews on Google, Trustpilot, Yelp
- Wikipedia page (for large brands)
- Consistent NAP (Name, Address, Phone) across web

---

## 8. Local SEO

For businesses targeting customers in a specific geographic area.

### 8.1 Google Business Profile (GBP)

- Free listing on Google Maps and Local Pack
- Complete every field: name, address, phone, hours, website, category
- Add photos regularly (higher engagement = better ranking)
- Enable messaging, booking if applicable
- Post weekly updates
- Respond to ALL reviews (positive and negative)

### 8.2 Local Ranking Factors

| Factor | Weight | Description |
|--------|--------|-------------|
| **Relevance** | High | Does business match the search? |
| **Distance** | High | How close to searcher? |
| **Prominence** | High | How well-known is the business? |
| **Reviews** | High | Volume, rating, recency, responses |
| **GBP Completeness** | Medium | All fields filled, active profile |
| **Website authority** | Medium | Standard SEO signals |
| **Citations** | Medium | Consistent NAP across directories |

### 8.3 Citations & NAP Consistency

- **NAP** = Name, Address, Phone — must be identical everywhere
- Submit to: Google Business, Bing Places, Apple Maps, Yelp, Yellow Pages, niche directories
- Inconsistency confuses Google and hurts local ranking

### 8.4 Local On-Page Signals

- Include city/region in: title tag, H1, content, URL where natural
- Create location-specific pages for multiple service areas
- Embed Google Map on contact page
- Add LocalBusiness schema markup

### 8.5 Review Strategy

- Ask satisfied customers for reviews (don't incentivize — violates Google policy)
- Respond to every review within 24–48 hours
- More recent reviews > old reviews
- Reviews with keywords help (don't ask customers to use specific keywords — just be detailed)

---

## 9. E-commerce SEO

### 9.1 Site Structure for E-commerce

```
Homepage
├── Category Page (e.g., /running-shoes/)
│   ├── Subcategory (e.g., /running-shoes/men/)
│   │   └── Product Page (e.g., /running-shoes/men/nike-air-zoom/)
```

- Category pages = highest value pages for ranking
- Keep products max 3 clicks from homepage

### 9.2 Product Page Optimization

- Unique product descriptions — not manufacturer copy (duplicate content)
- Include: specs, use cases, FAQs, user reviews
- Schema: `Product` with `AggregateRating`, `Offer`
- High-quality images (multiple angles) with proper alt text
- Clear CTAs, availability signals, trust badges

### 9.3 Category Page Optimization

- Write introductory text (150–300 words) at top or bottom
- Target category-level keywords ("men's running shoes")
- Breadcrumbs for navigation + schema
- Faceted navigation: use `noindex` or canonical on filtered URLs to prevent duplicate content
- Out-of-stock products: keep URL live, show similar products

### 9.4 E-commerce Technical Issues

- **Duplicate content**: from color/size variants → use canonical to main product
- **Pagination**: use `rel="next/prev"` or load-more (Google prefers paginated over infinite scroll for indexing)
- **Thin pages**: products with no description = thin content → add unique content
- **URL parameters**: `?sort=price&color=red` = duplicate URLs → canonicalize or block in robots.txt

### 9.5 Product Structured Data

```json
{
  "@type": "Product",
  "name": "Nike Air Zoom",
  "image": "...",
  "description": "...",
  "offers": {
    "@type": "Offer",
    "price": "120",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "reviewCount": "124"
  }
}
```

---

## 10. International SEO

### 10.1 URL Structure Options

| Structure | Example | Best For |
|-----------|---------|----------|
| **ccTLD** | domain.ir | Strongest geo signal — dedicated country TLD |
| **Subdomain** | fa.domain.com | Separate site signal |
| **Subdirectory** | domain.com/fa/ | Recommended — shares domain authority |
| **URL parameters** | domain.com?lang=fa | Avoid — hard to manage |

### 10.2 Hreflang Implementation

- Must be on every alternate version of the page
- Must be bidirectional (A references B, B references A)
- Use `x-default` for the fallback/language selector page
- Can be in: `<head>`, HTTP header, or sitemap

### 10.3 Content Localization

- Full translation — not Google Translate (low quality = thin content)
- Adapt for cultural context, not just language
- Use local keyword research — search behavior differs by language
- Local currency, date formats, units of measure

---

## 11. Core Web Vitals

Google's user experience metrics — direct ranking factors since 2021.

### 11.1 The Metrics

| Metric | Measures | Good | Needs Work | Poor |
|--------|----------|------|------------|------|
| **LCP** (Largest Contentful Paint) | Loading speed | ≤ 2.5s | 2.5–4s | > 4s |
| **INP** (Interaction to Next Paint) | Responsiveness | ≤ 200ms | 200–500ms | > 500ms |
| **CLS** (Cumulative Layout Shift) | Visual stability | ≤ 0.1 | 0.1–0.25 | > 0.25 |

> FID (First Input Delay) was replaced by INP in March 2024

### 11.2 Improving LCP

- Optimize hero image (largest element on page) — WebP, compressed, preloaded
- `<link rel="preload" as="image" href="hero.webp" />`
- Reduce server response time (TTFB)
- Remove render-blocking CSS/JS
- Use CDN

### 11.3 Improving INP

- Reduce JavaScript execution time
- Break up long tasks (> 50ms) into smaller chunks
- Avoid heavy event listeners on scroll/input
- Use `requestIdleCallback` for non-critical JS

### 11.4 Improving CLS

- Always set explicit `width` and `height` on images and videos
- Reserve space for dynamic content (ads, embeds)
- Avoid injecting content above existing content
- Use CSS `aspect-ratio` for media

### 11.5 Other Page Experience Signals

- **HTTPS**: required
- **Mobile-friendly**: tested via Google's tool
- **No intrusive interstitials**: pop-ups that block content on mobile hurt ranking
- **Safe browsing**: no malware, deceptive content

---

## 12. Google Algorithms

### 12.1 Core Algorithm Updates

| Algorithm | Year | What It Does |
|-----------|------|-------------|
| **PageRank** | 1998 | Counts and weighs inbound links — foundation of Google |
| **Florida** | 2003 | First major update — hit keyword stuffing hard |
| **Panda** | 2011 | Penalizes thin, duplicate, low-quality content |
| **Penguin** | 2012 | Penalizes spammy/manipulative link profiles |
| **Hummingbird** | 2013 | Semantic search — understands full query meaning not just keywords |
| **Pigeon** | 2014 | Improves local search — better distance and location ranking |
| **Mobilegeddon** | 2015 | Penalizes non-mobile-friendly sites |
| **RankBrain** | 2015 | First ML algorithm — interprets novel/complex queries |
| **Possum** | 2016 | Diversifies local results — prevents same address dominating |
| **Fred** | 2017 | Targets aggressive ad-heavy, low-value content sites |
| **Mobile-First Index** | 2018 | Google now indexes mobile version primarily |
| **Medic** | 2018 | YMYL sites need highest quality (health, finance, legal) |
| **BERT** | 2019 | NLP — understands context and relationships between words |
| **Core Updates** | Ongoing | Broad quality reassessments — winners and losers each time |
| **Passage Ranking** | 2021 | Can rank a specific passage/section, not just whole page |
| **Page Experience** | 2022 | Core Web Vitals as ranking signals |
| **E-E-A-T** | 2022 | Added Experience to original E-A-T framework |
| **Helpful Content** | 2022 | Rewards content made for humans, penalizes SEO-first content |
| **Spam Update** | Ongoing | Targets link spam, scaled content abuse, site reputation abuse |

### 12.2 YMYL (Your Money Your Life)

Pages that could impact users' health, finances, safety, or happiness.
- Examples: medical advice, financial advice, news, legal advice
- Google holds these to highest E-E-A-T standards
- Need: verified authors, citations, accuracy, trustworthiness signals

---

## 13. SERP Features

### Organic
- **Blue Links** — standard organic results
- **Sitelinks** — sub-links under major brand results (auto-generated)

### Rich Results (Need Schema)
- **Featured Snippet** — Position 0 answer box — paragraph, list, or table
- **FAQs** — expandable Q&A — uses FAQPage schema
- **How-To** — step-by-step — uses HowTo schema
- **Star Ratings** — product/recipe/review stars — uses AggregateRating schema
- **Breadcrumbs** — URL replaced by breadcrumb trail — uses BreadcrumbList schema
- **Sitelinks Search Box** — search box under result — uses WebSite schema

### Universal Results
- **Images** — Google Images pulled inline — needs good alt text + structured data
- **Videos** — usually YouTube — needs VideoObject schema or video in content
- **Top Stories** — news articles — requires Google News inclusion
- **People Also Ask (PAA)** — expandable related questions — semantic keyword goldmine

### Knowledge Features
- **Knowledge Panel** — right sidebar for brands/entities — fed by Google's Knowledge Graph
- **Local Pack (Map Pack)** — 3 local businesses + map — needs GBP
- **Related Searches** — bottom of SERP — great for finding LSI keywords

### Commerce
- **Shopping Ads (PLA)** — product cards with image/price — via Google Merchant Center
- **Google Flights** — flight search integration
- **Hotel Pack** — hotel listings with prices

### Paid
- **Google Search Ads** — top/bottom, labeled "Sponsored"

---

## 14. Analytics & Measurement

### 14.1 Google Search Console (GSC)

- **Performance**: impressions, clicks, CTR, average position per keyword/page
- **Coverage**: indexed pages, errors, excluded pages
- **Core Web Vitals**: LCP, INP, CLS status for all pages
- **Sitemaps**: submit and monitor sitemap processing
- **Links**: top linking sites, internal links
- **Manual Actions**: if Google has penalized your site
- **URL Inspection**: check index status of any specific URL

### 14.2 Google Analytics 4 (GA4)

- **Acquisition**: where traffic comes from (organic, direct, social, referral)
- **Engagement**: sessions, pages per session, engagement rate, dwell time
- **Conversions**: track goals (purchases, form submissions, sign-ups)
- **Audience**: demographics, device, location
- Connect GA4 to GSC for combined keyword + behavior data

### 14.3 Key SEO Metrics

| Metric | Description | Tool |
|--------|-------------|------|
| **Organic Traffic** | Visits from unpaid search | GA4 |
| **Keyword Rankings** | Position for target keywords | Ahrefs, GSC |
| **CTR** | Clicks ÷ Impressions | GSC |
| **Impressions** | Times site appeared in SERP | GSC |
| **Bounce Rate** | Left without interaction | GA4 |
| **Dwell Time** | Time before returning to SERP | Indirect (GA4 engagement) |
| **Pages Indexed** | Total pages in Google | GSC, site: search |
| **Backlinks** | Total and new/lost | Ahrefs |
| **DR/DA** | Domain authority score | Ahrefs / Moz |
| **Crawl Errors** | Pages Google couldn't crawl | GSC |
| **Core Web Vitals** | LCP, INP, CLS scores | GSC, PageSpeed Insights |

### 14.4 Rank Tracking

- Track keyword positions weekly/monthly
- Monitor rank changes after algorithm updates
- Compare against competitors
- Tools: Ahrefs, SEMrush, AccuRanker, Wincher

---

## 15. SEO Hat Types

### ✅ White Hat — Safe & Sustainable

- **On-Page SEO** — optimizing HTML, content, structure per Google's guidelines
- **Quality Content** — original, helpful, in-depth content for real users
- **Ethical Link Building** — earning links naturally via quality
- **Technical Optimization** — speed, mobile, Core Web Vitals

### ⚠️ Gray Hat — Risky

- **Expired Domain Buying** — acquire domains with existing authority and redirect
- **PBNs (Private Blog Networks)** — network of fake sites to build links (high risk)
- **Paid Links (hidden)** — buying links without disclosure
- **Spun Content** — auto-rewriting content to fake uniqueness
- **Negative SEO** — pointing spam links at competitor's site

### 🚫 Black Hat — Banned

- **Keyword Stuffing** — unnatural keyword density
- **Cloaking** — different content for users vs Googlebot
- **Doorway Pages** — pages made only for a keyword, not for users
- **Hidden Text** — white text on white background
- **Link Farms** — networks of worthless sites just for links
- **Sneaky Redirects** — send bots one place, users another
- **AI Spam Content** — mass AI-generated content with no value (targeted by Helpful Content)

---

## 16. GEO — Generative Engine Optimization

Optimizing your content to appear in **AI-generated answers** from:
- **Google AI Overviews** (SGE) — now showing for most searches
- **ChatGPT** (with Browse/Search)
- **Perplexity AI**
- **Bing Copilot**
- **Claude, Gemini** (when used with search)

> GEO is the next frontier of SEO — AI answers are replacing many traditional SERP clicks

### 16.1 How AI Search Engines Choose Sources

- They pull from pages that **directly answer the question clearly and concisely**
- Prefer **authoritative sources** (high DR, known entities, Wikipedia-cited)
- Pull from **structured, well-formatted content** (headings, lists, clear paragraphs)
- Favor **recent, updated content** (freshness matters even more)
- Trust **E-E-A-T signals** (author credentials, citations, factual accuracy)
- Rely on **entity recognition** — are you a recognized entity in the Knowledge Graph?

### 16.2 GEO Optimization Strategies

#### Answer Questions Directly
- Identify questions in your niche via PAA, Reddit, Quora, forums
- Write a clear, direct answer in the first 1–2 sentences of each section
- Use the question as the heading, answer immediately below
- Keep answers to 40–60 words for snippet-style extraction

#### Structured Content Format
- Use H2/H3 headings that are actual questions
- Use bullet points and numbered lists (AI loves extractable lists)
- Use comparison tables (AI pulls tables frequently)
- Use definition-style content ("X is...")

#### Establish Entity Authority
- Get your brand/entity into Google's Knowledge Graph
- Wikipedia page (if large enough brand)
- Wikidata entity entry
- Consistent brand mentions across authoritative sites
- Google Business Profile, social profiles, press coverage

#### Cite Sources & Be Factual
- Include citations and links to primary data
- Reference studies, statistics with sources
- AI engines trust pages that themselves cite trustworthy sources
- Avoid speculation — be factual and clear

#### E-E-A-T for AI
- Author bios with credentials on every article
- About page clearly stating expertise
- Contact information, privacy policy, terms
- Accurate, up-to-date information (AI checks recency)
- Regular content updates

#### Build Brand Awareness
- Be cited BY other authoritative sources — training data and live search both use this
- Get coverage in major publications, industry blogs
- Podcast appearances, interviews — brand entity recognition
- Use your brand name consistently everywhere

### 16.3 Google AI Overviews (SGE) Specifically

- AI Overviews appear at top — above Position 1
- Show mostly for informational queries
- Sources cited in the overview get a visibility box (thumbnail + link)
- Strategy: target informational queries with comprehensive, structured answers
- Monitor AI Overview appearances in GSC (now tracked in Performance report)

### 16.4 Perplexity & ChatGPT Optimization

- Perplexity reads live web — standard technical SEO applies
- ChatGPT Browse reads web — same approach
- These AIs favor sources already trusted by Google (so strong SEO = strong GEO)
- Ensure pages are crawlable (check robots.txt not blocking Perplexitybot, GPTBot)

**Allow AI crawlers in robots.txt:**
```
User-agent: GPTBot
Allow: /

User-agent: PerplexityBot
Allow: /

User-agent: Google-Extended
Allow: /
```

### 16.5 GEO vs SEO Comparison

| Factor | SEO | GEO |
|--------|-----|-----|
| **Goal** | Rank in SERP | Be cited in AI answer |
| **Traffic Type** | Click-through | Brand mention / direct citation |
| **Format** | Any | Structured Q&A, lists, definitions |
| **Authority Signal** | Backlinks | Entity recognition + backlinks |
| **Success Metric** | Rankings, CTR | AI citation frequency, brand mentions |
| **Content Style** | Keyword-optimized | Question-answering, factual |
| **Crawl** | Googlebot | GPTBot, PerplexityBot, Google-Extended |

### 16.6 Measuring GEO Performance

- **Manually search** target questions in ChatGPT/Perplexity — are you cited?
- Track **branded search volume** in GSC (more brand searches = more AI awareness)
- Monitor **"zero-click" organic traffic drops** — could mean AI Overviews are intercepting
- Use tools: **Semrush AI Toolkit**, **Ahrefs AI Overview tracker**, **SearchPilot**

---

## 17. Tools

### Research & Analysis
| Tool | Use | Cost |
|------|-----|------|
| **Google Search Console** | Rankings, indexing, CWV, errors | Free |
| **Google Analytics 4** | Traffic, behavior, conversions | Free |
| **Ahrefs** | Backlinks, keywords, competitor analysis | Paid |
| **SEMrush** | All-in-one SEO + content + ads | Paid |
| **Moz** | DA/PA metrics, keyword explorer | Freemium |
| **Ubersuggest** | Keywords + backlinks (Neil Patel) | Freemium |
| **Google Keyword Planner** | Keyword volume + CPC | Free (needs Ads account) |
| **Google Trends** | Seasonal trends, rising topics | Free |
| **Answer The Public** | Question-based keyword ideas | Freemium |
| **AlsoAsked** | PAA keyword mapping | Freemium |

### Technical SEO
| Tool | Use | Cost |
|------|-----|------|
| **Screaming Frog** | Full site crawl — finds all technical issues | Freemium |
| **PageSpeed Insights** | CWV + performance suggestions | Free |
| **GTmetrix** | Waterfall performance analysis | Freemium |
| **WebPageTest** | Advanced performance testing | Free |
| **Google Rich Results Test** | Validate schema markup | Free |
| **Schema Markup Validator** | Test structured data (schema.org) | Free |
| **Lighthouse** | Built into Chrome DevTools | Free |

### Content & On-Page
| Tool | Use | Cost |
|------|-----|------|
| **Surfer SEO** | Content optimization vs competitors | Paid |
| **Clearscope** | Keyword and topic coverage grader | Paid |
| **Frase** | AI + SEO content brief creation | Paid |
| **Hemingway Editor** | Readability improvement | Free |
| **Grammarly** | Grammar and clarity | Freemium |

### Local SEO
| Tool | Use | Cost |
|------|-----|------|
| **Google Business Profile** | Local listing management | Free |
| **BrightLocal** | Citation audit, rank tracking | Paid |
| **Whitespark** | Local citation finder | Freemium |
| **Moz Local** | NAP consistency checker | Paid |

### Link Building
| Tool | Use | Cost |
|------|-----|------|
| **Ahrefs** | Backlink analysis, prospecting | Paid |
| **Hunter.io** | Find email addresses for outreach | Freemium |
| **HARO** | Journalist query service for links | Free |
| **Pitchbox** | Outreach automation | Paid |
| **Majestic** | Trust Flow / Citation Flow metrics | Paid |

---

*Complete reference — updated to include GEO for AI search engines*
