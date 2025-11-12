I will provide a raw text copy of an email chain from Gmail. Your task is to clean and reformat this text.

Follow these rules:

1. **Ignore all Gmail UI text:** Skip any lines like 'Conversation opened', 'Skip to content', 'Inbox', etc.
    
2. **Extract the Subject:** Identify the main email subject line. This is typically located after the initial UI text and before the 'Inbox' label or the first sender's name.
    
3. **Parse each message:** Identify each individual email in the chain.
    
4. **Extract Email Parts:** For each email, extract the **Sender**, the **Recipient line** (e.g., 'to Jennifer, me'), the **Date line**, and the **Body**.
    
5. **Clean the Date:** From the extracted date line, remove any relative time text in parentheses, such as `(8 days ago)`. For example, `Oct 28, 2025, 9:11 PM (8 days ago)` should become `Oct 28, 2025, 9:11 PM`.
    
6. **Clean the Body:** Exclude any email signatures from the message body. Signatures often start with `--` (two dashes) or contain contact information, job titles, and company names (like 'Associate Director of Compliance', 'Office of Student Financial Aid', etc.).
    
7. **Format:** Structure the entire output as follows:
    
    - Start with the subject line formatted as a Level 2 Markdown header: `## [Subject Line]`
        
    - Follow with the first email, formatted exactly like this (including the two blank lines after the date):
        
        **From:** [Sender Name]
        
        **To:** [Recipient Line]
        
        **Date:** [Cleaned Date Line]
        
        `[Cleaned Body of Message (no signature)]`
        
8. **Separate:** Use a Markdown horizontal rule (`---`) to separate each subsequent complete email.
    
9. **Enclose:** The entire, final output must be wrapped in a single Markdown code block (`markdown ...` ).
    

Here is the text to process: