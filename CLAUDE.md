# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

Data analysis project examining U.S. manufacturing employment trends before and after the "Liberation Day" tariffs (April 2, 2025). Output is a publication-ready Jupyter notebook for GitHub/Reddit.

## Technical Stack

- Python 3.11+
- Core: pandas, matplotlib, requests
- Jupyter notebook as primary deliverable
- BLS Public Data API (https://api.bls.gov/publicAPI/v2/) for employment data

## Key Data

- BLS Series: CES3000000001 (Manufacturing employment)
- Time range: 2015-present, monthly frequency
- API keys via environment variables if using registered tier

## Build Commands

```bash
# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook manufacturing_tariffs_analysis.ipynb
```

## Project Structure

```
manufacturing_tariffs_analysis.ipynb  # Main analysis notebook
requirements.txt                       # Dependencies
figures/                              # Output PNGs (1080x1350px, 4:5 ratio)
```

## Visualization Notes

- Mark April 2, 2025 as "Liberation Day" event line
- Final output: static PNG at 1080x1350px
- Use colorblind-friendly palette
- Include title, subtitle with takeaway, source citation, date pulled
