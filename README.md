# Wonderland Weather

<img src="assets/thumb.png" width="200">

**Wonderland Weather** is a [Grinning Cat AI](https://github.com/matteocacciola/grinning-cat-core) plugin that provides
real-time and multi-day weather forecasts powered by the [OpenWeatherMap](https://openweathermap.org/) API.

> **Author:** [Matteo Cacciola](https://github.com/matteocacciola)  
> **Version:** 1.0.0  
> **Repository:** [github.com/matteocacciola/cat-wonderland-weather](https://github.com/matteocacciola/cat-wonderland-weather)

---

## Features

- Fetches a **5-day weather forecast** from the OpenWeatherMap API.
- Responds to natural language questions such as:
  - *"What's the weather today?"*
  - *"What will the weather be like tomorrow?"*
  - *"What will the weather be like in New York on Tuesday?"*
- Supports both **metric (°C)** and **imperial (°F)** temperature units.
- The **city is specified directly in the conversation** — no need to pre-configure it.

---

## Requirements

- A valid [OpenWeatherMap API key](https://openweathermap.org/api).

---

## Configuration

Once the plugin is installed, configure it from the Grinning Cat admin panel:

| Parameter          | Type                   | Required | Default    | Description                                                     |
|--------------------|------------------------|----------|------------|-----------------------------------------------------------------|
| `open_weather_api` | `string`               | ✅ Yes    | —          | Your OpenWeatherMap API key                                     |
| `temperature_unit` | `metric` \| `imperial` | ❌ No     | `imperial` | Temperature unit: Celsius (`metric`) or Fahrenheit (`imperial`) |

> ⚠️ **Note:** The city is **not** a fixed setting. It is inferred from each conversation message. If no city is mentioned in the question, the tool will not be invoked.

---

## Usage

After configuration, simply ask the Cat about the weather **including a city name**:

"What is the weather like in London today?" "Will it rain in Paris this weekend?" "Weather forecast for Tokyo on Friday"

The plugin will return a daily breakdown including:
- **Date**
- **Temperature** (in the configured unit)
- **Weather conditions** (e.g. *light rain*, *clear sky*)

---

## Installation

1. Open the Grinning Cat AI admin panel.
2. Navigate to **Plugins**.
3. Search for **"Wonderland Weather"** and click **Install**.
4. Set your OpenWeatherMap API key by using the endpoint URL provided by the Grinning Cat.