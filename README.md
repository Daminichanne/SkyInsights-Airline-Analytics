# SkyInsights — Airline Passenger Analytics Dashboard

An interactive, responsive portfolio project that analyses passenger satisfaction and airline service performance using the supplied airline passenger dataset.

## Live dashboard
After publishing with GitHub Pages, add your GitHub Pages URL here.

## Project highlights
- 129,880 passenger records and 22 source columns
- Data cleaning: whitespace normalization and median imputation for missing arrival-delay values
- Interactive filters: travel type, cabin class, customer type and gender
- KPIs: passenger count, satisfaction rate, average flight distance and average arrival delay
- Visual analysis: satisfaction split, satisfaction by cabin/travel type, service ratings, delays and age profile
- Responsive dark aviation theme with the supplied airplane photograph used as a subdued hero background
- Built with HTML, CSS and vanilla JavaScript; no build step or paid service required

## Repository structure
```text
skyinsights-airline-analytics/
├── index.html
├── cleaned_airline_passenger_data.csv
├── assets/
│   └── airplane-hero.jpg
└── README.md
```

## Run locally
The dashboard fetches its CSV file, so serve the folder through a local web server rather than opening `index.html` directly.

### Python
```bash
python -m http.server 8000
```
Open `http://localhost:8000`.

### VS Code
Install the **Live Server** extension, right-click `index.html`, and select **Open with Live Server**.

## Publish on GitHub Pages
1. Create a public GitHub repository, for example `skyinsights-airline-analytics`.
2. Upload all files and folders from this project. Keep `index.html`, the CSV, and `assets/` at the repository root as shown.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. Wait for deployment and open the generated Pages URL.

## Data preparation notes
- Original data contained 129,880 rows and 22 columns.
- No exact duplicate rows were found.
- `Arrival Delay in Minutes` contained 393 missing values; these were filled with the median (0 minutes).
- The boolean satisfaction field was converted to readable labels: `Satisfied` and `Dissatisfied`.
- Text fields were trimmed to remove leading/trailing whitespace.
- The original uploaded dataset is not included in this repository; only the cleaned output is included.

## Initial findings (full dataset)
- 43.45% of passengers are satisfied; 56.55% are dissatisfied.
- Average arrival delay after cleaning is approximately 15.0 minutes.
- Inflight Wi-Fi has the lowest average service rating (about 2.73/5).
- Business travel satisfaction is about 58.4%, compared with about 10.1% for personal travel.
- Business class satisfaction is about 69.4%, compared with about 18.8% in economy.

These are descriptive findings, not proof that any one factor causes satisfaction. Use the filters to investigate segments and validate recommendations.

## Suggested interview walkthrough
1. Explain the business question: which passenger segments and service touchpoints are associated with satisfaction?
2. Describe the cleaning decisions and why missing arrival delays were imputed with the median.
3. Demonstrate the four filters and explain how KPIs and charts update.
4. Share two findings and one practical recommendation.
5. Explain limitations: the dataset is observational, and the supplied data does not include airline, route, date or flight identifiers.

## LinkedIn project description
Built **SkyInsights — Airline Passenger Analytics Dashboard**, an end-to-end data analytics portfolio project using 129K+ passenger records. Cleaned missing values, explored satisfaction patterns, analysed service ratings and flight delays, and developed an interactive responsive dashboard with segment filters and business insights. Built using Python (Pandas) for data preparation and HTML, CSS and JavaScript for dashboard development.

**Skills demonstrated:** Data Cleaning · Exploratory Data Analysis · KPI Design · Data Visualization · Customer Segmentation · Business Insights · GitHub Pages
