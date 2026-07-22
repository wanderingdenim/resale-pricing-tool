# Resale Pricing Tool

A personal inventory tool for secondhand/vintage clothing resale. Given photos
of an item, it identifies the brand, style, size, and condition, researches
comparable sold and active listings across marketplaces, and generates an
optimized listing title, description, and price recommendation.

## Status

Live, in personal production use — not a public service or multi-tenant
application. Single user, one internal Flask application.

## eBay API usage

- **Browse API** — live, in active use for real-time active-listing search
  as part of comparable-pricing research for each item processed.
- **Marketplace Insights API** — requested, to replace an unofficial
  fallback (parsing eBay's own public Seller Hub research pages) with the
  official, sanctioned method for historical sold-price data.

All eBay API calls are application-level (`client_credentials` grant)
requests against public catalog/listing data only. No eBay user account
data is stored, accessed, or processed. Not affiliated with the eBay
Partner Network.
