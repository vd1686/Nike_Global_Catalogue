# Nike // Global Merchandise & Pricing Performance Dashboard

An end-to-end data analytics project that transforms raw, web-scraped global e-commerce product catalog data into an executive-ready analytics solution. This project showcases a complete data lifecycle pipeline: moving from programmatic data extraction and engineering in Python to high-end UI/UX application in Power BI.

<video src="https://github.com/user-attachments/assets/7f78f3eb-1455-4461-9872-9f8c56359528" width="100%" controls autoplay loop muted></video>

---

## 📂 Repository Contents

*   `nike_global_final.csv` — Final, structured CSV exported from the Python pipeline.
*   `Nike_Global_Catalogue.ipynb` — Google Colab notebook containing EDA & processing code.
*   `Nike_Global_Catalogue.pbit` — Polished Power BI Dashboard template file.
*   `README.md` — Technical project documentation.
*   `nike_logo.jpg` — Logo Image for Dashboard.

---

## 🛠️ Phase 1: Data Engineering & EDA (Python)

The raw web-scraped catalog dataset contained several data quality issues, unformatted text metrics, and high-cardinality categorical variables typical of raw e-commerce automated scrapes. 

Using **Python** within a **Google Colab** environment, the following engineering pipeline was executed:
*   **Target Segment Standardization:** Resolved messy, multi-tagged categorization string variables (e.g., combined gender parameters like `MEN|WOMEN` and trailing null blocks) by parsing core data boundaries into distinct, clean target demographics (*Men, Women, Boys, Girls*).
*   **Anomalous Outlier Handling:** Programmatically isolated pricing discrepancies and extreme distribution values to prevent skewing statistical aggregations.
*   **Schema Optimization:** Cast semantic data types correctly, computed base metrics, and exported a high-performance flat schema optimized for fast loading into downstream Business Intelligence tools.

---

## 🎨 Phase 2: UI/UX & Dashboard Architecture (Power BI)

Moving intentionally away from cluttered, default-styled analytics templates, this phase applied strict design constraints to align the interactive workspace with a premium corporate identity.

### Key Visual & Analytical Features:
*   **Intentional Brand Aesthetic:** Honored Nike's digital design language by engineering a sleek, minimal, monochromatic color palette.
*   **Geometric Grid System:** Standardized sharp, $90^\circ$ geometric container lines to establish an authoritative visual hierarchy and eliminate negative space fragmentation.
*   **Typographic Scannability:** Applied bold, high-contrast headline KPI metrics for immediate executive consumption, completely removing redundant chart axes and distracting background gridlines.
*   **Layout Integrity:** Calibrated tight visual constraints, adjusting layout margins to ensure critical categorical data strings and tooltips display flawlessly without truncation or ellipsis truncation bugs.

---

## 🔧 How to Run Locally

1. **Review Data Cleansing:** Open `Nike_Global_Catalogue.ipynb` via Google Colab or your local Jupyter environment to check the Python processing script.
2. **Deploy Template:** Download the `Nike_Global_Catalogue.pbit` file and open it using Power BI Desktop. When prompted, map the data connection to the `clean_nike_data.csv` file on your local machine.
