# Koh Rong Island Telegram Mini Apps

This repository contains the Mini Apps for the Koh Rong Island Management System Telegram bot.

## Components

- `input.html`: Mini App for capturing user input with an intuitive and context-aware interface
- `results.html`: Mini App for displaying AI-generated recommendations with filtering capabilities

## How It Works

1. The Telegram bot sends users to these Mini Apps with specific context parameters
2. Users can interact with the rich UI to provide input or view results
3. The Mini Apps communicate with the bot through Telegram's WebApp API
4. Data processing is handled by Google Cloud Functions

## Development

To run these Mini Apps locally for development:

1. Clone this repository
2. Use a local server (e.g., `python -m http.server`)
3. Update the `CLOUD_FUNCTION_URL` in `results.html` to point to your Google Cloud Function

## Deployment

This repository is set up for GitHub Pages deployment:

1. The Mini Apps will be available at `https://<username>.github.io/koh-rong-telegram-app/`
2. Remember to update the `WEBAPP_HOST` in your bot configuration with this URL

## Customization

To customize the UI:

1. Modify the CSS styles in the HTML files
2. Update the hint chips and categories in the JavaScript
3. Adjust result formatting to match your data structure

## Important Notes

- The Telegram bot must have Web App functionality enabled
- The Mini Apps require HTTPS (provided by GitHub Pages)
- The Google Cloud Functions must have CORS enabled for the GitHub Pages domain
