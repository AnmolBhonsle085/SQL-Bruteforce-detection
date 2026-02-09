## SQL Brute Force Login Detection

## Project Overview
This project demonstrates how SQL can be used in cybersecurity to analyze authentication logs and detect brute-force login attempts. Authentication events are stored in a database and analyzed to identify IP addresses with repeated failed login attempts. When a defined threshold is exceeded, a security alert is generated. The project simulates a real-world SOC (Security Operations Center) log analysis and alerting workflow.

## Objectives
Store authentication log data in a relational database
Analyze failed login attempts using SQL queries
Detect potential brute-force attacks based on thresholds
Generate automated security alerts

## Tools and Technologies
MySQL
SQL (SELECT, WHERE, GROUP BY, HAVING, COUNT)
MySQL Command Line Client or MySQL Workbench

## Database Structure
auth_logs table
Stores authentication events including username, IP address, and login result (FAILED_LOGIN or SUCCESS_LOGIN)

## alerts table
Stores detected security alerts including suspicious IP address, alert type, and timestamp

## Detection Logic
The system filters authentication logs to identify failed login events. These events are grouped by IP address and counted using SQL aggregation. A threshold is applied to detect abnormal behavior. IP addresses exceeding the threshold are flagged as potential brute-force attackers.

## Alert Generation
When an IP address exceeds the defined number of failed login attempts, a security alert is created and stored in the alerts table along with the alert type and creation timestamp.

## Output
Identification of IP addresses involved in multiple failed login attempts
Generation of brute-force detection alerts
Demonstration of SOC-style threshold-based detection logic

## Key Learnings
Understanding how SQL is used in cybersecurity
Analyzing authentication logs
Detecting brute-force attack patterns
Implementing alerting logic similar to SIEM systems

## Use Cases
SOC Analyst
Security Analyst
Cybersecurity Intern
Security Log Analysis Practice

## Conclusion
This project shows how basic SQL skills can be applied in cybersecurity to analyze authentication logs, detect suspicious login behavior, and generate meaningful security alerts in a SOC-like environment.

## Author 
ANMOL BHONSLE
