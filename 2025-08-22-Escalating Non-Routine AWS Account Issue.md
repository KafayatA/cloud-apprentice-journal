# Escalation of Non-Routine AWS Account Creation Issue

## Date
2025-08-22

## Context
A customer request was received by the Cloud Foundation team to create a new AWS account. The task involved standard account provisioning; however, during execution, a non-routine problem arose that required escalation in line with established procedures. Handling this correctly ensured compliance with team processes and prevented duplication of AWS accounts, minimizing operational risk.

---

## Problem Statement
During the account creation workflow, an error occurred:  
The combination of Application-Name and Environment-Type: is not unique.

Investigation revealed that an AWS account with the requested name already existed in the requested environment (test). The challenge involved determining the appropriate course of action while following escalation procedures and maintaining communication with both the requestor and the team.

---

## Objective
- Escalate the non-routine problem following internal procedures.  
- Resolve the conflict regarding the requested AWS account while maintaining compliance and documentation.  
- Determine a solution that satisfies the customer’s requirements while avoiding duplication of resources.  
- Ensure closure of the ticket aligns with team best practices and Jira board standards.

---

## Tools & Technologies Used
- AWS  
- ServiceNow  
- Jira  
- Internal team communication channels (e.g., Slack/Teams)  

---

## My Contribution
1. Volunteered to take ownership of the ticket despite limited prior experience with account vends.  
2. Investigated the error and identified that an AWS account with the same name already exists in the test environment.  
3. Escalated the issue to team members and communicated findings to ensure proper guidance.  
4. Contacted the requestor to clarify requirements and present options:  
   - Use the existing account.  
   - Submit a new request with a different account name.  
5. Collected additional context from the requestor about their need for a proper development environment.  
6. Relayed customer feedback to the team and manager; followed guidance to reference existing documentation on AWS dev environments.  
7. Confirmed the appropriate course of action and closed the ServiceNow ticket as incomplete, marking it as 'not required' in Jira per team agreement.  

---

## Testing Approach
- Verified account status in AWS to confirm the duplicate account existed.  
- Checked ServiceNow workflow logs to confirm the error was not due to a procedural failure.  
- Consulted internal documentation to ensure adherence to escalation and communication procedures.  
- Confirmed with the team and manager that closure of the ticket aligned with best practice.

---

## Outcome
- Escalation procedures were correctly followed, ensuring a non-routine problem was managed appropriately.  
- Requestor was informed and guided toward submitting a new request with a unique account name.  
- Duplication of AWS accounts was avoided.  
- The open ticket was closed correctly with team agreement, maintaining clean tracking in Jira.  
- The team gained awareness of the requestor’s need for a proper dev environment for Snowflake integration.

---

## Key Learnings
- Effective escalation requires prompt identification, clear communication, and alignment with team procedures.  
- Engaging directly with the requestor helps clarify requirements and prevent misunderstandings.  
- Documenting non-routine issues supports knowledge sharing and improves future workflow handling.  

---

## References
- ServiceNow Ticket  
- Internal AWS Account Provisioning Guidelines  


