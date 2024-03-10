
Postmortem: Web Application Downtime

Issue Summary:

Duration: Start Time: March 10, 2024/9:25 a.m/EAT
End Time: March 10, 2024/11:29/EAT
Impact:
• The web application experienced downtime for approximately 2 hours.
• Users were unable to access the service, resulting in a 100% outage for all users.

Root Cause:
• A misconfigured database connection pool caused the web application to exhaust
available database connections, leading to service downtime.

Timeline:

Issue Detected:
• Time: March 10, 2024/9:42 a.m/EAT
• Detection Method: Monitoring alerts indicated a sudden increase in HTTP 500 errors.

Actions Taken:
• Investigation focused on examining server logs and database performance metrics.
• Initial assumption: Suspected database overload due to high traffic or inefficient queries.

Misleading Paths:
• Initially investigated potential DDoS attacks or network issues, but network monitoring
showed no anomalies.

Escalation:
• The incident was escalated to the DevOps team for further investigation and resolution.

Resolution:
• The misconfigured database connection pool was identified as the root cause.
• Connection pool settings were adjusted to increase the maximum number of connections
and optimize connection reuse.
• Database server resources were also upgraded to handle higher connection loads.

Root Cause and Resolution:

Root Cause Explanation:
• The web application's database connection pool was misconfigured, leading to the
exhaustion of available database connections.
• As a result, the application was unable to establish new connections to the database,
causing downtime.

Resolution Explanation:
• Adjustments were made to the connection pool configuration to increase the maximum
number of connections and optimize connection reuse.
• Additionally, database server resources were upgraded to ensure sufficient capacity to
handle peak loads and prevent future connection pool exhaustion.

Corrective and Preventative Measures:

Improvements/Fixes:
• Implement automated monitoring of database connection pool usage to detect and
prevent future connection pool exhaustion.
• Conduct regular reviews of database configuration settings to identify and address
potential performance bottlenecks.

Tasks to Address the Issue:
1. Update database connection pool configuration to increase maximum connections.
2. Implement automated alerts for abnormal database connection pool usage.
3. Schedule regular performance reviews and capacity planning for database resources.
4. Document and communicate the incident response process to improve coordination
during future outages.
