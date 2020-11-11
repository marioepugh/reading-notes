Mario Pugh		November 10, 2020

Getting data into Splunk from Windows endpoints
The Get Windows Data section of the Getting Data exposes the nuance of data collection on Windows and the necessary installation prerequisites. The key items are Universal Forwarder which is the most efficient way to gather data from any Windows server that you want to gather data. Universal forwarders use limited resources such as Registry monitoring, because you cannot collect Registry data over WMI. 

Splunk forwarders use a universal forwarder to get data in from a remote Windows host. A universal forwarder offers the most types of data sources, provides more detailed data (for example, in performance monitoring metrics), minimizes network overhead, and reduces operational risk and complexity. It is also more scalable than WMI in many cases. The user that Splunk Enterprise runs as determines what Splunk Enterprise can monitor. 
