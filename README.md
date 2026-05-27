# virtual-care-state-expansion
An interactive dashboard prototype for evaluating U.S. state expansion opportunities and tracking launch performance for a virtual elderly care platform serving older adults living alone.

The project combines a weighted state attractiveness model, an interactive U.S. map, launch performance dashboards, and an Excel upload feature for refreshing KPI data.

## Live Demo

View the deployed version here: https://virtual-care-state-expansion.netlify.app/

## Project Overview

This prototype was built to translate a strategic market expansion framework into an interactive decision-support tool. It helps evaluate which U.S. states may be most attractive for launching a virtual elderly care coordination service, based on market size, care need, payer relevance, workforce availability, and competitive saturation.

The tool includes three main modules:

1. **Expansion Model**
   - Ranks all 50 states using a weighted scoring framework
   - Visualizes state attractiveness through a ranked list and interactive U.S. map
   - Shows score breakdowns by factor

2. **Launch Dashboard**
   - Tracks leading and lagging performance indicators after market launch
   - Includes both national aggregate and state-level views
   - Allows users to add launched states and compare performance across markets

3. **Data Upload**
   - Supports Excel upload to refresh dashboard metrics
   - Includes an expected template format
   - Updates KPI cards and charts automatically after upload

## Why This Matters

For a virtual elderly care platform, state expansion should not be driven by population size alone. The best markets are likely those with a large addressable elderly population, high care coordination needs, relevant payer pools, feasible workforce conditions, and manageable competitive dynamics.

This dashboard turns those qualitative and quantitative considerations into a practical operating tool that can support market prioritization, launch planning, and post-launch performance management.

## Scoring Framework

The expansion model evaluates each state across five factors:

| Factor | Weight | Rationale |
|---|---:|---|
| Population 65+ living alone | 50% | Direct measure of addressable market size |
| Traditional Medicare beneficiaries | 20% | Proxy for payer relevance and distribution potential |
| Multiple chronic condition prevalence among 65+ | 10% | Proxy for care coordination need |
| Community Health Worker supply | 10% | Signal of care workforce availability |
| Home health market saturation | 10% | Directional proxy for competitive intensity |

Each component is normalized against the highest observed state value, then weighted to create a composite attractiveness score.

## Key Features

- Interactive 50-state ranking
- U.S. heat map with hover-based score breakdown
- National launch performance dashboard
- State-level KPI dashboard
- Add/remove launched markets
- Excel upload workflow for refreshing dashboard data
- Downloadable dashboard data template
- KPI tracking across activation, engagement, NPS, subscription length, gross margin, revenue, and workforce capacity

## Tech Stack

- HTML
- CSS
- JavaScript
- Chart.js
- D3.js
- TopoJSON
- SheetJS / XLSX
- Netlify for deployment

## File Structure

```text
virtual-elderly-care-platform/
├── index.html
├── README.md
└── screenshots/
    ├── expansion-model.png
    ├── launch-dashboard.png
    └── data-upload.png
