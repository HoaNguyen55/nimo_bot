# NimoTV Bot

## Overview

This Python script is designed to automate interactions with the NimoTV website using Selenium and BeautifulSoup. The bot opens multiple tabs, logs in (if specified), and collects information from live streams on the [NimoTV Lives](https://www.nimo.tv/lives) page.

## Prerequisites

Before running the script, ensure you have the necessary dependencies installed. You can install them using the following command:

```bash
pip install beautifulsoup4 selenium
```

## Usage

### Command-Line Arguments

- `--waitlongtime`: Wait time for long intervals (default: 10 seconds).
- `--waitshorttime`: Wait time for short intervals (default: 5 seconds).
- `--opentabnum`: Number of tabs to open (default: 10).
- `--username`: NimoTV account username (required).
- `--password`: NimoTV account password (required).
- `--headless`: Run Chrome in headless mode (default: true).
- `--nonlogin`: Choose not to log in to the NimoTV account (default: false).
- `--url`: Website URL to scrape (default: [https://www.nimo.tv/lives](https://www.nimo.tv/lives)).
- `--urlonlyset`: Use a specific URL (default: false).
- `--specificurl`: Specific URL to use (default: empty string).
- `--egg`: Collect eggs during the process (default: false).

### Running the Script

Example:

```bash
python nimo_bot.py --username your_username --password your_password --opentabnum 5
```

### Notes

1. The script uses Chrome as the browser. Ensure you have the [ChromeDriver](https://sites.google.com/chromium.org/driver/) installed and added to your system PATH.

2. The script is designed for the specific structure of the NimoTV website. If the website structure changes, adjustments may be needed.

3. If collecting eggs (`--egg` set to true), the script will check for and click on egg images on each opened tab.

## Disclaimer

This script is provided as-is and may not comply with the terms of service of the NimoTV website. Use it responsibly and at your own risk. The authors are not responsible for any misuse or consequences arising from the use of this script.

## Example
- If use default, please remember put your account into `--username` and `--password` because they are the required \
`python3 nimobot.py --username=abcdef --pasword=12345 `

- If you'd like to change any parameters such as `opentabnum` (number of tab) on browser at a time \
`python3 nimobot.py --username=abcdef --pasword=12345 --opentabnum=10 `
