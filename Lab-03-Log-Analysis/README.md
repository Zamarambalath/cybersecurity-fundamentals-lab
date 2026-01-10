# Lab 03 – Log Analysis Basics (Mini Lab)

## Objective
Learn how to analyze basic system and authentication logs to identify suspicious activity and understand how logs support incident detection.

## Scenario
A system administrator noticed unusual login activity on a workstation. You are asked to review log entries and identify potential indicators of suspicious behavior.

## Log Sample

Jan 10 18:45:21 workstation sshd[1024]: Failed password for invalid user admin from 203.0.113.45 port 51432
Jan 10 18:45:25 workstation sshd[1024]: Failed password for invalid user admin from 203.0.113.45 port 51435
Jan 10 18:45:30 workstation sshd[1024]: Failed password for invalid user admin from 203.0.113.45 port 51440
Jan 10 18:46:10 workstation sshd[1024]: Accepted password for user john from 192.168.1.10 port 60214

## Analysis

- Multiple failed SSH login attempts were observed for the user "admin" from IP address 203.0.113.45.
- This indicates a possible brute-force or credential guessing attempt.
- A successful login for user "john" occurred from a different internal IP address.
- No further suspicious activity was observed after the successful login.

## Conclusion

The activity suggests a potential brute-force attempt targeting the admin account.
Monitoring and account lockout policies should be reviewed to prevent future attempts.
