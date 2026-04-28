# Simple Google Sheets Database Design

Google Sheets can be used as a simple database for beginner application prototypes. It is not suitable for large or secure production systems, but it is useful for early-stage learning, prototyping, and demonstration.

## Example Project

**Student Facility Complaint System**

## Sheet 1: Complaints

| Column Name | Description |
|---|---|
| complaint_id | Unique ID for each complaint |
| student_name | Name of student submitting complaint |
| matric_no | Student matric number |
| category | Type of complaint |
| location | Location of the issue |
| description | Complaint details |
| photo_url | Link to uploaded photo, if available |
| date_submitted | Date complaint was submitted |
| status | New, In Progress, Resolved, Rejected |
| staff_remark | Staff update or comment |

### Example

| complaint_id | student_name | matric_no | category | location | description | photo_url | date_submitted | status | staff_remark |
|---|---|---|---|---|---|---|---|---|---|
| C001 | Andi | TI001 | Wi-Fi | Lab 2 | Wi-Fi is unstable | link | 2026-04-28 | New | Pending review |

## Sheet 2: Users

| Column Name | Description |
|---|---|
| user_id | Unique user ID |
| name | User name |
| role | Student, Staff, Admin |
| email | User email |
| password | Password for prototype only |

### Example

| user_id | name | role | email | password |
|---|---|---|---|---|
| U001 | Andi | Student | andi@example.com | 12345 |
| U002 | Budi | Staff | budi@example.com | 12345 |

## Sheet 3: Categories

| Column Name | Description |
|---|---|
| category_id | Unique category ID |
| category_name | Complaint category |

### Example

| category_id | category_name |
|---|---|
| CAT001 | Wi-Fi |
| CAT002 | Projector |
| CAT003 | Air-conditioning |
| CAT004 | Furniture |
| CAT005 | Cleanliness |
| CAT006 | Electrical issue |

## Sheet 4: Status History

| Column Name | Description |
|---|---|
| history_id | Unique history ID |
| complaint_id | Related complaint ID |
| old_status | Previous complaint status |
| new_status | Updated complaint status |
| updated_by | Staff or admin who updated the status |
| updated_at | Date and time of update |
| remark | Update note |

## Why Use Google Sheets?

Google Sheets is suitable for beginner prototypes because:

1. It is easy to understand.
2. It allows students to see the data directly.
3. It can be connected to simple web applications.
4. It reduces database setup complexity.
5. It helps students focus on process and data structure first.

## Limitation

Google Sheets should not be treated as a secure production database. For real systems, students should later move to proper databases such as MySQL, PostgreSQL, Firebase, or MongoDB.
