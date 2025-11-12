Here are several best-practice prompts, categorized by the task your employees are trying to accomplish.

The most important takeaway for them should be **The Golden Rule of AI Prompts: Context is Everything.**

An AI is like a brilliant, eager assistant who has never seen your database. A vague prompt like "Get student addresses" will fail. A specific prompt that provides table and column names will succeed. The "Rosetta Stone" trick (using **Help > Item Properties** in Banner) is what gives them the context they need to feed the AI.

Here are the prompt templates.

---

### 1. The "Query Explainer" (For Deconstructing Existing Code)

**Scenario:** Your employee is given a 50-line query to modify, but they don't understand what it does.

- **Bad Prompt:** `What is this? [Paste query]`
    
- **Good Prompt:**
    
    > "Act as a senior Oracle SQL developer. Explain this query to me in simple, step-by-step terms. What is the business purpose of this query? Explain what each join does and why it's using `GROUP BY`."
    > 
    > `[Paste the complex query here]`
    
- **Follow-up Prompt:**
    
    > "In that query, what does the `LEFT JOIN ON R.RRRAREQ_PIDM = S.SPRIDEN_PIDM` part mean? Why is it a `LEFT JOIN` and not an `INNER JOIN`?"
    

### 2. The "Query Generator" (For Writing New Code)

**Scenario:** Your employee needs to write a new query from scratch but is staring at a blank page. They have used the Banner "Rosetta Stone" trick to find the key tables.

- **Bad Prompt:** `Find all financial aid requirements for students.`
    
- **Good Prompt:**
    
    > "Act as a Banner data expert. Write an Oracle SQL query to find the **first name**, **last name**, and **student ID** for all students who have an unsatisfied financial aid requirement for the '2526' aid year.
    > 
    > - Student information (first name, last name, ID) is in `SATURN.SPRIDEN`.
    >     
    > - Requirement information (description, status, aid year) is in `FAISMGR.RRRAREQ`.
    >     
    > - The tables join on `SPRIDEN_PIDM` and `RRRAREQ_PIDM`.
    >     
    > - Only show me records where `RRRAREQ_SAT_IND` is 'N' and `RRRAREQ_AIDY_CODE` is '2526'."
    >     
    

### 3. The "Error Debugger" (For Fixing Their Own Code)

**Scenario:** Your employee wrote a query, but it's throwing an Oracle error message.

- **Bad Prompt:** `My query is broken, fix it. [Paste query]`
    
- **Good Prompt:**
    
    > "I am trying to run the following Oracle SQL query, but I am getting an error.
    > 
    > My Query:
    > 
    > [Paste their broken query here]
    > 
    > The Error:
    > 
    > [Paste the Oracle error message, e.g., ORA-00904: 'SPRIDEN_ID': invalid identifier]
    > 
    > Please explain what this error means, why it's happening, and provide the corrected query."
    

### 4. The "Schema Explorer" (For Finding the Right Data)

**Scenario:** Your employee knows the _concept_ they need (e.g., "student address") but has no idea where to find it in Banner.

- **Bad Prompt:** `Where are addresses?`
    
- **Good Prompt:**
    
    > "I am working in an Ellucian Banner database. I need to find the **'Mailing' (MA) address** for students.
    > 
    > I know the main student table is `SATURN.SPRIDEN` and the join key is `SPRIDEN_PIDM`.
    > 
    > What is the primary table for addresses? What table and column stores the address _type_ (e.g., 'MA', 'BI')? How do I join them all together?"
    
- **Finance Example:**
    
    > "What is the difference between the `FIMSMGR.FOBDETL` and `FIMSMGR.FGBDETL` tables in Banner Finance?"
    

### 5. The "Query Refiner" (For Improving Their Code)

**Scenario:** Their query _works_, but it's slow or messy.

- **The "Formatter" Prompt:**
    
    > "Please format this messy Oracle SQL query to be more readable. Use standard indentation, capitalize SQL keywords, and lowercase identifiers."
    > 
    > `[Paste their messy query here]`
    
- **The "Optimization" Prompt:**
    
    > "This query runs, but it's very slow. Can you suggest any ways to make this Oracle query run more efficiently? For example, are the joins in the right order or could I use a better filter?"
    > 
    > `[Paste their slow query here]`
    

Encouraging them to use these structured prompts will teach them to think more clearly about the data they need, and the AI will act as a patient, 24/7 tutor that helps them build confidence.

I hope this training plan and these prompts are a great starting point for your team!

Would you like me to help you find some common Banner tables in the Student, Financial Aid, and Finance modules so they have a "cheat sheet" to start with?