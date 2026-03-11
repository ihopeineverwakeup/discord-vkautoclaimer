# Turbo Claimer

Fast and reliable VK ID claimer with Discord integration, ID swapper, and adjustable speed.

---

## Features

- High-speed VK ID claiming
- Built-in ID swapper
- Discord bot integration
- Captcha solving support
- Adjustable claiming speed
- Multi-token support
- Stable request handling

---

## Requirements

Before running the script make sure you have:

- Python 3.8 or newer
- Discord Bot
- VK API tokens

Your Discord bot must have all three Privileged Gateway Intents enabled:

- Presence Intent
- Server Members Intent
- Message Content Intent

---

## Installation

Install required dependencies:

pip install requests pyyaml discord vk_captchasolver xmltodict aiohttp bs4 lxml

If the script fails to start:

1. Open the project in Visual Studio Code or another editor
2. Check the error output
3. Install the missing libraries mentioned in the error

---

## Configuration

| Key | Description | How to get |
|-----|-------------|-----------|
| vk_token | VK Admin host token | Must not be listed in tokens.txt |
| check_token | VK community token | Community Settings → API → Create token |
| turbo_token | VK community token (separate group) | Same as above but from another community |
| vk_me_token | VK Me application token | See instructions below |

---

## Getting vk_me_token

Replace LOGIN and PASSWORD with your VK credentials:

https://oauth.vk.com/token?grant_type=password&client_id=6146827&client_secret=qVxWRF1CwHERuIrKBnqe&username=LOGIN&password=PASSWORD&v=5.131&2fa_supported=1

The API response will contain the vk_me_token.

---

## Discord Bot Setup

1. Open the Discord Developer Portal
2. Select your bot
3. Go to Bot → Privileged Gateway Intents
4. Enable the following:

- Presence Intent
- Server Members Intent
- Message Content Intent

---

## Usage

Run the script:

python claimer.py

After launching the script type:

h

to see the available commands.

---

## Adjusting Speed

Open claimer.py and change the delay value.

| Delay | Speed |
|------|------|
| 0.2 | Default (stable) |
| 0.02 | Fast (minimum recommended) |

Do not set the delay lower than 0.02 because it may cause instability.

---

## ID Swapper

The script includes a built-in ID swapper.

Speed is relatively stable. It is recommended to target short and clean IDs.

---

## Support

If you have questions or encounter issues, contact the me:

@repeater

Response time: up to 12 hours.
