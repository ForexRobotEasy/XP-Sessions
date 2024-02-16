# XP Sessions

This is a custom indicator for MetaTrader 4 that displays the key global trading sessions on the chart. The indicator detects and highlights the London, New York, Sydney, and Tokyo sessions based on the user's input parameters.

## Input Parameters

- **showLondon**: Set to true to show the London session on the chart.
- **showNewYork**: Set to true to show the New York session on the chart.
- **showSydney**: Set to true to show the Sydney session on the chart.
- **showTokyo**: Set to true to show the Tokyo session on the chart.
- **maxDaysBack**: Maximum number of days back to get/draw the sessions.

## How it works

The indicator calculates the GMT time for each bar and checks if it falls within the specified number of days back. If it does, the indicator determines which session the bar belongs to and assigns a value to the xpBuffer. The xpBuffer values are used to highlight the sessions on the chart.

The indicator uses the following helper functions to check if a given time falls within a specific session:

- `IsLondonSession(datetime time)`: Checks if the given time is within the London session hours (8:00 to 16:00 GMT).
- `IsNewYorkSession(datetime time)`: Checks if the given time is within the New York session hours (12:00 to 20:00 GMT).
- `IsSydneySession(datetime time)`: Checks if the given time is within the Sydney session hours (22:00 to 06:00 GMT).
- `IsTokyoSession(datetime time)`: Checks if the given time is within the Tokyo session hours (00:00 to 08:00 GMT).

## Product Description

XP Sessions is a powerful custom indicator for MetaTrader 4 that helps traders identify and visualize the key global trading sessions on their charts. By highlighting the London, New York, Sydney, and Tokyo sessions, XP Sessions allows traders to better understand the market dynamics and make more informed trading decisions.

With XP Sessions, you can easily see when the major sessions start and end, enabling you to align your trading strategies with the most active and volatile market periods. Whether you are a scalper, day trader, or swing trader, knowing the session times can greatly improve your trading performance.

XP Sessions is easy to use and highly customizable. You can choose which sessions to display on your chart and adjust the maximum number of days back to get/draw the sessions. The indicator is designed to work seamlessly with any currency pair and time frame.

Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that can work as described in this product. To find the official developer and obtain the full version of XP Sessions, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/xp-sessions-review-master-forex-trading-with-key-global-sessions/).
