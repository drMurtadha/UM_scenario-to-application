# Suggested GitHub Repository Template

Students should use GitHub not only to store code, but also to show their thinking process.

## Recommended Repository Structure

```text
project-name/
│
├── README.md
├── problem-scenario.md
├── requirements.md
├── user-stories.md
├── database/
│   └── google-sheets-structure.md
├── ui-design/
│   ├── stitch-prompts.md
│   └── screenshots/
├── source-code/
│   └── README.md
├── testing/
│   └── test-plan.md
└── reflection.md
```

## File Descriptions

### README.md

Main project overview.

Should include:

1. Project title
2. Problem scenario
3. Proposed solution
4. Target users
5. Main features
6. Tools used
7. Screenshots or prototype links

### problem-scenario.md

Explains the real-world situation before the system is developed.

Suggested structure:

```markdown
# Problem Scenario

## Background

## Target Users

## Current Process

## Pain Points

## Impact of the Problem

## Proposed Application Support
```

### requirements.md

Lists system requirements.

Suggested structure:

```markdown
# System Requirements

## Functional Requirements

1. The system shall ...
2. The system shall ...

## Non-Functional Requirements

1. The system should be easy to use.
2. The system should load within a reasonable time.
```

### user-stories.md

Captures requirements from the user perspective.

Example:

```markdown
# User Stories

1. As a student, I want to submit a complaint so that faculty staff can respond to facility problems.
2. As a staff member, I want to update complaint status so that students know the progress.
3. As an admin, I want to view complaint reports so that unresolved issues can be monitored.
```

### database/google-sheets-structure.md

Explains the simple database design.

Include:

1. Sheet names
2. Columns
3. Example records
4. Relationship between sheets

### ui-design/stitch-prompts.md

Stores prompts used in Google Stitch.

Include:

1. Prompt version
2. Target screen
3. Generated output link or screenshot
4. Reflection on what should be improved

### source-code/README.md

Explains how to run the prototype.

Include:

1. Technology stack
2. Setup instructions
3. Folder structure
4. Known limitations

### testing/test-plan.md

Simple testing plan.

Example:

```markdown
# Test Plan

| Test ID | Function | Test Case | Expected Result | Status |
|---|---|---|---|---|
| T001 | Submit complaint | Student submits valid complaint form | Complaint is saved successfully | Pass |
| T002 | View status | Student checks complaint status | Status is displayed correctly | Pass |
```

### reflection.md

Student reflection.

Suggested questions:

1. What problem does the application solve?
2. What did I learn from analysing the scenario?
3. How did generative AI help?
4. What parts of the AI output needed correction?
5. What would I improve in the next version?
