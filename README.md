# X-Crypto

A React-based cryptocurrency tracking application that displays live market data using the CoinGecko API.

## Project Overview

X-Crypto is a crypto tracker built with React and Material UI. It provides a dashboard for browsing popular cryptocurrencies, checking live prices, reviewing market changes, and opening individual coin detail pages with historical price charts.

This project was originally based on the public react-crypto-tracker project and has been customized and adapted for X-Crypto.

## Features

- Cryptocurrency market listings
- Current prices in INR and USD
- 24-hour price change tracking
- Market capitalization information
- Search functionality for coins
- Pagination for large lists
- Currency selection
- Individual coin detail pages
- Historical price chart data
- Responsive UI for desktop and smaller screens

## Tech Stack

- React 17
- React DOM 17
- React Scripts 4
- Material UI 4
- React Router DOM 5
- Axios
- Chart.js
- react-chartjs-2
- GitHub Pages

## API

This project uses the CoinGecko public market API with a demo API key passed through the environment variable `REACT_APP_COINGECKO_API_KEY`.

Because the app is a static frontend hosted on GitHub Pages, the browser-side API key cannot be treated as a fully secret production credential. It should be kept out of Git history and not committed to the public repository.

## Project Structure

```text
src/
  App.js
  index.js
  CryptoContext.js
  Pages/
    HomePage.js
    CoinPage.js
  components/
    Header.js
    CoinsTable.js
    CoinInfo.js
    SelectButton.js
    Banner/
      Banner.js
      Carousel.js
  config/
    api.js
    data.js
  App.css
  index.css
```

## How to Run Locally

1. Install dependencies:
   ```bash
   npm install --legacy-peer-deps
   ```
2. Create a `.env` file in the root of the project:
   ```env
   REACT_APP_COINGECKO_API_KEY=YOUR_API_KEY
   ```
3. Start the app:
   ```bash
   npm start
   ```
4. Open the local app in the browser:
   ```text
   http://localhost:3000
   ```

## Environment Variables

Create a `.env` file in the root directory with:

```env
REACT_APP_COINGECKO_API_KEY=YOUR_API_KEY
```

Do not commit the `.env` file to GitHub.

## Deployment

This project is configured for GitHub Pages deployment using the `gh-pages` package.

Deploy steps:

```bash
yarn build
yarn deploy
```

GitHub Pages should be configured to deploy from the `gh-pages` branch, with the root folder selected.

## Live Demo

- Website: https://dalip01.github.io/X-Crypto/
- GitHub Repository: https://github.com/Dalip01/X-Crypto

## Future Improvements

- Add portfolio tracking
- Add dark/light theme toggle
- Improve chart filtering options
- Add more advanced coin analytics
- Add caching for API data

## License

This project is for portfolio and demonstration use.
