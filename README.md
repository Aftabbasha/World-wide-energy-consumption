# World Energy SQL Analysis Project

This project explores global energy consumption, production, CO₂ emissions, GDP, and population across countries and years using structured SQL queries. It aims to extract meaningful business insights and visualize patterns related to sustainability, efficiency, and economic growth.

---

##  Project Objectives

- Analyze total and per capita CO₂ emissions across countries.
- Examine trends in energy production and consumption by energy type.
- Calculate emission-to-GDP ratios to assess energy efficiency.
- Determine energy consumption per capita over the last decade.
- Compare economic output and emissions to draw sustainability insights.

---

## 🗃️ Dataset Description

The dataset consists of 6 interrelated CSV files imported into MySQL, structured to support multi-dimensional analysis:

| Table Name     | Description                                                      |
|----------------|------------------------------------------------------------------|
| `country_3`     | Master dimension table with country names and codes              |
| `emission_3`    | CO₂ emissions data (MMT) including per capita values             |
| `gdp_3`         | GDP in Billion USD (PPP-adjusted) per country per year           |
| `population_3`  | Population data (in thousands)                                   |
| `production_3`  | Energy production by type (likely in Quadrillion BTUs)           |
| `consumption`   | Energy consumption by type (likely in Quadrillion BTUs)          |

---

## 🔗 Schema Overview

This is a **fact constellation schema** where multiple fact tables (emission, GDP, population, production, and consumption) are linked through a shared dimension table `country_3`.

Each fact table includes:
- `country`
- `year`
- One or more quantitative values (e.g., GDP, emission, population)

---

## 🧠 Key Analyses & Metrics

- **Global emission trends** (year-over-year change)
- **Emission-to-GDP ratio** (MMT/Billion USD)
- **Per capita energy consumption**
- **Energy production vs. consumption** comparison
- **High-efficiency and high-emission countries** ranking

---

## 📈 Tools Used

- **MySQL** for database setup and analysis queries
- **Excel** for preliminary data cleaning
- **PowerPoint** for project presentation
- **GitHub** for version control and project sharing
