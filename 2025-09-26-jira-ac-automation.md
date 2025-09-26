# Automating Jira Acceptance Criteria for New AWS Account Requests

## Context

When a customer requests a new AWS account, a Jira ticket is automatically generated containing a list of acceptance criteria (ACs). These ACs were often **out-of-date**, causing:

- Confusion about which ACs need manual checking  
- Slower verification times for new account vending  
- Inconsistency in verification of new accounts  

The goal was to **enable the team to maintain up-to-date ACs directly in Jira** and to ensure only ACs requiring manual testing are included.

---

## Problem Statement

Existing Jira tickets:

- Include ACs already covered by automated tests  
- Require manual intervention to update ACs  
- Automatically create unnecessary “testing notes” subtasks  

This created inefficiencies for cloud engineers verifying new accounts.

---

## Objective

- Replace outdated ACs in Jira tickets with up-to-date template ACs  
- Restrict changes only to tickets labeled `newAWSaccountrequest`  
- Remove unnecessary “testing notes” subtasks  
- Commit updated automation rules to the GitHub repository  
- Ensure proper versioning and labels (`CR` / `non-CR`) for traceability  

---

## Tools & Technologies Used

- **Jira Automation Rules** – to update ACs automatically  
- **GitHub** – for version-controlled automation rules  
- **Sandbox Jira instance** – for testing before production deployment  
- **AWS Account Request workflow** – domain context for testing and validation  

---

## My Contribution

1. Developed a **new Jira automation rule** in the sandbox environment.  
2. Tested the rule by creating tickets to verify AC replacement and removal of unnecessary subtasks.  
3. Exported the rule as a JSON file and submitted a **Pull Request** to the team repository.  
4. Sanitized sensitive info (API tokens, URLs, email addresses) before committing.  
5. Verified versioning and applied `CR/non-CR` labels.  
6. Deprecated the old template ticket and linked it appropriately.

---

## Testing Approach

- Tested in **sandbox Jira**  
- Verified AC replacement on new tickets  
- Confirmed “testing notes” subtasks were no longer created  
- Simulated edge cases to catch potential issues  
- Prepared for **blue-green deployment** in production

---

## Outcome

- Jira tickets now automatically contain **up-to-date ACs**  
- Only relevant tickets are affected  
- Manual errors and time spent verifying new accounts are reduced  
- Legacy subtasks removed, cleaning up ticket workflows  
- Team repository now contains **versioned automation rules** for traceability  

---

## Key Learnings

- Jira automation rules can significantly **reduce manual work**  
- Sandbox testing is essential for catching issues early  
- Sanitizing sensitive information is critical before committing  
- Documentation ensures work is **reproducible and shareable**  
- Versioning and PRs improve **team transparency and auditability**

---

## References

- Sandbox testing environment  
- Deprecated template ticket  
- Team GitHub repository for automation rules
