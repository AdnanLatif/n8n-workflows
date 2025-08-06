# Global Earthquake Alert System

This project is an automated earthquake monitoring system built using [n8n](https://n8n.io/). It checks global seismic activity every 10 minutes, and if any recent earthquakes are detected with a magnitude above 1.5, it sends a detailed email alert directly to your inbox.

## Overview

Instead of constantly checking external apps or websites, this workflow automates the process for you. It connects to the US Geological Survey (USGS) public feed, filters for relevant data, formats it cleanly, and emails it using your Gmail account.

---

![Cover Image](./cover.png)

---

## What the Workflow Does

- Runs every 10 minutes using the built-in schedule trigger
- Calls the USGS API for earthquakes that occurred in the past hour
- Filters events where the magnitude is greater than 1.5
- Formats the output as an HTML-friendly report
- Sends the report via Gmail to your configured email address

## Setup Instructions

1. Open your n8n editor.
2. Import the provided JSON workflow file.
3. Set up a Gmail account credential in n8n if you haven't already.
4. In the Gmail node, replace the default email with your own address.
5. Activate the workflow.

That's it—your global earthquake alert system is now live.

## Requirements

- A working n8n setup (self-hosted or cloud)
- A Gmail account connected via OAuth2 credentials
- Internet access to connect to the USGS feed:  
  `https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_hour.geojson`

## Credits

This project uses the open and reliable earthquake data provided by the [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/).

---

## 🤖 Author

Built by [Adnan Latif](https://github.com/AdnanLatif)  
🧠 Follow my AI + automation series on [Medium](https://medium.com/@alatif.bwp)  
💼 Connect on [LinkedIn](https://www.linkedin.com/in/adlatif)
