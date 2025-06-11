# 📍 Google Maps Email Scraper (n8n Workflow)

This n8n automation extracts business contact data — including emails — from Google Maps search results. It's perfect for generating local B2B leads for marketing or outreach campaigns.

## 🔧 Use Case

Extract verified business emails and details from Google Maps to:

- 📩 Build cold email campaigns
- 📊 Create segmented lead lists
- 📍 Find local service providers
- 📞 Generate contact databases for agencies

## 🧠 How It Works

1. **Input Search Keywords**  
   Provide search terms and target locations (e.g., "Yoga Studios in Berlin").

2. **Maps Scraping**  
   A headless browser (via Puppeteer or Browserless API) is used to visit Google Maps, scroll through results, and extract:

   - 📛 Business Name  
   - 🌍 Address  
   - 📞 Phone  
   - ✉️ Email (from website/contact page)
   - 🔗 Website

3. **Email Validation**  
   Optional step: validate and filter only working emails.

4. **Output Delivery**  
   Save data to:
   - Google Sheets
   - CSV file
   - Email
   - Telegram channel

## 🛠 Tech Stack

- [n8n](https://n8n.io/)
- Puppeteer / Browserless API
- Google Maps search engine
- Email Validation API (optional)
- Google Sheets / CSV
- Telegram or SMTP (optional)

## 📁 Example Flow Nodes

- Webhook (start with query: location + keyword)
- HTTP Request (Browserless scrape or external API)
- Data Split / Clean (Extract email from business website)
- Google Sheets / Email / Telegram

---

## ⚠️ Legal Note

- Ensure compliance with local laws (e.g., GDPR in EU) before using contact data for cold outreach.
- Best for **B2B** and **publicly listed contact information**.

---

## 🧪 Output Example

Search: "Tattoo Studios in Hamburg"
Result:

InkHaus Berlin | info@inkhaus.de | https://inkhaus.de | Berlin

TattooCraft | kontakt@tattoocraft.de | https://tattoocraft.de | Berlin
...
→ Leads.csv

## 📬 Contact

Created by [Serhii Litus](https://www.upwork.com/freelancers/~016b54c2291f96bd7d)  
Let me help you build lead gen workflows that scale 🚀
