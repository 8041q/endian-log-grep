# endian-log-filter
Endian VPN powershell script that will filter the logs for when each user logged in  

> Coding language: English | EN  
> User displayed language: Portuguese | PT  

Unfortanetly, Endian VPN doesn't let you grab the a log of a whole year, you would need to grab each month. But you can gather all of them and then merge all those logs together, the script will have the expected end output faster, easier and less confusing.
```
How to concatenate multiple log files into a single one
	- Do the following command in a DOS-box (cmd.exe) located on the folden containing the logs

		type *.log > logs-merged.log
```

When starting the script, it will first open the file explorer for you to select the log file, then 3 options will show up to filter the log by (N/D/M): 
- N - Name
- D - Day and Month
- M - Month

To select each, just write the first letter (N/D/M) and press enter. The script will then show you the results, and it will let you choose to save the output in a CSV file in a given location.

## How it works
The script will simply filter out using keyworks, sush as "Peer Connection Initiated" and then using regex to grab certain words by the pattern.
