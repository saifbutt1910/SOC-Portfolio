Week 2 Day 8 - SOC Incident Investigation #1

Incident Summary

35 failed login attempts (Event ID 4625) were detected against the `finance_admin` account from the same IP address, followed by a successful login (Event ID 4624) five minutes later.

Initial Assessment

The activity is suspicious and may indicate a brute-force attack. However, additional investigation is required before confirming malicious activity.

Investigation Steps

- Check whether the source IP is recognized.
- Review Windows Security Logs for related events.
- Check for previous failed logins and account activity.
- Review Sysmon logs for suspicious processes, commands or file downloads.
- Analyze network connections after the successful login.

Recommended Actions

- If malicious activity is confirmed, temporarily disable the account.
- Force a password reset.
- Block the malicious IP address.
- Escalate the incident to the security team.
- Document all findings and actions taken.

What I Learned Today

- A successful login after many failed attempts requires investigation.
- Analysts should consider both malicious and legitimate explanations.
- Decisions should be based on evidence, not assumptions.
- Building a timeline helps understand the sequence of events.
