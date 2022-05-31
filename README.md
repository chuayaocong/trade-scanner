# trade-scanner
This program scans for options trades (real-time) based on a certain criteria
This program can be executed daily (after market open hours) as an easy way to determine if trades should be placed. It checks if the VIX value from the day before is below the 21-day exponential moving average of VIX, and also if VIX is increasing. If both conditions are met, the prompt prints a message indicating to the user to open trade.
- OpentradeTT - a more stringent rule which requires that both conditions are True on the same day.
- OpentradeFTT - a less stringent rule which requires that VIX is increasing, but if VIX is less than VIX-21D EMA the day before, open trade == True.
The program also checks the number of consecutive wks SPY has closed lower, for an overall indicator of the health of the stock market.
