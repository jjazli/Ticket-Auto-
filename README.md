# Ticket Automation Bot

## Description
This bot automates the process of purchasing tickets. It searches for a specified event, logs in with provided credentials, and attempts to purchase tickets when they become available based on specified criteria (e.g., ticket type and price).

## Features
- **Search for Event**: Locates the desired event based on the event name and category.
- **Login**: Automatically logs into KKTix using your username and password.
- **Ticket Selection**: Automatically selects and purchases tickets when they are available at the preferred price.
- **Automatic Refresh**: Continuously refreshes the page to check for ticket availability.
- **Configurable**: Adjust the ticket type, preferred price, quantity, and refresh interval as needed.

## Prerequisites
- **Chrome Driver**: Ensure that the Chrome Driver executable (`chromedriver.exe`) is correctly configured and accessible in your system's PATH.
- **KKTix Account**: A KKTix account with the ability to purchase tickets is required.
- **Python 3.x**: This script is written in Python and requires Python 3.x to run.
- **Dependencies**:
  ```bash
  pip install selenium

## Configuration
# -----------------
# To configure the bot, update the following variables in your script:

```python
BASE_URL = "https://.com/"
EVENT_NAME = "sample_event"
CATEGORY_NAME = "Entertainment"
DESIRED_TICKET_PRICES = ["800", "3,200"]
TICKET_TYPE = "B1"
PREFERRED_PRICE = "800"
QUANTITY = "2"
REFRESH_INTERVAL = 1  # in seconds
MAX_WAIT_TIME = 900  # in seconds
USERNAME = "your_username_here"
PASSWORD = "your_password_here"
CHROME_DRIVER_PATH = "chromedriver.exe"

# Usage
# -----------------
# To use the bot:

1. Clone the repository from GitHub:
   ```bash
   git clone <repository_url>

2. Navigate to the script directory:
```bash
cd path/to/repository

3. Run the script:
```bash
python ticket_bot.py


This approach ensures that users understand it’s for educational purposes and provides a clear and concise guide on how to use the bot.


