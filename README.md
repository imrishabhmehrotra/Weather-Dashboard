# Weather Dashboard

## Description

Weather Dashboard is a React-based web application that provides real-time weather information for a given city. The application displays the current weather and a 5-day forecast. It uses the OpenWeatherMap API to fetch weather data and a JSON server to store and manage favorite cities. The application is designed to be visually appealing with a focus on a good user experience.

## Features

- **Search for a City:** Enter the name of a city to get the current weather and 5-day forecast.
- **Favorite Cities:** Add, view, and manage favorite cities.
- **Real-time Weather Data:** Displays up-to-date weather information using the OpenWeatherMap API.
- **Toggle Temperature Units:** Switch between Celsius and Fahrenheit.
- **Responsive Design:** The application is designed to be responsive and works on both desktop and mobile devices.
- **Local Storage:** Remembers the user's last searched city.

## Installation

Follow these steps to set up and run the Weather Dashboard application on your local machine.

### Prerequisites

- Node.js and npm installed on your machine.
- An OpenWeatherMap API key. You can sign up for a free API key [here](https://openweathermap.org/api).

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/imrishabhmehrotra/Weather-Dashboard.git
   cd weather-dashboard
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file in the root directory and add your OpenWeatherMap API key:**
   ```plaintext
   VITE_API_KEY=your_openweathermap_api_key
   ```

4. **Start the JSON server:**
   ```bash
   npx json-server --watch db.json --port 8000
   ```

5. **Run the application:**
   ```bash
   npm run dev
   ```

6. **Open your browser and navigate to:**
   ```plaintext
   http://localhost:3000
   ```

## Project Structure

```plaintext
weather-dashboard/
├── public/
│   ├── index.html
├── src/
│   ├── components/
│   │   ├── Search.js
│   │   ├── FavoriteCities.js
│   │   ├── WeatherDisplay.js
|   |   |   Dashboard.js
│   ├── styles/
│   │   ├── main.scss
│   ├── App.js
│   ├── index.js
├── .env
├── db.json
├── package.json
└── README.md
```

## Usage

- **Search for Weather:** Enter a city name in the search bar and press enter to see the current weather and 5-day forecast.
- **Add to Favorites:** Click on the "Add to Favorites" button to save the city to your favorites list.
- **View Favorites:** Click on a city in the favorites list to view its weather information.
- **Remove from Favorites:** Click the "Remove" button next to a city in the favorites list to remove it.

## Technologies Used

- **React**: Front-end library for building user interfaces.
- **OpenWeatherMap API**: Provides weather data.
- **JSON Server**: A simple full fake REST API for managing favorite cities.
- **SCSS**: CSS preprocessor for styling.
