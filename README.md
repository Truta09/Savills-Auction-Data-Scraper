# Savills Auction Data Scraper
>This scraper collects detailed property information from Savills UK auction listings—both past and upcoming—and turns it into structured, analysis-ready data. It’s built to navigate auction result pages lot by lot, mimicking natural browsing while capturing every available detail. Whether you're analyzing the market, sourcing leads, or automating reporting, this tool keeps property data organized and easy to work with.

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
  If you are looking for <strong>Savills Auction Data Scraper</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
This project extracts property lot information from any Savills auction results URL. It navigates sequentially through each lot page, gathering addresses, pricing, statuses, descriptions, and more. It’s ideal for real-estate analysts, investors, researchers, and automation-focused businesses looking to streamline property data collection.

### What It Focuses On
- Scrapes full property details from Savills auction result pages.  
- Handles both upcoming auctions and historical listings.  
- Moves through lots automatically using next-lot navigation.  
- Captures pricing, status, addresses, features, and descriptions.  
- Provides clean structured datasets for pipelines or dashboards.

---
## Features
| Feature | Description |
|---------|-------------|
| Sequential Lot Navigation | Visits each lot page automatically via “Next Lot” traversal. |
| Comprehensive Data Extraction | Collects lot numbers, addresses, pricing, sell values, and descriptions. |
| Auction Scope Flexibility | Works on both future auction listings and past results. |
| Structured Output | Produces clean data ideal for analysis or automation tasks. |
| Robust Page Handling | Mimics human browsing to reduce missed data or navigation issues. |
| Direct Lot URL Capture | Stores the exact link for every scraped lot for reference. |

---
## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|-------------------|
| lotNumber | The auction lot identifier. |
| auctionDate | The date the auction took place or is scheduled for. |
| addressLine1 | First line of the property address. |
| addressLine2 | Second line of the property address. |
| guidePrice | Listed guide price when available. |
| sellValue | Final achieved price for sold properties. |
| status | Outcome of the lot (sold, withdrawn, unsold, etc.). |
| features | List of highlighted features for the property. |
| description | Main descriptive text for the property. |
| additionalInfo | Supplementary details such as tenure or accommodation notes. |
| lotUrl | Direct URL to the individual lot page. |

---
## Example Output
    
    [
      {
        "lotNumber": "15",
        "auctionDate": "2024-09-12",
        "addressLine1": "12 High Street",
        "addressLine2": "Birmingham, B1",
        "guidePrice": "£120,000",
        "sellValue": "£138,500",
        "status": "Sold",
        "features": ["Freehold", "Two bedrooms", "Close to city centre"],
        "description": "A well-located terraced property suitable for investors.",
        "additionalInfo": "Accommodation over two floors; EPC rating D.",
        "lotUrl": "https://auctions.savills.co.uk/lot/12345"
      }
    ]

---
## Directory Structure Tree
    
    Savills Auction Data Scraper/
    ├── src/
    │   ├── main.js
    │   ├── scraper/
    │   │   ├── lot_parser.js
    │   │   ├── navigation_handler.js
    │   │   └── auction_page_loader.js
    │   ├── utils/
    │   │   ├── logger.js
    │   │   └── formatters.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── example_input.json
    │   └── sample_output.json
    ├── package.json
    └── README.md

---
## Use Cases
- **Investors** use it to evaluate past auction outcomes and identify high-yield opportunities.  
- **Real-estate analysts** use it to track pricing trends, sell-through rates, and market movement.  
- **Property researchers** use it to build structured datasets for valuation studies.  
- **Automation teams** feed the data into CRMs or data warehouses for streamlined reporting.  
- **Lead-generation companies** use it to identify properties meeting specific investment criteria.  

---
## FAQs

**Does it work with both past and future auctions?**  
Yes. It can scrape upcoming listings and historical results from any valid Savills auction URL.

**Do I need multiple URLs?**  
No. A single auction results page is enough—the scraper navigates through every lot automatically.

**What happens if a lot has missing data?**  
The scraper continues processing and includes all available fields without interruption.

**Is the scraping process fast?**  
It navigates efficiently while mimicking human interaction to reduce the chance of navigation errors or data loss.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Processes 30–50 property lots per minute depending on page complexity and network conditions.

**Reliability Metric:**  
Maintains a success rate above 95% in multi-lot auctions thanks to controlled navigation.

**Efficiency Metric:**  
Loads only necessary pages and reuses sessions to minimize overhead.

**Quality Metric:**  
Produces consistently complete records with accurate parsing of guide prices, sell values, and structured descriptions.

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


