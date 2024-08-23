# Weather App

A simple weather application built with Django that allows users to check current weather conditions for any city.

## Features

- View current weather conditions including temperature, humidity, and weather description.
- Search for weather by city name.
- Responsive design for desktop and mobile devices.

## Technologies

- Django
- Python
- OpenWeatherMap API (or any other weather API of your choice)
- HTML/CSS for frontend

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/weather-app.git
   cd weather-app
   ```

2. **Create and activate a virtual environment:**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```

3. **Install the required packages:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up your environment variables:**

   Create a `.env` file in the root directory and add your OpenWeatherMap API key:

   ```
   WEATHER_API_KEY=your_api_key_here
   ```

5. **Run migrations to set up the database:**

   ```bash
   python manage.py migrate
   ```

6. **Create a superuser (optional for admin access):**

   ```bash
   python manage.py createsuperuser
   ```

7. **Start the development server:**

   ```bash
   python manage.py runserver
   ```

   You can now access the app at `http://127.0.0.1:8000/`.

## Usage

1. Open the app in your web browser.
2. Enter the city name in the search bar and submit.
3. View the current weather details displayed on the page.


## API Integration

- This app uses the [OpenWeatherMap API](https://openweathermap.org/api) to fetch weather data.
- Update `weather/views.py` with your API key and endpoint details.

## Dependencies

List of dependencies is included in `requirements.txt`:

```
Django>=3.0,<4.0
requests
python-dotenv
```
