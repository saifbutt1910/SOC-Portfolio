Week 2 Day 12 - SIEM Basics

What is a SIEM?

A SIEM (Security Information and Event Management) collects and analyzes logs from multiple devices to help detect security threats.

Why SIEM is Important

- Centralizes logs
- Correlates events
- Generates alerts
- Helps SOC analysts investigate incidents

Key Terms

- Log: Record of an event
- Event: An activity that occurred
- Alert: Notification of suspicious activity
- Incident: Confirmed security issue

Correlation

A SIEM uses correlation rules to combine multiple events and generate meaningful alerts.

What I Learned Today

- SIEM is the central monitoring platform in a SOC.
- Correlation helps identify attacks by combining related events.
- Not every alert is a real attack; analysts must distinguish false positives from true positives.

SOC Investigation Notes

Indicators Observed

- Multiple failed login attempts
- Successful login after repeated failures
- Unexpected PowerShell execution
- Unauthorized administrator account creation
- Connection to an unknown IP address
- Antivirus disabled

Investigation Plan

- Review Windows Event Logs
- Analyze Sysmon logs
- Check network connections
- Review user activity
- Verify whether sensitive data was accessed

Response Plan

- Isolate the affected endpoint
- Disable unauthorized administrator account
- Block malicious IP address
- Reset affected credentials
- Escalate the incident
- Document findings and actions
