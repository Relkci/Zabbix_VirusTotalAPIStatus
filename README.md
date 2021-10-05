# Zabbix_VirusTotalAPIStatus
Zabbix Template for VirusTotal API account usage. Provides account info and API usage.

## Installation
Import Zabbix_VirusTotal-APIStatus.yaml (Zabbix Template)
Create Zabbix host
Link new Zabbix Template "VirusTotal API Provider"
Set macro "{$VIRUSTOTALAPIKEY}" to your VirusTotal API Key
Add agent interface (its necessary for the HTTP Agent to work, despite an actual "host" not being necessary.)

## Items
- VirusTotal User type
- VirusTotal API User Status
- VirusTotal User Reputation
- VirusTotal UserID
- VirusTotal User MFA Enabled
- USED / ALLOWED for all quotas:
  - Monitor Uploaded Files (Count)
  - Monitor Uploaded Files (Bytes)
  - Monitor Storage Files (Count)
  - Monitor Storage Files (Bytes)
  - Intelligence VTDiff Creation
  - Intelligence Searches
  - Intelligence Retro-Hunt Jobs
  - Intelligence Hunting Rules
  - Intelligence Graphs Private
  - Intelligence Downloads 
  - Cases Created
  - API Requests (Monthly)
  - API Requests (Daily)
  - API Requests (Hourly)

## Graphs
- API Requests - use/allowed
- Intelligence frameworks - used/allowed
- Monitored files uploaded/stored - used/allowed

## Triggers
- 75% Use and 100% use for all above listed quotas
- Plan change
- Account not active
- Account without MFA


## Triggers
Credits has reached zero
Change in account status
Account status is inactive

## Contact
Twitter: @KRelkci
GitHub: @Relkci

## Special Thanks
Black Hills Information Security
https://www.blackhillsinfosec.com