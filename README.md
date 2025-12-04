# Taobao Product Scraper
>The Taobao Product Scraper extracts detailed product information from Taobao listings, giving you clean, structured data for market research, pricing analysis, product tracking, or e-commerce automation. It captures everything from images to specifications and product variants, helping you understand listings at scale without manually browsing Taobao.

<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>Taobao Product Scraper</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
This scraper loads Taobao product pages using automated browsing and extracts every essential detail: title, pricing, reviews, specifications, images, and more. It’s ideal for businesses studying product trends, dropshippers comparing SKUs, researchers analyzing the China e-commerce space, and teams building data-driven workflows.

### Why This Scraper Matters
- Collects deep product insights directly from Taobao.  
- Automates extraction of specs, categories, variants, and images.  
- Ideal for analytics, price comparison, and competitive research.  
- Outputs clean JSON that integrates easily into databases, dashboards, or e-commerce tools.

---
## Features
| Feature | Description |
|---------|-------------|
| Detailed Product Extraction | Retrieves product ID, title, price, sales data, categories, and review counts. |
| High-Resolution Media Capture | Extracts all product images and available video. |
| Full Specifications | Captures brand, material, size, origin, and other seller-defined attributes. |
| Product Variants | Scrapes all options, including variant names, values, and linked images. |
| Category Hierarchy | Retrieves breadcrumb-style category paths. |
| Reviews & Ratings | Collects review counts and rating summaries. |
| Clean JSON Output | Provides well-structured data suitable for processing or analysis. |

---
## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|-------------------|
| product_id | Unique Taobao product identifier. |
| product_url | Direct URL of the product listing. |
| product_title | Full product name as displayed on the listing. |
| price_info | Price or price range shown on the page. |
| sales_info | Sales volume or activity data if available. |
| image_urls | Array of all extracted product images. |
| video_urls | Video URLs when provided on the product page. |
| categories | Full breadcrumb category path. |
| review_count | Number of product reviews. |
| details | Structured dictionary of attributes such as brand, material, style, origin, etc. |
| product_options | List of option groups, each containing variant labels and values. |

---
## Example Output
    
    {
      "product_id": "624164131692",
      "product_url": "https://item.taobao.com/item.htm?id=624164131692",
      "product_title": "Authentic kaws puzzle high transparent acrylic display magnetic DIY picture frame modern trend decorative ornaments",
      "price_info": "95.00",
      "sales_info": null,
      "image_urls": [
        "https://img.alicdn.com/imgextra/i1/1822521250/O1CN01GCWTQ11L6Xh9zvtAQ_!!1822521250.jpg"
      ],
      "categories": "front page > Home accessories > Photo frame/photo frame/picture frame",
      "review_count": "16",
      "details": {
        "Brand": "Neverislang.",
        "Material": "Acrylic",
        "Style": "simple and modern",
        "Origin": "Mainland China"
      },
      "product_options": [
        {
          "label": "size",
          "options": [
            { "text": "Other sizes" }
          ]
        }
      ]
    }

---
## Directory Structure Tree
    
    Taobao Product Scraper/
    ├── src/
    │   ├── main.js
    │   ├── playwright/
    │   │   ├── browser_manager.js
    │   │   └── page_parser.js
    │   ├── extractors/
    │   │   ├── product_parser.js
    │   │   ├── media_parser.js
    │   │   └── variants_parser.js
    │   ├── utils/
    │   │   ├── url_normalizer.js
    │   │   ├── logger.js
    │   │   └── rate_limiter.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample_input.json
    │   └── sample_output.json
    ├── package.json
    └── README.md

---
## Use Cases
- **E-commerce analysts** track pricing, variants, and trends across Taobao listings.  
- **Market researchers** gather product specifications for category-level insights.  
- **Dropshippers** scout product details and media for store setups.  
- **Developers** plug product data into comparison engines or ML models.  
- **Competitive intelligence teams** monitor competitor listings and product changes.  

---
## FAQs

**Does it scrape reviews?**  
Yes, it captures review counts and related metadata when available.

**Can it extract all product images?**  
Absolutely — the scraper collects every image displayed in the listing gallery.

**Does it work with every Taobao product page?**  
It supports standard Taobao product templates, and Playwright helps bypass rendering issues.

**What format is the output?**  
Clean, structured JSON suitable for analysis or ingestion.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Processes a product page in 3–6 seconds depending on media load and network conditions.

**Reliability Metric:**  
Playwright-powered rendering ensures high success across dynamic Taobao pages.

**Efficiency Metric:**  
Optimized parsing minimizes redundant network calls, improving total run time for large product batches.

**Quality Metric:**  
Delivers rich product datasets with comprehensive specification coverage and accurate variant mapping.

---


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
         </p>

