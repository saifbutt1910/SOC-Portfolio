Week 2 Day 13 - Splunk Basics

What is Splunk?

Splunk is a SIEM platform used to collect, store, search and analyze logs from different systems.

Why Splunk is Important

- Searches millions of logs quickly
- Helps investigate incidents
- Generates alerts
- Correlates events

Basic SPL Examples

Search Windows logs:

index=windows

Search failed logins:

index=windows EventCode=4625

Search PowerShell activity:

index=sysmon powershell.exe

What I Learned Today

- Splunk is widely used in SOC environments.
- SPL is used to search logs.
- An index is a collection of related logs.
- Splunk helps analysts investigate security incidents efficiently.

SOC Investigation Exercise

Timeline

- Multiple failed login attempts
- Successful login
- PowerShell execution
- Unauthorized administrator account creation
- Outbound connection to an unknown IP address

Assessment

The correlation of these events suggests a likely successful compromise requiring immediate investigation.

Investigation Steps

- Review Windows Event Logs
- Analyze Sysmon process creation events
- Review PowerShell command-line activity
- Investigate network connections
- Check for file creation and modification
- Verify whether sensitive data was accessed

Response

- Isolate the affected system
- Preserve evidence
- Disable unauthorized account
- Block malicious IP
- Reset credentials
- Escalate and document
