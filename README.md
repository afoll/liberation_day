# Manufacturing Employment & Liberation Day Tariffs Analysis

Analysis of U.S. manufacturing employment trends before and after the "Liberation Day" tariffs announced April 2, 2025.

## Data Source

- **Bureau of Labor Statistics (BLS)** Current Employment Statistics (CES)
- Series: CES3000000001 (Manufacturing employment, seasonally adjusted)
- API: https://api.bls.gov/publicAPI/v2/
- Time range: 2015-present, monthly frequency

## Setup

```bash
# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows

# Install dependencies
pip install -r requirements.txt
```

### BLS API Key (Optional)

For higher rate limits, register for a free API key at https://data.bls.gov/registrationEngine/

Set the key as an environment variable:
```bash
export BLS_API_KEY=your_key_here
```

Or create a `.env` file:
```
BLS_API_KEY=your_key_here
```

## Usage

```bash
jupyter notebook manufacturing_tariffs_analysis.ipynb
```

Run all cells to:
1. Fetch data from BLS API
2. Process and analyze employment trends
3. Generate visualizations
4. Export final figure to `figures/`

## Output

Final visualization: `figures/manufacturing_employment.png` (1080x1350px, 4:5 ratio)

## License

MIT
