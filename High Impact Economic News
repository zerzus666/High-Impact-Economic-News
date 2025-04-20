# Create a Render-compatible Python script that pulls high-impact news and serves JSON
news_script = """
from flask import Flask, jsonify
import requests
from datetime import datetime, timedelta

app = Flask(__name__)

@app.route('/')
def home():
    return "News Feed Online"

@app.route('/high-impact-news')
def high_impact_news():
    # Example: Static list simulating TradingEconomics or ForexFactory impact feed
    events = [
        {"symbol": "USD", "time": "2025-04-24T13:30:00Z", "impact": "high", "event": "US GDP QoQ"},
        {"symbol": "EUR", "time": "2025-04-25T09:00:00Z", "impact": "high", "event": "ECB Rate Decision"},
        {"symbol": "GBP", "time": "2025-04-25T10:00:00Z", "impact": "high", "event": "UK CPI y/y"},
    ]
    return jsonify(events)

if __name__ == '__main__':
    app.run(debug=True, port=5000)
"""

# Save the script to file for user to deploy on Render or Replit
script_path = "/mnt/data/render_high_impact_news_feed.py"
with open(script_path, "w") as file:
    file.write(news_script)

script_path
