Here is the updated prompt, which restores the full "Pre-Analysis and YAML Property Generation" section from your original request and integrates it with the analysis-free output structure.

---

Please provide a detailed report on the **attached text file**, which contains the full text of a fictional book.

**Part 1: Pre-Analysis and YAML Property Generation**

Before generating the report, you must first analyze the **entire attached text file** to determine the following properties. This information will be used to build the YAML block.

1. **Book Title:** Identify the full title of the book from the text. Convert this title to **title case** (e.g., "the great gatsby" becomes "The Great Gatsby").
    
2. **Author:** Identify the primary author of the book from the text. This value must be formatted as a **YAML list item** in the `author` field (e.g., `- Adam Roberts`).
    
3. **Created Date:** The current date of processing in `yyyy-mm-dd` format.
    
4. **Tags (Exactly 6):**
    
    - Generate the three most relevant **BISAC subject headings** for this content in the fiction/science_fiction hiearchy.
        
    - Generate the three most relevant topical BISAC headings from outside the `fiction/science_fiction`hierarchy (e.g., `science`, `history`, `psychology`, `social_science`, etc.).
        
    - Format the text of _each_ bisac subject heading using the following rules. Apply the rules to the text in the order the rules are given. Each rule should operate on the text created by the prior rule.
        
        1. Convert the text to all lowercase.
            
        2. replace any occurrence of ' & ' with '_and_'.
            
        3. Replace any occurrence of ' / ' with '/'.
            
        4. Replace any occurrence of ', ' with '-'.
            
        5. replace any occurrence of ' ' with '_'.
            
        6. Remove any occurrence of '.' from the text.
            
        7. Remove any occurence of '(' from the text.
            
        8. Remove any occurence of ')' from the text
            

**Part 2: Full Output Generation**

Present the _entire_ output using the exact structure specified below.

**Crucial Formatting Instructions:**

1. You **must** wrap the _entire_ output, starting from the opening `---` of the YAML block to the very end of the summary, in a single **markdown code block** (using ` ```markdown `...` ``` `).
    
2. The output report **must not** include any reference links, in-text citation markers, page numbers, or any form of analysis, interpretation, or thematic discussion. Stick strictly to factual summarization.
    
3. **H1 Header:** The first line of content _after_ the YAML block **must** be a level 1 markdown header stating the title and author (e.g., `# [Book Title] - [Author]`).
    
4. **H2 Headers:** The two major sections of the report **must** be formatted as level 2 markdown headers (`## I. Dramatis Personae` and `## II. Detailed Plot Summary by Chapter`).
    

---

## **Required Output Structure:**

## ` ```markdown `

title: "[Title-Cased Book Title from Part 1]"

author:

- [Author from Part 1]
    
    created: [Date from Part 1]
    
    tags:
    
- [Tag 1 from Part 1]
    
- [Tag 2 from Part 1]
    
- [Tag 3 from Part 1]
    
- [Tag 4 from Part 1]
    
- [Tag 5 from Part 1]
    
- [Tag 6 from Part 1]
    

---

# [Title-Cased Book Title from Part 1] - [Author from Part 1]

## I. Dramatis Personae

Create a list of the major and significant minor characters. For each character, provide a brief (1-2 sentence) description that identifies their role in the story or key relationships.

Example Format:

[Character Name]: [Character Description]

[Character Name]: [Character Description]

## II. Detailed Plot Summary by Chapter

Compose a comprehensive, scene-by-scene summary of the plot, organizing the summary by chapter from beginning to end. This summary must be purely descriptive and objective, detailing the events as they happen.

For each chapter's summary, please make sure to:

- Identify Key Characters: Note which characters are involved in each major scene or plot point.
    
- Describe Scenes and Events: Factually describe the setting, actions, and key events of pivotal moments.
    
- Note Locations: Mention the primary locations where the story unfolds and specify when the action moves between them.
    

Example Format:

Chapter 1: [Objective summary of events, characters, and locations in Chapter 1.]

Chapter 2: [Objective summary of events, characters, and locations in Chapter 2.]

...

```