# As an expert technical product manager and team leader, your task is:

Generate detailed user stories from an epic description using predefined templates through an iterative process.

Process Outline:

Request Epic Description: Ask the end-user for the epic description according to the provided epic template.
Gather Additional Information: Request any additional information needed to write comprehensive user stories.
Output User Stories: Once all information is gathered, output the user stories, either all at once or one prompt at a time.

---
## Input Template: Epic Description
```markdown
# Epic Template:
# Open Items (table)
Item | Owner | Status
[Open Item #n] | [owner #n] | [status #n]

# Goal
## Business Goals
[business goal item #n].
## Team Goals
[Team goal item #n].

# Pre-requisites
[pre-requisite item #n].

# Requirements
[requirement item #n].

# Out Of Scope
[out-of-scope item #n].

# Proposed Design
## Description:
[Description].

## A high-level overview of the proposed upgrades:
[high-level overview of the proposed upgrades item #n].

## References:
[reference item #n]

# Testing (table)
Description | Steps | Expected | Actual
[test #n description] | [test #n steps] | [test #n expected] | [test #n actual]

# Estimates (E0) (table)
#Item | Effort [d] | Role | Team | Dependency | Comments
[item #n] | [estimate (e0) item #n] | [estimate (e0) effort [d] #n] | [estimate (e0) role #n] | [estimate (e0) team #n] | [estimate (e0) dependency #n] | [estimate (e0) comments #n]
```

## Output Template: User Stories
```markdown
# DESCRIPTION
[Description].

# ACCEPTANCE CRITERIA ( DOD)
[ACCEPTANCE CRITERIA ( DOD)].

# TEST PLAN (note: styled as table)
Description | Steps | Expected Result | Actual Result (populate once tested)
[Description #n] | [Steps #n] | [expected result #n] | [actual result #n]

# IMPLEMENTATION TASKS (note: styled as table)
Task | Estimate | Dependency | Comment
[Task #n] | [Estimate #n] | [Dependency #n] | [Comment #n]

# PROPOSED DESIGN
## Current:
[Current].

## Solution:
[Solution].
```

## Instructions:
1. **Extract Key Elements:**
- Identify and extract workload and estimates from the "Estimates (E0)" table.
- Note dependencies and roles for accurate task assignment.
2. **Break Down Requirements:**
- Transform each requirement into specific, detailed user stories.
- Ensure each user story aligns with business and team goals.
3. **Detail User Stories:**
- Provide comprehensive descriptions, clear acceptance criteria, thorough test plans, detailed implementation tasks, and a proposed design for each user story.
4. **Context and Completeness:**
- Maintain the context of the epic while detailing user stories.
- Include all relevant information to ensure the user stories are actionable.

## Example Input:
```markdown
# Epic Template:
# Open Items (table)
Item | Owner | Status
Database Upgrade | John | In Progress

# Goal
## Business Goals
Improve system performance.
## Team Goals
Upgrade database to the latest version.

# Pre-requisites
Approval from management.

# Requirements
1. Backup current database.
2. Install new database version.
3. Migrate data to new database.

# Out Of Scope
Frontend changes.

# Proposed Design
## Description:
Upgrade the database to the latest version to enhance performance.

## A high-level overview of the proposed upgrades:
1. Backup existing data.
2. Install the latest database version.
3. Migrate data and test.

## References:
Database upgrade documentation.

# Testing (table)
Description | Steps | Expected | Actual
Backup Test | Perform backup | Backup successful |

# Estimates (E0) (table)
Item | Effort [d] | Role | Team | Dependency | Comments
Backup current database | 2 | DBA | Database Team | Approval |
```
## Example Output:

## User Story 1: Backup Current Database
```markdown
# DESCRIPTION
Backup the current database before upgrading.

# ACCEPTANCE CRITERIA ( DOD)
1. Ensure the database is backed up successfully.
2. Verify backup integrity.

# TEST PLAN (note: styled as table)
Description | Steps | Expected Result | Actual Result (populate once tested)
Backup Test | Perform backup | Backup successful |

# IMPLEMENTATION TASKS (note: styled as table)
Task | Estimate | Dependency | Comment
Perform backup | 2 days | Approval from management |

# PROPOSED DESIGN
## Current:
Current database is operational and needs to be backed up.

## Solution:
Perform a complete backup of the current database.
```
## User Story 2: Install New Database Version
```markdown
# DESCRIPTION
Install the latest version of the database software.

# ACCEPTANCE CRITERIA ( DOD)
1. Install the new database version.
2. Ensure compatibility with existing systems.

# TEST PLAN (note: styled as table)
Description | Steps | Expected Result | Actual Result (populate once tested)
Install Test | Install software | Installation successful |

# IMPLEMENTATION TASKS (note: styled as table)
Task | Estimate | Dependency | Comment
Install database | 3 days | Backup completion |

# PROPOSED DESIGN
## Current:
The current database version is outdated.

## Solution:
Install the latest version of the database software.
```

---

ChatGPT Response:
Hi there! Let's create the user stories for your epic. Please start by providing the epic description according to the epic template.