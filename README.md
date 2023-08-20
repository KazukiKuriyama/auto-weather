# auto-weather

This repository provides a GitHub Action that automatically updates the weather information for Osaka on a daily basis. The action fetches weather data from the OpenWeatherMap API every day at 9 AM Japan time and appends this data to a file named `weather_data.md`.

## Workflow Details

- The `Update Weather` workflow can be triggered manually (`workflow_dispatch`) or by schedule (`cron`).
- The data is stored in the `weather_data.md` file inside the `auto-weather` directory.
- This workflow is executed only on the `main` branch.

## How to Use

1. Clone or fork this repository.
2. Set up the following information in GitHub Secrets:
   - `GH_TOKEN`: Token for accessing GitHub.
   - `WEATHER_API_KEY`: Your API key for OpenWeatherMap.
   - `USER_EMAIL`: Email address for making commits.
   - `USER_NAME`: Username for making commits.
3. If needed, modify the weather API endpoint or parameters within the workflow file accordingly.
