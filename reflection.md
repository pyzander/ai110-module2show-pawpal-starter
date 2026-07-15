# PawPal+ Project Reflection

## 1. System Design

Worked with Richard Devitt and Badhan Barua 

Step 1: Understand the Problem 

3 core actions that the user should be able to perform: 

* add a pet 
* add/edit/delete a activity 
* see activities / view schedule/calendar 

Step 2: List the Building Blocks

Brainstorm the main objects needed for the system. For each object, determine:

What information it needs to hold (attributes)

What actions it can perform (methods)

Objects (attributes and methods listed as bullet points 

* pet 
    - petID PK 
    - name 
    - type 
    - age 
    - activities - list of activityIDs 
* pet-activity 
    - pet-activityID PK 
    - petID FK 
    - activity FK 
    - priority int (0-5)
    - owner_preferences int (0-5)
* activity 
    - activityID  PK 
    - type (ex: walks, feeding, meds, enrichment, grooming,etc) 
    - duration 
    - timeStart 
    - timeEnd 
* calendar 
    - calendarID 
    - list of acitivityIDs 
    - method to track available times 

**a. Initial design**

- Briefly describe your initial UML design.
- What classes did you include, and what responsibilities did you assign to each?

**b. Design changes**

- Did your design change during implementation?
- If yes, describe at least one change and why you made it.



* I need to change the type ot Mermaid class and edit diagrams/uml.mmd 
    - I definitely should've reviewed the step 
* calendar should include petActivityIds instead 
* timeStart and timeEnd should be on petActivityIds 
    - having duration and timeStart and timeEnd together are redundant 
* 

---

## 2. Scheduling Logic and Tradeoffs

**a. Constraints and priorities**

- What constraints does your scheduler consider (for example: time, priority, preferences)?
- How did you decide which constraints mattered most?

**b. Tradeoffs**

- Describe one tradeoff your scheduler makes.
- Why is that tradeoff reasonable for this scenario?

---

## 3. AI Collaboration

**a. How you used AI**

- How did you use AI tools during this project (for example: design brainstorming, debugging, refactoring)?
- What kinds of prompts or questions were most helpful?

**b. Judgment and verification**

- Describe one moment where you did not accept an AI suggestion as-is.
- How did you evaluate or verify what the AI suggested?

---

## 4. Testing and Verification

**a. What you tested**

- What behaviors did you test?
- Why were these tests important?

**b. Confidence**

- How confident are you that your scheduler works correctly?
- What edge cases would you test next if you had more time?

---

## 5. Reflection

**a. What went well**

- What part of this project are you most satisfied with?

**b. What you would improve**

- If you had another iteration, what would you improve or redesign?

**c. Key takeaway**

- What is one important thing you learned about designing systems or working with AI on this project?