# Reviewpad Configurations

This directory contains Reviewpad configuration files.

## Configurations

### [Require approval by senior reviewers](./require-approval-from-senior-reviewers.yml)

This configuration blocks the merge until a senior reviewer from the author's team approves the pull request.

We assign the senior reviewers for each GitHub team using a dictionary in the configuration file. 
The dictionary key is the GitHub team name, and the value is a list of GitHub usernames.

---

### [Require multiple approvals in sequence](./require-multiple-approvals-in-sequence.yml)

This configuration blocks the merge until a senior reviewer from the author's team approves the pull request.

Additionally, depending on the changes, the pull request may require approval from other teams.

This approval is required in sequence, i.e., the pull request must be approved by the senior reviewer first, and then by the other team.

--- 

### [Block on code freeze label](./block-on-code-freeze-label.yml)

This configuration blocks the merge if the pull request has a label `code-freeze`.

This label could also be automatically added by other Reviewpad workflows.

---

### [Block on checklist](./block-on-checklist.yml)

This configuration blocks the merge if the pull request does not
have all the checklist items checked.

---

