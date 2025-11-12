
### **Prompt:**

**Role:** You are a senior business analyst and technical writer specializing in higher education administrative processes.

**Task:** Analyze the provided meeting transcript to produce a comprehensive report. The report must synthesize the discussion into a structured format, focusing on workflows, problems, and actionable solutions.

**Input:** A raw transcript from a meeting involving multiple participants discussing technical and procedural issues in a financial aid office.

---

### **Output Requirements**

You must format the entire output as a single Markdown document.

1. **Main Title (H1):** The very first line must be a Level 1 Markdown heading (`#`). This title should be a concise and descriptive summary of the meeting's primary topic, which you will derive from the transcript's content (e.g., `# Financial Aid Process Review: ISIR Locking and C-Flag Handling`).
    
2. **Report Structure (H2 Headings):** The body of the report must be divided into the following sections, each starting with a Level 2 Markdown heading (`##`):
    
    - `## Current Processes and Procedures`
        
        - Describe the existing workflows and procedures as they are currently practiced (e.g., which ISIRs are locked, how C flags are currently reviewed).
            
    - `## Identified Problems`
        
        - Detail all problems, inefficiencies, and negative consequences associated with the current processes (e.g., manual work required, missed tracking requirements, data disconnects, effects on packaging and disbursement).
            
    - `## Proposed Solutions and New Workflows`
        
        - Clearly outline each solution proposed during the meeting.
            
        - Explain how the new, proposed workflow would function (e.g., "Stop locking packaged ISIRs," "Handle C flags entirely on RRAAREQ").
            
        - Include any discussion of risk management or potential trade-offs for the new workflow.
            
    - `## Implementation Requirements and Step-by-Step Instructions`
        
        - This is the most critical section. You must extract and detail all requirements needed to implement the proposed solutions.
            
        - **Data and Reporting:** Specify any new reports that need to be created, data that must be reviewed, or changes to data entry practices.
            
        - **Software Configuration:** Explicitly list any configuration changes needed for software systems mentioned (e.g., **Banner Financial Aid**, **Banner Student Forms**, **Scholarship Universe**, **Argos**).
            
        - **Detailed Instructions:** Provide **detailed, step-by-step instructions** for any new procedure or configuration change discussed. If the transcript provides the logic (e.g., "tell Banner to ignore the C flag"), formulate the instructional step (e.g., "1. Access the relevant Banner settings page. 2. Locate the two options to 'Ignore the C flag.' 3. Enable these settings for both Pell and general disbursement.").
            
    - `## Action Items`
        
        - List any specific tasks assigned to individuals, including who is responsible and what the task is (e.g., "Kenneth: Create a new report to identify packaged students with an SAI change.").
            

---

**[PASTE MEETING TRANSCRIPT HERE]**