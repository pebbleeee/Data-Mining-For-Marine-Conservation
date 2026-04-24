# 📂 Dataset Instructions

The raw dataset is not included in this repository due to its size (~247MB). Follow the steps below to download it from the AODN portal.

---

## 🌐 Data Source

**Reef Life Survey (RLS) Australia Ecosystem Subset (2016 to 2026)**
Provider: [Australian Ocean Data Network (AODN) Portal](https://portal.aodn.org.au/)

The AODN portal provides open access to Australian ocean data. No account is required.

---

## 📥 Download Steps

1. Go to [https://portal.aodn.org.au/](https://portal.aodn.org.au/)
2. Click **Biological** under the parameter categories
3. Click **Ocean Biota**
4. Click **Abundance**
5. You will see **IMOS - National Reef Monitoring Network Sub-Facility - Global Reef Fish Abundance and Biomass** in the results
6. Select **Australia** as the region
7. Set the date range to **2016 to 2026**
8. Download the dataset as a CSV file

---

## ⚠️ Important Notes

**Results may vary slightly over time.** The AODN portal updates this dataset continuously, and 2026 data is still being added as of the time this project was completed. If you download the dataset at a later date, your species counts, sparsity, and association rules may differ slightly from the results in this notebook.

**Larger timeframes are possible.** If you want to extend the analysis beyond 2016 to 2026, the portal supports broader date ranges. Keep in mind that expanding the timeframe will increase dataset size and may affect sparsity and network structure.

---

## 🔧 Setup

Once downloaded, place the CSV file at the path specified in **Section 1** of `main_notebook.ipynb`:

```python
path = "/content/IMOS_-_National_Reef_Monitoring_Network_Sub-Facility_-_Global_reef_fish_abundance_and_biomass.csv"
```

The file ingestion cell skips the first **71 lines** of AODN portal metadata automatically, so no manual preprocessing is needed before running the notebook.
