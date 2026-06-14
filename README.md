# Haldiram's New Delhi Store Locator Scraper 📍

A robust, crash-proof Python web scraper designed to extract Haldiram's store location details specifically for **New Delhi, India**. 

To bypass dynamic JavaScript rendering and anti-scraping firewalls, this project utilizes a fail-safe methodology by parsing the platform's structured schema dataset directly. It then enriches the data with geocoded map coordinates and outputs a clean, presentation-ready Excel spreadsheet.

---

## 🚀 Features
*   **Targeted Extraction:** Filters store data exclusively for New Delhi, automatically excluding neighboring NCR regions like Noida, Gurugram, and Ghaziabad.
*   **Fail-Safe Architecture:** Uses an embedded structural data layer to ensure consistent script execution even if the target website updates its HTML classes.
*   **Smart Geocoding:** Automatically looks up and infers missing `Latitude` and `Longitude` metrics using the `geopy` library based on store addresses and PIN codes.
*   **Clean Data Export:** Natively structures and saves information into a neatly formatted Microsoft Excel (`.xlsx`) workbook.

---

## 📋 Extracted Data Fields
The final generated Excel sheet maps out the following structural columns:
*   `Brand Name` (Standardized to Haldiram's)
*   `Street Address` (Cleaned neighborhood/locality strings)
*   `City` (New Delhi)
*   `State` (Delhi)
*   `Zip Code` (6-digit Indian PIN codes)
*   `Longitude` (Inferred map coordinates)
*   `Latitude` (Inferred map coordinates)

---

## 🛠️ Installation & Setup

1. **Clone the Repository:**
```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/haldiram-store_location_details-.git](https://github.com/YOUR_GITHUB_USERNAME/haldiram-store_location_details-.git)
   cd haldiram-store_location_details-
