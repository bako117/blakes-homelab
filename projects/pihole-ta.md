# Splunk Technology Add-on (TA) for Pi-hole  
## Summary
**First Started:** August 2025  

**End-Date:** Completed (v1) — extendable with future features  

**Overview:**  
This project involved developing a custom Splunk Technology Add-on (TA) to properly parse and normalize Pi-hole DNS logs ingested into Splunk. Out-of-the-box, Splunk does not natively understand Pi-hole log formats. By creating a TA with custom props and transforms, I enabled Splunk to extract fields such as domains, query types, response codes, and client IPs.  

**Goal/Idea:** Build a Splunk TA that allows clean, searchable DNS data from Pi-hole logs.  
- Write custom regex patterns to extract relevant fields  
- Normalize logs into a consistent schema for analysis  
- Enable dashboards and detections for DNS traffic  
- Lay groundwork for integration with Splunk Enterprise Security  

## Skills Learned
- Splunk app/TA development  
- props.conf and transforms.conf configuration  
- Regex design for log parsing  
- Field extraction and normalization  
- Testing with `btool` and Splunk SPL searches  

## Outcome
A working Splunk TA that:  
- Normalizes Pi-hole logs under the sourcetype `pihole:dns`  
- Extracts key fields (domain, rtype, answer, qtype, client_ip, sinkhole flag)  
- Distinguishes between event types (Blocked, Cached, Forwarded, Query, Reply)  
- Provides structured data for dashboards, alerts, and correlation searches  

This transforms raw DNS logs into actionable data for a SOC-style workflow.  

## Progress Notes
- v1.0: Created base app structure (`app.conf`, `default.meta`, `props.conf`, `transforms.conf`)  
- v1.1: Added regex extractions for blocked, cached, forwarded, and query events  
- v1.2: Normalized fields using `EVAL-` statements (rtype, sinkhole)  
- v1.3: Validated with `btool` and SPL searches to confirm accuracy  
