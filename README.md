# Windows Virtual Desktop

This workbook visualises the health and performance of WVD (Spring Release). To be able to use this workbook, you will need to enable the following:

1. [VMInsights](https://docs.microsoft.com/en-us/azure/azure-monitor/insights/vminsights-enable-overview) on the hosts
2. [WVD Diagnostic Logs](https://docs.microsoft.com/en-us/azure/virtual-desktop/diagnostics-log-analytics#push-diagnostics-data-to-your-workspace)
3. Collection of the following [performance counters](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/data-sources-performance-counters) in your Log Analytics workspace:

* `Terminal Services Session(*)\% Processor Time`
* `Terminal Services(*)\Active Sessions`
* `Terminal Services(*)\Inactive Sessions`
* `Terminal Services(*)\Total Sessions`
* `LogicalDisk(*)\% Free Space`
* `Processor(_Total)\% Processor Time`
* `Memory(*)\% Committed Bytes In Use`
* `Network Adapter(*)\Bytes Received/sec`
* `Network Adapter(*)\Bytes Sent/sec`
* `Process(*)\% Processor Time`
* `Process(*)\% User Time`
* `Process(*)\IO Read Operations/sec`
* `Process(*)\IO Write Operations/sec`
* `Process(*)\Thread Count`
* `Process(*)\Working Set`
* `RemoteFX Graphics(*)\Average Encoding Time`
* `RemoteFX Graphics(*)\Frames Skipped/Second - Insufficient Client Resources`
* `RemoteFX Graphics(*)\Frames Skipped/Second - Insufficient Network Resources` 
* `RemoteFX Graphics(*)\Frames Skipped/Second - Insufficient Server Resources`
* `RemoteFX Network(*)\Current TCP Bandwidth`
* `RemoteFX Network(*)\Current TCP RTT`
* `RemoteFX Network(*)\Current UDP Bandwidth` 
* `RemoteFX Network(*)\Current UDP RTT`



To use this workbook, create a new workbook in Azure Monitor, and copy the code from this sample into the code area for the workbook, replacing the sample code in this workbook
