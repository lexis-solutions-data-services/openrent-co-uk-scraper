# 🏠 OpenRent.co.uk Scraper

![OpenRent Scraper](https://i.ibb.co/dsdPTbcF/openrent-cover.png)

This Apify actor allows you to scrape rental property listings from [https://www.openrent.co.uk/](https://www.openrent.co.uk/), one of the UK's leading rental property platforms. Extract comprehensive property data including prices, locations, descriptions, amenities, and contact information — perfect for rental market research and property analysis.

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/DevbkY3adMTBuoECt-actor-4fg5axInasUygZz5g-CP16XJE8Od-id8PMqSkH3_1758525614053.png" alt="Openrent.co.uk Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/openrent-co-uk-scraper" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>


---


## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `1.0.2` |
| **Last Update** | Dec 1, 2025 |

---



## 💻 Integration Examples

This repository includes example code showing how to integrate the `openrent-co-uk-scraper` actor into your projects.

You can find example implementations in the [`examples/`](./examples) folder:
- **TypeScript/JavaScript**: See [`examples/typescript/`](./examples/typescript) for a complete TypeScript example
- **Python**: See [`examples/python/`](./examples/python) for a complete Python example

Each example includes:
- Ready-to-use code templates
- Setup instructions
- Documentation links

---


## 🚀 Key Features

- 🔎 Scrape listings from OpenRent search pages or individual property detail pages
- 📍 Enhanced location data with transport links and walking times
- 💰 Accurate pricing extraction (monthly rent PCM and weekly PW rates)
- 🏠 Property specifications (bedrooms, bathrooms, max tenants, EPC ratings)
- 👥 Tenant preferences (student-friendly, pets allowed, families, smokers, DSS)
- 🏢 Landlord information (response rates, response times, contact details)
- 📅 Availability details (available from date, minimum tenancy)
- 🚇 Transport connectivity - Nearby stations with walk times and transport types
- 🗺️ Static map images for location visualization
- 🌐 Proxy support for stable, anonymous scraping
- 🖼️ High-resolution property image URLs extraction

---

## ❓ Why Use This Actor

- ✅ **Fast & Reliable**: fetches thousands of listings in a matter of minutes
- ✅ **Rich Transport Data**: Get nearby stations, walk times, and transport types
- ✅ **Accurate Pricing**: Extract both monthly (PCM) and weekly (PW) rates
- ✅ **Comprehensive**: Full property details, landlord info, and tenant preferences

---

## 👥 Who Is This Actor Suitable For?

- 🏘️ Property managers and letting agents
- 📈 Rental market researchers and analysts
- 🧠 Data scientists studying housing markets
- 🧰 Developers building property search platforms
- 📚 Academic researchers studying rental markets
- 💼 Real estate investors and landlords

---

## 📥 Input Schema

The actor accepts the following input parameters:

### Search Page URLs

```json
{
  "startUrls": [
    {
      "url": "https://www.openrent.co.uk/properties-to-rent/greater-london?term=Greater%20London"
    }
  ],
  "maxItems": 50,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

### Direct Property Detail URLs

```json
{
  "startUrls": [
    {
      "url": "https://www.openrent.co.uk/property-to-rent/london/2-bed-flat-buckingham-street-wc2n/2485701"
    },
    {
      "url": "https://www.openrent.co.uk/2485701"
    }
  ],
  "maxItems": 10,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

### Input Parameters

- **startUrls** (required): Array of OpenRent URLs to scrape. Supports both:
  - **Search page URLs**: Extract multiple properties from search results
  - **Detail page URLs**: Extract single property details directly (format: `openrent.co.uk/{propertyId}`)
- **maxItems** (optional): Maximum number of properties to scrape (default: 10, max: 10,000)
- **proxyConfiguration** (optional): Proxy settings for anonymous scraping

---

## 📤 Output Schema

Each scraped property returns comprehensive structured data with **direct detail page extraction**:

```json
[
  {
    "id": "2612802",
    "title": "1 Bed Flat, Whitehall, SW1A",
    "price": 3599,
    "pricePerWeek": 830.54,
    "location": "London, SW1A",
    "description": "Key features: Modern 1-bedroom apartment in prime central London location. Fully furnished with integrated appliances and excellent transport links...",
    "images": [
      "https://imagescdn.openrent.co.uk/listings/2612802/o_1j3lqq1trgnu1d2f140n1scv1a967.JPG",
      "https://imagescdn.openrent.co.uk/listings/2612802/o_1j3lqpnvuhjr2vh1uv41c5v1jbq0.JPG"
    ],
    "listing_url": "https://www.openrent.co.uk/2612802",

    "bedrooms": 1,
    "bathrooms": 1,
    "maxTenants": 2,
    "deposit": 4384.61,
    "billsIncluded": false,

    "features": {
      "garden": false,
      "parking": false,
      "fireplace": false,
      "furnishing": "Furnished",
      "epc_rating": "B"
    },

    "tenantPreferences": {
      "student_friendly": true,
      "families_allowed": true,
      "pets_allowed": true,
      "smokers_allowed": true,
      "dss_income_accepted": false
    },

    "status": "Available",
    "availableFrom": "Today",
    "minimumTenancy": "12 Months",

    "landlordName": "Property Manager",
    "landlordResponseRate": "99%",
    "landlordResponseTime": "Within 3 Days",

    "imageCount": 12,
    "propertyReference": "2612802",

    "transportLinks": [
      {
        "type": "Underground",
        "name": "Charing Cross",
        "walkTime": "~3 min. walk"
      },
      {
        "type": "National Rail",
        "name": "London Charing Cross",
        "walkTime": "~4 min. walk"
      },
      {
        "type": "Underground",
        "name": "Embankment",
        "walkTime": "~7 min. walk"
      },
      {
        "type": "Underground",
        "name": "Westminster",
        "walkTime": "~8 min. walk"
      }
    ],

    "mapImage": "https://imagescdn.openrent.co.uk/staticMapPhotoForProperty/26128020409202595914822.JPG"
  }
]
```

### Output Fields

**Core Property Data:**

- `id`, `title`, `price` (monthly PCM), `pricePerWeek` (weekly PW)
- `location`, `description`, `listing_url`, `images`

**Property Specifications:**

- `bedrooms`, `bathrooms`, `maxTenants`
- `deposit`, `billsIncluded`

**Property Features:**

- `features.garden`, `features.parking`, `features.fireplace`
- `features.furnishing`, `features.epc_rating`

**Tenant Preferences:**

- `tenantPreferences.student_friendly`, `tenantPreferences.families_allowed`
- `tenantPreferences.pets_allowed`, `tenantPreferences.smokers_allowed`
- `tenantPreferences.dss_income_accepted`

**Availability & Landlord:**

- `status`, `availableFrom`, `minimumTenancy`
- `landlordName`, `landlordResponseRate`, `landlordResponseTime`
- `imageCount`, `propertyReference`

**🚇 Transport & Location (NEW):**

- `transportLinks[]` - Array of nearby transport with type, name, and walk time
- `mapImage` - Static map image URL for location visualization

---

## 🔍 Looking to Scrape Real Estate Websites?

In addition to this actor, you can explore our suite of dedicated scrapers tailored for other popular property listing platforms. Each scraper is optimized for its target site to ensure accurate, efficient, and high-performance data extraction.

| Scraper                                                                                          | Country        | Description                                                                                       |
| ------------------------------------------------------------------------------------------------ | -------------- | ------------------------------------------------------------------------------------------------- |
| [FlatFox.ch Properties Scraper](https://apify.com/lexis-solutions/flatfox-ch-properties-scraper) | Switzerland    | Scrape real estate listings, including prices, locations, and property details from FlatFox.ch.   |
| [Boligsiden.dk Scraper](https://apify.com/lexis-solutions/boligsiden-dk-scraper)                 | Denmark        | Extract housing data from Boligsiden.dk, including listings, prices, and property specifications. |
| [Pararius.nl Scraper](https://apify.com/lexis-solutions/pararius)                                | Netherlands    | Collect property listings and rental data from Pararius.nl for the Dutch real estate market.      |
| [Onthemarket.com Scraper](https://apify.com/lexis-solutions/onthemarket-com-scraper)             | United Kingdom | Gather UK housing listings, prices, and property details from Onthemarket.com.                    |
| [Seloger.com Scraper](https://apify.com/lexis-solutions/seloger-scraper)                         | France         | Scrape property advertisements, pricing, and location details from the French site Seloger.com.   |

Explore these solutions to expand your data collection capabilities across property and real estate websites.

---

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a [certified Apify Partner](https://apify.com/partners/find). We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:scraping@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)

## Support Our Work 💝

If you're happy with our work and scrapers, you're welcome to leave us a company review [here](https://apify.com/partners/find/lexis-solutions/review) and leave a review for the scrapers you're subscribed to. It will take you less than a minute but it will mean a lot to us!

Image Credit: https://www.openrent.co.uk/
