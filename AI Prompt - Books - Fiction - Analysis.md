Please provide a detailed analysis of the **attached text file**, which contains the full text of a fictional book.

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
    
2. The output report **must not** include any reference links, in-text citation markers, page numbers, or blocks like `or`. All information must be presented cleanly.
    
3. **H1 Header:** The first line of content _after_ the YAML block **must** be a level 1 markdown header stating the title and author (e.g., `# [Book Title] - [Author]`).
    
4. **H2 Headers:** The major sections of the report **must** be formatted as level 2 markdown headers (`## I. Dramatis Personae`, `## II. Chapter-by-Chapter Analysis`, and `## III. Holistic Analysis of the Work`).
    

---

## **Required Output Structure:**

Markdown

```
---
title: "[Title-Cased Book Title from Part 1]"
author:
  - [Author from Part 1]
created: [Date from Part 1]
tags:
  - [Tag 1 from Part 1]
  - [Tag 2 from Part 1]
  - [Tag 3 from Part 1]
---

# [Title-Cased Book Title from Part 1] - [Author from Part 1]

## I. Dramatis Personae

Create a list of the major and significant minor characters. For each character, provide a brief (1-2 sentence) description that identifies their role, core motivations, or key relationships.

*Example Format:*
[Character Name]: [Character Description]
[Character Name]: [Character Description]

## II. Chapter-by-Chapter Analysis

For each chapter (or major section) of the book, provide the following:

* **Plot Summary:** A concise summary of the key events, actions, and plot developments that occur within the chapter.
* **Character Development:** An analysis of any new characters introduced, as well as the development, changes, or significant revelations concerning existing characters (their motivations, decisions, or internal conflicts).
* **Themes and Motifs:** Identification of any central themes or recurring motifs that are introduced or reinforced in the chapter.
* **Setting and Atmosphere:** A description of the chapter's setting(s) and the mood or atmosphere it creates (e.g., tense, somber, idyllic).
* **Key Quotes or Passages:** List 1-2 significant quotes from the chapter and briefly explain their importance to the plot, character, or theme.
* **Narrative/Stylistic Elements:** Note any significant narrative techniques used (e.g., flashback, foreshadowing, shift in point-of-view, symbolism).

*Example Format:*
**Chapter 1**
* **Plot Summary:** [Summary of events]
* **Character Development:** [Analysis of character changes]
* **Themes and Motifs:** [Themes introduced or reinforced]
* **Setting and Atmosphere:** [Description of setting and mood]
* **Key Quotes or Passages:**
    1.  "[Quote]" - [Explanation of significance.]
* **Narrative/Stylistic Elements:** [Notes on narrative techniques]

**Chapter 2**
* **Plot Summary:** [Summary of events]
...

## III. Holistic Analysis of the Work

Provide a cohesive, in-depth analysis of the entire novel, organized into the following sections:

### 1. Plot and Structure

* Analyze the overall plot structure (e.g., linear, non-linear, episodic) and the traditional story arc (exposition, rising action, climax, falling action, resolution).
* Discuss the effectiveness of the story's pacing.
* Evaluate the main plot and any significant subplots and how they interconnect.

### 2. Character Analysis

* **Protagonist(s):** Analyze the main character's journey, motivations, internal and external conflicts, and overall character arc.
* **Antagonist(s):** Analyze the primary sources of conflict or opposition, their motivations, and their complexity.
* **Supporting Characters:** Discuss the roles and functions of key supporting characters and their impact on the protagonist and the story.
* **Relationships:** Examine the key character dynamics and relationships.

### 3. Core Themes

* Identify and analyze the 3-5 most prominent themes in the novel (e.g., love, betrayal, power, social class, human nature).
* Provide specific examples and evidence from the text to show how these themes are developed.

### 4. Style, Tone, and Narrative Voice

* **Narrative Perspective:** Analyze the point of view (e.g., first-person, third-person omniscient, third-person limited) and discuss how this choice impacts the reader's experience and understanding.
* **Author's Style:** Describe the author's prose style (e.g., sparse, ornate, journalistic, poetic), diction, and use of literary devices.
* **Tone and Mood:** Describe the overall tone (the author's attitude toward the subject) and mood (the feeling the book evokes in the reader).

### 5. Setting and World-Building

* Analyze the role of the setting (time and place). Is it merely a backdrop, or does it function as a symbolic element or even a "character" in its own right?
* Discuss the atmosphere created by the world-building and its effect on the story.

### 6. Symbolism and Motifs

* Identify and interpret key recurring symbols or motifs (images, objects, or ideas) that appear throughout the novel and explain their contribution to the overall meaning.

### 7. Synthesis and Conclusion

* Provide a concluding summary of the novel's primary message or purpose.
* Offer a brief critical assessment of the book's strengths, weaknesses, and overall literary merit or impact.
```