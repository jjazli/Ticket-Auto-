# RRHTBX Ticket Automation Bot

## Description
This bot automates the process of purchasing tickets on KKTix. It searches for a specified event, logs in with provided credentials, and attempts to purchase tickets when they become available based on specified criteria (e.g., ticket type and price).

## Features
- **Search for Event**: Locates the desired event on KKTix based on the event name and category.
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

# Configuration
# -----------------
# To configure the bot, update the following variables in your script:

BASE_URL = "https://kktix.com/"
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

# 1. Clone the repository from GitHub:
# ```bash
# git clone <repository_url>
# ```

# 2. Navigate to the script directory:
# ```bash
# cd path/to/repository
# ```

# 3. Run the script:
# ```bash
# python ticket_bot.py
# ```

# Customization
Adjust these variables to customize your bot:

- EVENT_NAME: Change this to match the name of the event you want to purchase tickets for.
- CATEGORY_NAME: Adjust this if the event is under a different category on KKTix.
- DESIRED_TICKET_PRICES: Set the ticket prices you are willing to pay.
- TICKET_TYPE: Specify the ticket type to target.
- PREFERRED_PRICE: Set the preferred ticket price to target.
- QUANTITY: Number of tickets you wish to purchase.
- REFRESH_INTERVAL: Time interval in seconds for refreshing the page (default is 1 second).
- MAX_WAIT_TIME: Maximum wait time in seconds before stopping attempts (default is 900 seconds).

# Notes
This bot is intended for personal use. Be mindful of RRHTBX's terms of service and avoid misuse.
The script will log relevant actions and any issues encountered in `bot_log.log`.
Adjust the logging level in the `logging.basicConfig` call if you want more or less detailed logging output.

# Troubleshooting

"Event not found or incorrect name specified": Ensure your event name and category are correct and spelled as expected by KKTix.
"Tickets are sold out": The bot may be too late; adjust the refresh interval and retry.
"Error navigating to event page": Check your connection and ensure the RRHTBX page structure hasn't changed.



