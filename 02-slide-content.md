# Slide Content

## Slide 1: Title

# From Scenario to Application  
## A Quick Way to Formulate Problems Using Generative AI

For S1 Teknik Informatika  
Fakultas Teknik, Universitas Negeri Malang

---

## Slide 2: The Main Problem

Many students begin with:

- "I want to build a mobile app."
- "I want to use AI."
- "I want to make a dashboard."
- "I want to create a web system."

However, a better student begins with:

- Who has the problem?
- What is currently difficult?
- What process is inefficient?
- What data is needed?
- What decision should the system support?

**Key point:**  
Application development must start from the **problem scenario**, not from the technology.

---

## Slide 3: Common Student Mistake

Weak project idea:

> I want to develop a student attendance system using QR code.

This sounds like a system idea, but the problem is still unclear.

Better questions:

1. Who uses the system?
2. What is wrong with the current attendance process?
3. Is the problem about cheating, slow recording, missing records, manual reporting, or lecturer workload?
4. What evidence shows this problem exists?
5. What data should be collected?
6. What output should the system produce?

---

## Slide 4: Scenario Is the Key

A scenario is a short but detailed explanation of the real situation.

A good scenario contains:

| Element | Guiding Question |
|---|---|
| User | Who faces the problem? |
| Context | Where does the problem happen? |
| Current process | How is it done now? |
| Pain point | What is difficult, slow, risky, or inefficient? |
| Data | What information is involved? |
| Impact | What happens if the problem is not solved? |
| Proposed support | How can an application help? |

---

## Slide 5: Simple Framework

Use this formula:

> User + Context + Current Process + Problem + Impact + Data + Proposed Application

Example:

> In a university class, lecturers still record student attendance manually using paper or spreadsheet. This process takes time, may produce missing records, and makes it difficult to generate attendance reports quickly. The system needs student data, course data, class schedule, attendance records, and report output. Therefore, a simple attendance management application can help lecturers record, verify, and monitor attendance more efficiently.

---

## Slide 6: Before and After Example

### Weak version

> I want to build a complaint system for students.

### Better version

> Students often report facility problems such as broken projectors, Wi-Fi issues, damaged chairs, or air-conditioning problems through informal channels such as WhatsApp. These reports may be missed, duplicated, or delayed because there is no structured tracking process. A complaint management application can help students submit complaints, allow staff to update status, and help the faculty monitor unresolved issues using simple report data.

This version is better because it explains:

1. Real users
2. Real context
3. Current process
4. Pain point
5. System function
6. Data and output

---

## Slide 7: How Generative AI Helps

Generative AI should not replace thinking. It should support thinking.

Use AI to:

1. Clarify the problem scenario
2. Identify stakeholders
3. Extract functional requirements
4. Suggest data fields
5. Generate user stories
6. Propose UI screens
7. Draft database structure
8. Create initial code or prototype

---

## Slide 8: Recommended AI Workflow

### Step 1: Write the raw scenario

Student writes the messy real-world situation.

### Step 2: Ask AI to clarify the problem

Use ChatGPT or Claude to extract:

1. Stakeholders
2. Problem statement
3. Root cause
4. System objective
5. Functional requirements
6. Data requirements

### Step 3: Ask AI to generate user stories

Example:

> As a student, I want to submit a complaint so that the faculty can respond to facility problems.

### Step 4: Ask AI to suggest database fields

Use Google Sheets first for a simple prototype.

### Step 5: Ask Google Stitch to generate UI

Use a clear prompt based on the scenario.

### Step 6: Use GitHub

Store documentation, screenshots, prompt history, and source code.

---

## Slide 9: Prompt 1 — Scenario Clarification

```text
Act as a software engineering lecturer. I am a first-year Informatics student. 
Help me analyse the following scenario before I build an application.

Scenario:
[PASTE SCENARIO HERE]

Please produce:
1. Main problem
2. Target users
3. Current manual process
4. Pain points
5. Impact of the problem
6. Proposed application idea
7. Functional requirements
8. Non-functional requirements
9. Data needed
10. Possible simple database tables
Use simple language suitable for a beginner.
```

---

## Slide 10: Prompt 2 — Turning Scenario into Project Title

```text
Based on the scenario below, suggest 5 suitable application development project titles.

Scenario:
[PASTE SCENARIO HERE]

The title must:
1. Be suitable for first-year Informatics students
2. Focus on solving the problem
3. Avoid overclaiming
4. Be simple enough to develop as a prototype
5. Include the target user or application context
```

---

## Slide 11: Prompt 3 — Generate Requirements

```text
Based on this application idea:

[PASTE APPLICATION IDEA]

Generate:
1. 5 functional requirements
2. 5 non-functional requirements
3. 5 user stories
4. Main modules
5. Simple database fields using Google Sheets
6. Suggested screens for the user interface
Keep the scope simple for beginner students.
```

---

## Slide 12: Prompt 4 — Google Stitch UI Prompt

```text
Design a simple web application interface for a student facility complaint system.

Target users:
1. Students
2. Faculty staff
3. Admin

Main functions:
1. Submit complaint
2. Upload complaint photo
3. View complaint status
4. Update complaint progress
5. Generate simple complaint report

Design style:
Clean, simple, student-friendly, suitable for university use.

Create screens for:
1. Login
2. Student dashboard
3. Complaint submission form
4. Complaint status page
5. Staff dashboard
6. Admin report page
```

---

## Slide 13: Simple Google Sheets Database Example

For a beginner prototype, Google Sheets can act as a simple database.

### Sheet: Complaints

| complaint_id | student_name | matric_no | category | location | description | date_submitted | status | staff_remark |
|---|---|---|---|---|---|---|---|---|

### Sheet: Users

| user_id | name | role | email | password |
|---|---|---|---|---|

### Sheet: Categories

| category_id | category_name |
|---|---|

Example categories:

1. Wi-Fi
2. Projector
3. Air-conditioning
4. Furniture
5. Cleanliness
6. Electrical issue

---

## Slide 14: GitHub Advantage

Students should use GitHub not only for code, but also for project discipline.

Suggested GitHub repository structure:

```text
project-name/
│
├── README.md
├── problem-scenario.md
├── requirements.md
├── ui-design/
│   ├── screenshots/
│   └── stitch-prompts.md
├── database/
│   └── google-sheets-structure.md
├── source-code/
└── reflection.md
```

The important part is not only the final system. The important part is showing the thinking process from:

> Scenario → Problem → Requirement → Design → Prototype

---

## Slide 15: Mini Activity

Weak idea:

> I want to build a food ordering app for campus.

Improve it using this structure:

1. Who is the user?
2. What is the current problem?
3. What happens now?
4. Why is it inefficient?
5. What data is needed?
6. What should the app help users do?
7. What is the simplest version of the app?

Expected improved version:

> Students on campus often face long queues when buying food during lunch hours. Some students do not know which food stalls are open or whether certain menu items are still available. Stall operators also handle orders manually, which may cause delays and order mistakes. A simple campus food pre-ordering application can help students view menus, place orders, and check order status, while stall operators can manage incoming orders using a simple dashboard.

---

## Slide 16: Closing Message

Do not start with:

> What technology should I use?

Start with:

> What problem am I solving?

Then use generative AI to help you refine the scenario, identify the real problem, design the workflow, generate UI ideas, prepare a simple database, and document the project properly.

**Final takeaway:**

> A good application is not built from coding skills alone. It is built from a clear understanding of the problem.
