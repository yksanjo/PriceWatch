# PriceWatch 💵

> **Competitor Price Tracker** - Track competitor pricing changes and get alerts when prices change. Perfect for e-commerce and SaaS businesses.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Status: Active](https://img.shields.io/badge/status-active-success.svg)](https://github.com/yksanjo/PriceWatch)
[![GitHub stars](https://img.shields.io/github/stars/yksanjo/PriceWatch?style=social)](https://github.com/yksanjo/PriceWatch)

**PriceWatch** monitors your competitors' pricing and alerts you when prices change. Stay competitive with real-time price tracking, historical data, and trend analysis.

## Features

- 💰 Price change tracking
- 🔔 Email/Slack notifications
- 📊 Price history charts
- 🎯 Multiple competitor tracking
- ⏰ Scheduled price checks
- 📈 Price trend analysis

## Installation

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file:

```env
# Notification Settings
SLACK_WEBHOOK_URL=https://hooks.slack.com/services/YOUR/WEBHOOK/URL
EMAIL_TO=your-email@example.com

# Check Settings
CHECK_INTERVAL=3600  # Check every hour
```

## Usage

### Add Competitor Product

```bash
python tracker.py --add "Product Name" --url https://competitor.com/product --selector ".price"
```

### Check Prices Once

```bash
python tracker.py --check
```

### List Tracked Products

```bash
python tracker.py --list
```

### Start Continuous Monitoring

```bash
python tracker.py --watch
```

### View Price History

```bash
python tracker.py --history "Product Name"
```

## Supported Sites

- Any website with price information
- Custom CSS selectors for price extraction
- Supports JavaScript-rendered prices (with Selenium)

## License

MIT License


