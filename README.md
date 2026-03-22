# Dynamics 365 PCF KPI & Scorecard Controls

A collection of **custom PowerApps Component Framework (PCF) controls** for **Dynamics 365 / Dataverse**, designed to display KPIs, engagement metrics, and communication summaries using a consistent, modern card-based UI. The design is heavily based on the original works by Bill Whalen.

All controls are built with **PCF API v1.3.18** using **pac CLI v1.51.1** and share a common visual language:
- Rounded KPI cards
- Gradient / white / transparent backgrounds
- Segoe UI typography
- Lightweight CSS and SVG icons where applicable

<img width="1176" height="552" alt="image" src="https://github.com/user-attachments/assets/2606a96c-78fd-43af-a104-142746cd075d" />


---

## Included Controls

### UPDATE: 4 new controls for showing numerical values have been added. Value Card 1, 2, 3, and 4. Better color control has been added.   
  
### 1. DAEngagementScorecard
A configurable **3-metric engagement scorecard** that calculates an overall score using **weighted**, **average**, or **sum** scoring methods.

**Key features**
- Three required numeric inputs
- Configurable labels, weights, and scoring logic
- Number or percentage formatting
- Inline SVG icons per metric
- Adjustable card height and background style

**Best for:** Engagement scoring, health indexes, composite KPIs

---

### 2. DAKpi1Control
A **single KPI card** with an optional **trend indicator** that compares two values and displays directional arrows.

**Key features**
- Supports numeric and text KPI values
- Optional trend comparison (▲ / ▼ / —)
- Preset color themes
- Gradient, white, or transparent backgrounds
- Lightweight implementation (no localization file)

**Best for:** Simple KPIs with directional context

---

### 3. DAKpiStatControl (v2.2.0)
An enhanced KPI card with **formatting options** and **fully customizable gradient colors**.

**Key features**
- Number, currency, or percentage formatting
- Optional trend indicator
- Free-form color and gradient configuration (hex values)
- Adjustable card height
- Localization support (.resx)

**Best for:** Executive dashboards and branded KPI visuals

---

### 4. DAMultiNumbControl
A **multi-metric KPI card** displaying one primary value and two secondary values in a compact two-row layout.

**Key features**
- Three required bound values
- Supports numeric and text fields
- Clean, icon-free design
- Preset color themes and background styles

**Best for:** Comparing totals vs. historical or secondary metrics

---

### 5. DATripleKpiCard (v1.1.0)
A communication summary card purpose-built for **Phone Calls, Emails, and Meetings**.

**Key features**
- Optional numeric inputs for each communication type
- Inline SVG icons (phone, email, calendar)
- Custom accent color and adjustable height
- Localization support (.resx)

**Best for:** Activity summaries and communication tracking

---

## Feature Comparison

| Feature | Engagement Scorecard | KPI 1 | KPI Stat | Multi Number | Triple KPI |
|---|---|---|---|---|---|
| Bound values | 3 (required) | 1–2 | 1–2 | 3 (required) | 0–3 |
| Text field support | No | Yes | No | Yes | No |
| SVG icons | Yes | No | No | No | Yes |
| Trend indicators | No | Yes | Yes | No | No |
| Format options | Number / % | — | Number / Currency / % | — | — |
| Custom gradients | No | No | Yes | No | No |
| Card height | Configurable | Fixed | Configurable | Fixed | Configurable |
| Localization (.resx) | Yes | No | Yes | No | Yes |

---

## Technical Notes
- Built using **PCF API v1.3.18**
- Developed with **pac CLI v1.51.1**
- Designed for **model-driven apps**
- Compatible with **Dynamics 365 Customer Engagement**
