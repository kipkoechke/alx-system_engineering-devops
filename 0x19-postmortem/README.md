# **Incident Postmortem Report: Service Interruption on January 20, 2024**

### Summary
On January 20, 2024, our system underwent a service disruption that spanned 2 hours. During this period, our services were inaccessible to our users, and some data was unfortunately lost. The primary cause of the incident was traced back to a hardware malfunction in one of our data centers.

*Timeline (All the times are in EAT time-zone):*

  1. 9:00 AM: Our surveillance system signaled an issue with one of our servers in Data Center A.
  2. 9:15 AM: Our team initiated an investigation into the problem and found that the server had suffered a hardware malfunction.
  3. 8:30 AM: We tried to switch to our backup server, but it too failed due to a software glitch.
  4. 10:00 AM: We escalated the problem to our hardware supplier for additional assistance.
  5. 11:30 AM: The hardware supplier replaced the defective hardware and reinstated service to the affected server.
  6. 11:45 AM: We verified that all services were back online and started monitoring the system for any further complications.

### Root Cause

The incident's root cause was a hardware malfunction in one of our servers in Holberton. A defective power supply unit caused the failure, leading to data loss and the subsequent service interruption.

### Consequences

The interruption impacted all users trying to use our services during the downtime, leading to lost productivity and potential revenue. Additionally, the interruption led to the loss of some data, causing data integrity concerns.

### Mitigation 

To avoid a similar incident in the future, we have undertaken the following measures:

  - We have replaced the defective power supply unit and carried out a comprehensive review of all hardware in Holberton Data Center.
  - We have set up an automatic failover mechanism for our backup server to avoid future service interruptions.
  - We have revised our incident response protocols to ensure quicker escalation to our hardware supplier for extra support.

### Closing Remarks

We extend our apologies for the inconvenience this incident caused our users and clients. We take this incident with utmost seriousness and have implemented measures to prevent a recurrence. We will persist in monitoring our systems and enhancing our incident response protocols to reduce the impact of any future incidents.


