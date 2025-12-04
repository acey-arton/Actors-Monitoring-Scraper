# Actors Monitoring Scraper
>This system monitors actor and task performance, compares runs, and generates structured monthly reports so you can keep track of runtime behavior, costs, and operational trends. It automates the heavy lifting of collecting performance data, filtering actors, and delivering insights by email—ideal for teams managing multiple automated workflows.


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
  If you are looking for <strong>Actors Monitoring Scraper</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
The Actors Monitoring Scraper analyzes actor run history, aggregates metrics over defined time ranges, and produces polished Excel reports. It’s built for developers, automation managers, and analysts who need a reliable way to observe performance patterns, track costs, and maintain operational oversight without digging manually through logs.

### Why This Matters
- Compares any two actor or task runs to highlight differences.
- Generates detailed monthly reports across periods from 1 to 24 months.
- Delivers refined insights in multiple categories including geography, runtime, and efficiency.
- Provides email alerts so your reporting always stays automated and on time.
- Applies smart filtering to include or exclude actors based on name patterns.

---
## Features
| Feature | Description |
|---------|-------------|
| Run Comparison | Compare the latest two runs or any two selected runs for detailed deltas. |
| Monthly Reporting | Generate Excel reports covering any period between 1 and 24 months. |
| Direct Actor Runs | Fetches run data directly from actors for efficiency and simplicity. |
| Email Delivery | Sends reports automatically to chosen recipients. |
| Filtering Controls | Include or exclude actors and tasks using pattern-based filters. |
| Performance Analytics | Tracks runtime, costs, efficiency, and error trends. |
| Geographic Categorization | Breaks down run data by region or country. |
| Excel Export | Creates multi-sheet, professionally formatted Excel reports. |

---
## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|-------------------|
| actorName | Name of the actor being monitored. |
| runId | Unique identifier of a monitored run. |
| runtime | Total execution time for the run. |
| cost | Cost associated with running the task or actor. |
| region | Geographic region tied to the run. |
| period | Monthly period covered in the report. |
| comparison | Differences between two runs in key metrics. |
| sheetData | Structured Excel-ready output segmented by category. |
| filtersApplied | Filters used to include or exclude tasks and actors. |

---
## Example Output
    
    [
      {
        "actorName": "my-actor",
        "runId": "t4F89Ds",
        "runtime": 322,
        "cost": 0.45,
        "region": "US",
        "period": "2024-02",
        "comparison": {
          "previousRun": "t4F89Cr",
          "runtimeDelta": -14,
          "costDelta": -0.05
        },
        "sheetData": {
          "summary": { "runs": 10, "averageRuntime": 300 },
          "regions": [{ "region": "US", "count": 8 }]
        },
        "filtersApplied": ["include:my"]
      }
    ]

---
## Directory Structure Tree
    
    Actors Monitoring/
    ├── src/
    │   ├── main.js
    │   ├── services/
    │   │   ├── email_validation_service.js
    │   │   ├── api_client_wrapper.js
    │   │   ├── log_helper.js
    │   │   ├── input_validator.js
    │   │   ├── filtering_service.js
    │   │   └── sheet_factory.js
    │   ├── modules/
    │   │   ├── run_comparison.js
    │   │   ├── monthly_report.js
    │   │   └── email_notifications.js
    │   ├── utils/
    │   │   └── formatters.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample_input.json
    │   └── sample_output.json
    ├── package.json
    └── README.md

---
## Use Cases
- **Automation engineers** track performance drift over time to maintain stable actor workflows.  
- **Data teams** analyze cost and runtime trends across large sets of automated tasks.  
- **Ops managers** rely on scheduled reports to keep stakeholders informed.  
- **Developers** debug performance differences by comparing runs directly.  
- **Organizations** maintain visibility into regional or large-scale workflow performance.

---
## FAQs

**Can I compare any two runs manually?**  
Yes, you can select any pair of runs rather than relying only on recent ones.

**Does it support automated report delivery?**  
The system can send Excel reports by email to any configured recipients.

**Can I limit the monitoring to only certain actors?**  
Yes, with include/exclude pattern matching you can control which actors and tasks are monitored.

**What metrics are included in the reports?**  
Runtime, cost, efficiency indicators, regional breakdowns, and multi-sheet summaries.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Processes actor run histories in seconds, even across multi-month periods.

**Reliability Metric:**  
Maintains a stable success rate above 97% for API fetches thanks to a unified client wrapper and retry logic.

**Efficiency Metric:**  
Reduces repeated logic through a modular service layer, cutting overhead and improving processing speed.

**Quality Metric:**  
Generates well-structured, cleanly formatted Excel sheets with consistent styling across all report types.

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


