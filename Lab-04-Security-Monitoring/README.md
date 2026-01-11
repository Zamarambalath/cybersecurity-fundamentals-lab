# Lab 04 – Security Monitoring & Alert Triage (Mini Lab)

## Objective
Understand the basics of security monitoring by reviewing alerts, determining severity, and deciding appropriate response actions.

## Scenario
A security monitoring system generates an alert indicating multiple failed login attempts followed by a successful login from an unfamiliar IP address.

The alert details are as follows:
- Username: admin
- Failed login attempts: 6
- Source IP: 185.220.101.45
- Successful login occurred 2 minutes after failures
- Login time: 02:14 AM (outside normal business hours)

## Alert Analysis

### Indicators Observed
- Multiple failed authentication attempts
- Successful login shortly after failures
- Login occurred outside normal working hours
- Source IP is unfamiliar

### Severity Assessment
**Medium to High**

Reasoning:
The pattern may indicate a brute-force attempt that resulted in successful access.

### Recommended Actions
- Flag the account for review
- Force password reset for the affected user
- Check login history for further suspicious activity
- Monitor the IP address for additional attempts
- Escalate to security team if confirmed malicious

## Key Security Takeaways
- Monitoring login behavior is critical for early threat detection
- Time-based anomalies can indicate compromise
- Quick response reduces potential impact

## Security Summary

This lab reinforced how small misconfigurations or repeated authentication failures can indicate early-stage attacks.  
By reviewing system behavior and logs, I practiced identifying patterns that could suggest brute-force attempts or misuse.  
This highlights the importance of continuous monitoring and structured log analysis in detecting incidents early.
