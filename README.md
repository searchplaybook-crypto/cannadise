# Cannadise Eldos — Landing Page Handover

## 🧩 Overview
This document defines the **Cannadise Cannabis Club Eldos** landing page structure, styling, and schema for deployment within the GSE‑optimized framework.  
It includes HTML layout, CSS layering logic, and schematic notes for ingestion by coding LLMs.

---

## 🏗️ Page Architecture
### Sections
1. **Header (Hero Block)**
   - Cannadise Eldos logo centered.
   - Tagline: “Premium Cannabis Lifestyle Brand.”
   - CTA button: “Learn More.”
   - CSS: radial gradient (dagga green → $100 blue), metallic text shadow.

2. **Map Section**
   - Embedded Google Maps iframe centered on Eldorado Park.
   - Schema: LocalBusiness with Eldos coordinates.
   - CSS: rounded corners, subtle box‑shadow.

3. **FAQ Section**
   - Three collapsible items:
     - What makes Cannadise Eldos unique?
     - Where are you located?
     - Do you offer delivery or events?
   - CSS: gradient buttons (green → blue), hover transitions, hidden answer panels.

4. **Footer**
   - Text: “© 2026 Cannadise Cannabis Club Eldos.”
   - CSS: dark background, silver typography.

---

## 🎨 CSS Layering Logic
| Layer | Description | Colors |
|-------|--------------|--------|
| **Primary Gradient** | Radial blend for hero section | Dagga Green `#1B5E20` → $100 Blue `#0077B6` |
| **Accent Gradient** | Hover states and CTA buttons | Sunset Gold `#FDB813` → Platinum Silver `#E5E4E2` |
| **Typography** | Headings: Montserrat ExtraBold<br>Body: Roboto Medium | Silver `#E5E4E2` |
| **Background** | Linear gradient base | Black `#000000` → Charcoal `#111111` |

---

## 🗺️ Schema Integration
```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Cannadise Cannabis Club Eldos",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Eldorado Park",
    "addressLocality": "Johannesburg",
    "addressRegion": "Gauteng",
    "postalCode": "1811",
    "addressCountry": "ZA"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": -26.2700,
    "longitude": 27.9000
  },
  "url": "https://wemustcreateza.my.canva.site/",
  "telephone": "+27 82 000 0000",
  "openingHours": "Mo-Su 09:00-21:00"
}
