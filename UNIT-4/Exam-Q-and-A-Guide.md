# Unit 4 Exam Question & Answer Guide
*(Comprehensive Guide Solving Past Exam Questions with Model Answers and Calculations)*

This guide contains structured solutions to past exam questions for Unit 4, referencing the detailed notes files created in the workspace.

---

## Question 1: Draw a bar chart (Gantt chart) for the following task schedule starting on 1/1/2022. [5 Marks]

### **Task Schedule Table**
| Task | Effort (Person-days) | Duration (Days) | Dependencies |
| :---: | :---: | :---: | :---: |
| **T1** | 10 | 10 | None (Starts immediately) |
| **T2** | 5 | 5 | None (Starts immediately) |
| **T3** | 9 | 10 | T1 (M1) |
| **T4** | 6 | 10 | None (Starts immediately) |
| **T5** | 8 | 20 | T2, T4 (M2) |

---

### **1.1 Schedule Analysis & Date Calculations**
*   **Start Date:** 1/1/2022.
*   **T1:** Starts 1/1/2022, runs for 10 days. Finishes on **10/1/2022**. Milestone **M1** is reached.
*   **T2:** Starts 1/1/2022, runs for 5 days. Finishes on **5/1/2022**.
*   **T4:** Starts 1/1/2022, runs for 10 days. Finishes on **10/1/2022**.
*   **Milestone M2:** Requires both T2 and T4 to complete. Since T4 finishes on 10/1/2022, milestone **M2** is reached on **10/1/2022**.
*   **T3:** Depends on T1 (M1). Starts on **11/1/2022**, runs for 10 days. Finishes on **20/1/2022**.
*   **T5:** Depends on T2 and T4 (M2). Starts on **11/1/2022**, runs for 20 days. Finishes on **30/1/2022**.

---

### **1.2 Calendar Bar Chart (Gantt Chart Representation)**
```text
Dates (Jan 2022): 1..5....10...15...20...25...30
T1 [==========] (Ends 10/1 - M1)
T2 [=====] (Ends 5/1)
T4 [==========] (Ends 10/1)
M2            * (Reached 10/1)
T3            [==========] (Starts 11/1, Ends 20/1)
T5            [====================] (Starts 11/1, Ends 30/1)
```

---

## Question 2: Cost and Effort Estimation Numerical [5 Marks]
**Problem:** Consider 7 functions with their estimated lines of code. Average productivity based on historical data is **620 LOC/pm** and labor rate is **Rs. 8,000 per month**. Find the total estimated project cost and effort.
*   **Function Sizes:** F1 = 2340, F2 = 5380, F3 = 6800, F4 = 3350, F5 = 4950, F6 = 2140, F7 = 8400.

### **Step-by-Step Solution:**
1.  **Calculate Total Lines of Code (LOC):**
$$\text{Total LOC} = 2340 + 5380 + 6800 + 3350 + 4950 + 2140 + 8400$$
$$\text{Total LOC} = \mathbf{33,360 \text{ Lines of Code}}$$

2.  **Calculate Effort (Person-Months):**
$$\text{Effort} = \frac{\text{Total LOC}}{\text{Productivity}} = \frac{33,360}{620}$$
$$\text{Effort} \approx \mathbf{53.81 \text{ Person-Months}}$$

3.  **Calculate Total Project Cost:**
$$\text{Total Cost} = \text{Effort} \times \text{Labor Rate}$$
$$\text{Total Cost} = 53.81 \text{ PM} \times \text{Rs. } 8,000/\text{Month}$$
$$\text{Total Cost} = \mathbf{\text{Rs. } 430,480}$$

*   **Final Answer:** Estimated Effort = **53.81 Person-Months**, Estimated Project Cost = **Rs. 430,480**.

---

## Question 3: Taking the example of an RFID-Based Attendance Management System, write the project plan components. [5 Marks]
*   **Related Notes:** [6.Plan-Driven-Development.md](6.Plan-Driven-Development.md)

Applying the 7 project plan sections to an RFID Attendance System:
1.  **Introduction:** 
    *   *System Goal:* Create an automated system that registers student attendance when their RFID cards scan at classroom doors.
    *   *Constraints:* Must be delivered in 4 months, budget limit of Rs. 2,00,000.
