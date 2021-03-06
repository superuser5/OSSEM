# DNP3 Log

## Description
None

## Data Dictionary
|Standard Name|Field Name|Type|Description|Sample Value|
|---|---|---|---|---|
|@timestamp|ts|date_time|Timestamp of the beginning of the event in epoch format|`1300475167.096535`|
|network_protocol|proto|string|The transport layer protocol of the connection.|`tcp`|
|src_ip_addr|id.orig_h|ip|The originating/source IP address|`10.1.1.1`|
|src_port|id.orig_p|integer|The originating/source port|`37682`|
|dst_ip_addr|id.resp_h|ip|The responding/destination IP address|`10.2.2.2`|
|dst_port|id.resp_p|integer|The responding/destination port|`20000`|
|event_uid|uid|string|Unique ID for the connection.|`CHhAvVGS1DHFjwGM9`|
|dnp3_function_reply|fc_reply|string|The name of the function message in the reply.|````|
|dnp3_function_request|fc_request|string|The name of the function message in the request.|`OPERATE`|
|dnp3_iin|iin|integer|The response's "internal indication number".|````|
