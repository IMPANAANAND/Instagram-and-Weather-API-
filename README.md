# Climate and Instagram API

This Jupyter Notebook demonstrates how to fetch and analyze data from three different sources:
- **Weather Data** using the OpenWeather API
- **Agricultural Market Data** from the eNAM (National Agriculture Market) portal
- **Instagram Profile and Post Data** using the Instaloader library

## Features

- Fetches current weather information for any city using OpenWeather API.
- Retrieves mandi (market) trade data from the eNAM portal via HTTP requests.
- Scrapes Instagram profile details and post statistics (likes, comments, captions) using Instaloader.

## Requirements

- Python 3.7+
- Jupyter Notebook
- [requests](https://pypi.org/project/requests/)
- [instaloader](https://pypi.org/project/instaloader/)
- [httpx](https://pypi.org/project/httpx/) (optional, for advanced HTTP requests)

Install dependencies with:

```sh
pip install requests instaloader httpx
```

## Usage

1. **Weather Data**
   - Enter a city name when prompted to get current temperature, humidity, wind speed, and more.
   - Requires a free API key from [OpenWeather](https://openweathermap.org/).

2. **Mandi Data**
   - Fetches trade data from the eNAM portal for a given date and filters (state, commodity, etc.).
   - Example POST request is included for custom queries.

3. **Instagram Data**
   - Scrapes public profile information and post details.
   - You can download posts or just print statistics (likes, comments, captions).
   - Replace the username in the code with any public Instagram profile.

## Example

```python
# Get weather for a city
city = input("Enter city name: ")
get_weather(city)

# Fetch mandi data for a specific date
# (See code cell for form_data customization)

# Scrape Instagram profile and posts
profile_username = 'example_username'
# See notebook for details
```

## Notes

- For Instagram scraping, only public profiles are supported unless you log in with Instaloader.
- Respect the terms of service of all APIs and websites.
- API keys should be kept private and not shared publicly.

## License

For educational and research purposes only.