2.  **Project Organization:**
    *   *Team Roles:* 1 Project Manager (Liaison), 1 Hardware Engineer (RFID reader installation & testing), 2 Software Developers (Database and web portal programming), 1 QA tester.
3.  **Risk Analysis:**
    *   *Identified Risk:* Delay in hardware delivery (RFID card readers).
    *   *Mitigation:* Order readers in Week 1; simulate hardware using software simulators during early software coding.
4.  **Hardware and Software Resource Requirements:**
    *   *Hardware:* 10 RFID scanner modules, 500 blank RFID student cards, 1 central database server.
    *   *Software:* MySQL database, Python (for reading serial ports), React.js (for the web attendance dashboard).
5.  **Work Breakdown Structure (WBS):**
    *   *Activities:* WBS 1: Hardware installation; WBS 2: Database schema design; WBS 3: UI integration; WBS 4: System validation testing.
6.  **Project Schedule:**
    *   Define milestones: M1 (Hardware installed - Week 6), M2 (Database integrated - Week 10), M3 (System Testing Complete - Week 14).
7.  **Monitoring and Reporting Mechanisms:**
    *   Hold weekly team stand-ups. Bi-weekly progress reports submitted to the college dean.

---

## Question 4: For a group of students doing a major project in a semester course, list the major risks a typical project will face. [5 Marks]
*   **Related Notes:** [2.Risk-Management.md](2.Risk-Management.md)

For a student team, risks differ slightly from corporate projects. The 6 major risks are:
1.  **Team Conflict / Lack of Cohesion (People Risk):** Students clashing over technology choices or unequal division of labor.
2.  **Poor Time Management (Estimation Risk):** Underestimating the time needed, resulting in cramming code in the final week before submission.
3.  **Technology Learning Curve (Technology Risk):** Selecting complex, unfamiliar technologies (e.g., machine learning, block-chain) and spending months learning them without writing core code.
4.  **Requirement Scope Creep (Requirements Risk):** The project guide or advisor continuously changing project specifications or adding new features close to the deadline.
5.  **Academic Workload Clashes (People Risk):** Team members becoming unavailable during mid-semester exams, laboratory tests, or placement drives.
6.  **Tool/Hardware Failures (Tools Risk):** Crucial physical parts (e.g., microcontrollers, sensors) burning out or laptops crashing without Git backups.

---

## Question 5: Classify the following situations into Project, Product, or Business Risk: [8 Marks]
*   **Related Notes:** [2.Risk-Management.md](2.Risk-Management.md)

1.  *Hardware that is essential for the project will not be delivered on schedule:* **Project Risk** (directly impacts the calendar schedule).
2.  *Experienced staff will leave the project before it is finished:* **Project Risk** (affects team staffing resource limits).
3.  *The underlying technology on which the system is built is superseded by new technology:* **Business Risk** (affects the long-term sales and competitive position of the organization).
4.  *A competitive product is marketed before the system is completed:* **Business Risk** (affects market capture and corporate viability).

---

## Quick-Map for Theory Questions:
*   **Explain the Risk Management Process with a neat diagram:** Map to [2.Risk-Management.md (Section 3)](2.Risk-Management.md#3-the-risk-management-process).
*   **Discuss Maslow’s Hierarchy of Needs:** Map to [3.Managing-People.md (Section 3)](3.Managing-People.md#3-motivating-people-maslows-hierarchy-of-needs).
*   **Identify the issues/challenges with software project management:** Map to [1.Introduction-to-Project-Management.md (Section 2)](1.Introduction-to-Project-Management.md#2-why-software-management-is-uniquely-challenging).
*   **Discuss the factors influencing Project Management:** Map to [1.Introduction-to-Project-Management.md (Section 3)](1.Introduction-to-Project-Management.md#3-factors-affecting-project-management-style).
*   **Discuss the factors that affect the group Communications:** Map to [4.Teamwork.md (Section 5)](4.Teamwork.md#5-group-communications).
*   **Describe any two cost estimation techniques (Algorithmic vs. Expert/Experience):** Map to [9.Estimation-Techniques.md (Section 2)](9.Estimation-Techniques.md#2-types-of-estimation-techniques).

