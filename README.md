# Enterprise Hardware Catalog - Data & Analytics Pipeline

An end-to-end data engineering and analytics pipeline engineered to clean, enrich, categorize, and extract business intelligence from an enterprise hardware infrastructure dataset. The project demonstrates advanced data architecture capabilities using **Python (Pandas/Matplotlib)** and **SQL (DuckDB)**.

---

## Repository Architecture

This repository operates as a self-contained environment structured with the following core assets:

* **`notebook.ipynb`** - The primary engineering pipeline. Contains structured documentation, sequential code execution blocks, inline documentation, and advanced analytical queries.
* **`hardware_catalog_clean.csv`** - The foundational output generated after the ingestion and cleansing phase (Task 1).
* **`assignment_output.csv`** - The enriched feature-engineered dataset containing derived financial indicators and regional tax compliance mapping (Task 2).
* **`taxonomy_output.csv`** - The subset data architecture isolating indexable infrastructure entries into a structured 3-level catalog hierarchy (Task 3.1).

---

## Core Engineering Highlights

### 1. Programmatic Data Cleansing & Audit Ledger
* Developed a dynamic **Audit Tracking System** within the cleaning cycle to monitor and report metadata modification flags (null conversions, out-of-bounds metrics, and dropped records).
* Built an internal **Geographical Knowledge Base (Source of Truth)** to identify structural anomalies, execute cross-column data imputation between warehouse identifiers and location fields, and enforce syntax standards across mixed inputs.
* Applied explicit spatial boundary constraints to handle edge cases, multi-format unknown string sequences, numeric absolute adjustments, and strict chronological integrity limits on asset record lifecycles.

### 2. Feature Engineering & Dynamic Financial Modeling
* Parsed complex, unstructured alphanumeric sequences within raw detail attributes into discrete, isolated structural groups.
* Derived critical financial evaluation models, mapping standalone margin profiles alongside gross physical inventory valuations.
* Fabricated conditional tax functions integrating layered logic parameters, compound corporate tax surcharges, and localized volume thresholds tied to specific regional facility hubs.

### 3. Structural Taxonomy & High-Performance SQL Engine
* Architected a rigid **3-Level Product Taxonomy Engine** (*Category ➔ Sub-category ➔ Component Type*) powered by pattern recognition to segment unclassified computing hardware rows.
* Implemented **DuckDB integration** to execute highly optimized relational queries directly over memory-resident DataFrames, bridging Python and analytical SQL environments.
* Utilized complex **Regular Expressions (`regexp_extract`)** to target, parse, and clean unstructured text fields, extracting physical storage and memory profiles into standardized numerical database columns.

### 4. Density Distribution Visualization
* Engineered a dynamic multi-dimensional bubble chart utilizing coordinate mapping and scale-intensity density to evaluate geographic inventory concentration zones across operational infrastructure clusters.

---

## Execution Guide

### Environment Prerequisites
To run the analysis and reproduce the data states across the pipeline, ensure the following core dependencies are available in your workspace:
```bash
pip install pandas numpy matplotlib duckdb
