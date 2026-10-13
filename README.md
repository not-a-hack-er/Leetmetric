# Leetmetric

A small vanilla HTML/CSS/JavaScript page that looks up a LeetCode username and displays solved counts by difficulty as progress rings and summary cards.

## Run locally

Open `index.html` in a browser, enter a username, and select **Search**. No build step or package installation is required.

The page fetches statistics from the third-party `leetcode-stats-api.herokuapp.com` service. It is not an official LeetCode client. The lookup requires an internet connection and may fail if that service is unavailable, changes its response format, or blocks browser requests. The UI reports fetch errors, but no offline statistics are available.

## Project files

| File | Role |
| --- | --- |
| `index.html` | Search form and result containers |
| `style.css` | Responsive layout and progress-ring styling |
| `script.js` | Input validation, API request, and rendering |

## Current limitations

- The total-question fallback values in `script.js` are fixed and may become outdated.
- The repository has no automated test suite yet.
- Solved counts depend on what the third-party API reports; do not use this page as an authoritative activity export.
