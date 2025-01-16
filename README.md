# README for Customer Segmentation by Spending Patterns Project

## Overview

This repository contains the analysis and deliverables for a data analytics project aimed at understanding client spending patterns for Company XYZ, a wholesale distributor in Portugal. The project identifies meaningful client segments to help XYZ optimize inventory management, improve customer service, and drive strategic business decisions.

The analysis uses the Wholesale Customers dataset, which includes annual spending data for 440 clients across six product categories, categorized by channel and region. The project outputs include a technical document (generated with RMarkdown) and an executive summary.

---

## Repository Structure

### Files and Directories

- **`data/`**
  - `Wholesale_customers_data.csv`: The dataset containing spending information for 440 clients.

- **`analysis/`**
  - `Technical_Doc.pdf`: A detailed technical report generated in RMarkdown, documenting the full analysis process, code, and results.

- **`docs/`**
  - `Executive_Summary.pdf`: A managerial summary translating the technical insights into actionable business recommendations.

- **`scripts/`**
  - `analysis_script.Rmd`: The RMarkdown script used for data preprocessing, clustering, and visualization.

---

## Key Objectives

1. **Understand Spending Patterns:**
   - Analyze annual spending data across six product categories.
   - Identify meaningful client segments using clustering techniques.

2. **Generate Actionable Insights:**
   - Provide strategic recommendations to optimize inventory, logistics, and customer service based on identified segments.

---

## Methodology

### Data Preparation
- **Outlier Detection:** Identified and removed clients with multiple outliers to improve clustering accuracy. High spenders were separated into a distinct cluster.
- **Normalization:** Standardized spending data for clustering.

### Analysis
- **Clustering:** Applied K-Means clustering to segment clients based on their spending patterns. Chose the optimal number of clusters (k = 4) using silhouette scores and visual inspection.
- **Visualization:** Used cluster plots to analyze and validate segment characteristics.

### Results
Four distinct client segments were identified:
1. **Suburban Retailers** - High spenders on milk, grocery, and detergents.
2. **Small Horeca Businesses** - Low spenders across all categories.
3. **Upscale Horeca Buyers** - High spenders on fresh and frozen products.
4. **High-Value Clients** - Outliers with extremely high spending across all categories.
