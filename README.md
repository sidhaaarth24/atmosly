# Atmosly

Atmosly is a clean, responsive weather dashboard that brings current weather conditions, forecasts, and atmospheric information together in one place. Search for a city to explore its local weather, track conditions throughout the day, and plan ahead with a detailed 7-day forecast.

[View the live site](https://sidhaaarth24.github.io/atmosly/)

## Features

- Live weather conditions with temperature and feels-like temperature.
- City search powered by location geocoding.
- Celsius and Fahrenheit temperature toggle.
- Hourly forecast for the next 24 hours.
- 7-day weather forecast with daily high and low temperatures.
- Atmospheric details including wind, humidity, pressure, UV index, and rainfall.
- Air quality information, including US AQI and PM2.5.
- Sunrise, sunset, daylight duration, and moon phase information.
- Interactive location map powered by Leaflet and OpenStreetMap.
- Light and dark themes with the selected theme saved in the browser.
- Responsive interface for desktop and mobile screens.

## Project Structure

```text
Atmosly/
├── index.html      # Main dashboard structure
├── styles.css      # Layout, styling, themes, and responsive design
├── script.js       # Weather data, search, rendering, and interactions
├── README.md       # Project overview and usage guide
└── LICENSE         # MIT license
```

## Getting Started

### Option 1: Open directly in a browser

1. Download or clone the project.
2. Open the `index.html` file in your preferred browser.
3. Allow the page to connect to the required online services to load weather information.

### Option 2: Serve locally

For a more consistent local development experience, run a static web server from the project directory. For example, with Python:

```bash
cd Atmosly
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

No package installation, build process, or API key is required for the current implementation.

## Usage

- The dashboard initially loads weather information for Patna, India.
- Enter a city name in the search field and press Enter to view its weather.
- Use the temperature control to switch between Celsius and Fahrenheit.
- Use the theme control to switch between light and dark appearances.
- Review the hourly forecast to follow temperature and precipitation chances over the next 24 hours.
- Explore the weather metrics, daylight information, moon details, and interactive map.
- Check the 7-day forecast to compare expected conditions throughout the week.

## Data Sources and Dependencies

Atmosly retrieves weather information from the following online services:

- **Open-Meteo Geocoding API** — city search and geographic coordinates.
- **Open-Meteo Forecast API** — current conditions, hourly data, and daily forecasts.
- **Open-Meteo Air Quality API** — US AQI and PM2.5 information.
- **Leaflet** — interactive map functionality.
- **OpenStreetMap** — map tiles and map data.
- **Google Fonts** — DM Sans and Manrope typefaces.

These services require an internet connection. Their availability, data coverage, and terms of use are independent of this project.

## Privacy

Atmosly does not require an account or a project-specific backend. City searches and weather requests are made directly from the browser to the external services listed above. The selected appearance theme is stored locally in browser storage.

When using the application, the relevant city search or geographic coordinates are sent to the weather and geocoding services to retrieve the requested information. Refer to those providers' privacy policies and terms for details about their handling of requests.

## Acknowledgements

Atmosly was created as a straightforward weather dashboard focused on presenting useful weather information in a clear and accessible interface.

Weather data is provided by [Open-Meteo](https://open-meteo.com/). Map functionality is provided by [Leaflet](https://leafletjs.com/) and [OpenStreetMap](https://www.openstreetmap.org/).

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
