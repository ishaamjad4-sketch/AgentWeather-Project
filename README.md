# Weather Agent

An end-to-end weather and air-quality forecasting project. The goal is to forecast six metrics for a city over the next 24 hours, generate hazard alerts, and display results in a dashboard.

> **Project status:** Work in progress. Some planned features, including live API ingestion, model training, LangGraph agents, and deployment, are not implemented yet.

## Planned forecasts

- Air Quality Index (AQI)
- Temperature (°C)
- Precipitation (mm) and rain probability
- Humidity (%)
- UV Index
- Wind speed and direction

## Planned technology

Python, pandas, scikit-learn, SARIMAX or Prophet, TensorFlow or PyTorch, Hopsworks, LangGraph, GitHub Actions, and Streamlit.

## Project structure

```text
src/weather_agent/   Application and pipeline code
data/                Sample data for local development
notebooks/           Exploratory data analysis
reports/             Project report and findings
tests/               Checks for project code
.github/workflows/   GitHub Actions workflows
```

## Getting started

1. Install Python 3.10 or newer.
2. Clone this repository:

   ```bash
   git clone https://github.com/[your-username]/project-weather-agent.git
   cd project-weather-agent
   ```

3. Create and activate a virtual environment:

   **Windows PowerShell**
   ```powershell
   py -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

   **macOS or Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

4. Install packages:

   ```bash
   pip install -r requirements.txt
   ```

5. Start the dashboard:

   ```bash
   streamlit run src/weather_agent/app.py
   ```

The starter dashboard uses sample data. It does not show live weather forecasts yet.

## Configuration

When API integration is added, copy `.env.example` to `.env` and add your API keys there. Never commit `.env` or publish API keys in this repository. Add production keys through your deployment platform's secrets settings.

## Planned project stages

- [ ] Fetch weather and air-quality observations
- [ ] Clean, align, and store data
- [ ] Explore metrics and build historical training data
- [ ] Compare forecasting models with a 24-hour naive baseline
- [ ] Build forecast, alert, weather-report, and drift agents
- [ ] Create and deploy the dashboard
- [ ] Document results, limitations, and issues

## Data sources

Planned sources: [OpenWeather](https://openweathermap.org/api) and [AQICN](https://aqicn.org/api/). API access and terms may apply.

## License

No license has been selected yet.
