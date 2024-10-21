# Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates

OVERVIEW:

The system is designed to monitor weather conditions in real-time across major Indian metros using data from the OpenWeatherMap API. It continuously fetches weather updates for cities like Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad. The system processes the data to produce daily weather summaries, trigger alerts when certain thresholds are breached, and visualize historical weather trends.

IMPLEMENTATION  DETAILS:
1. API Interaction:
The system uses Python (or another language like Java or Node.js) to interact with the OpenWeatherMap API. Weather data is fetched at configurable intervals using a scheduled task.
2. Data Aggregation Logic:
For each city, weather data is stored in memory during the day.
At the end of each day, the system calculates aggregates (average, max, min temperature, and dominant weather condition).
3. Database for Storage:
The daily summaries and alert history are stored in a relational database like MySQL or SQLite. This allows for efficient retrieval of historical data.
4. Alerting System:
A comparison is made between the current weather data and user-defined thresholds.
If the temperature exceeds the configured threshold for two consecutive updates, or specific weather conditions (e.g., rain) occur, an alert is triggered.
5. Visualizations:
Visualization libraries such as matplotlib, seaborn (in Python), or front-end tools like Chart.js or D3.js can be used to display weather summaries and trends on a dashboard.

PREREQUISITE:

1.Installation of Python 3.8

2.pip Installment

DEPENDENCY:

1. pip install -r requirement.txt

2. import pandas

3. import time

4. import sqlite3 and datatime

5. import ploty.graph_object and defaultdict

CONCLUSION:

This real-time weather monitoring system provides a comprehensive solution for tracking and analyzing weather data for specific cities. By utilizing rollups and aggregates, the system can generate insightful daily summaries, trigger alerts for predefined weather conditions, and offer visualizations of historical data, making it ideal for users looking to monitor weather trends in real-time.



