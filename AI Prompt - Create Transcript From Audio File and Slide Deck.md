Of course. Here is the modified prompt that incorporates the use of an accompanying PDF slide deck. The new instructions are designed to use the PDF as the primary source for the outline structure and as a reference for improving the accuracy of the transcription.

---

### Modified Prompt:

Your task is to act as a multi-step processor, turning an audio file and its accompanying PDF slide deck into a clean, readable, and comprehensive outline using markdown. Do not use canvas, and do not include citations. 

Follow these rules in sequence:

1. **Analyze the PDF Slides for Structure and Title**: Your first task is to analyze the attached PDF file.
    
    - **Create a Title**: Use the title from the first or most prominent slide for the Level 1 markdown heading (`#`). This will be the very first line of the final output.
        
    - **Establish the Outline Structure**: Use the slide deck's structure as the primary scaffold for the document. Main topic slides should become Level 2 headings (`##`), and individual slide titles or key bullet points should become Level 3 (`###`) and Level 4 (`####`) headings. This structure derived from the PDF will be the skeleton you fill in with the spoken content.
        
2. **Transcribe the Audio File**: Create a complete and accurate transcript from the attached audio file.
    
    - Differentiate between speakers where possible (e.g., using 'Speaker 1', 'Speaker 2').
        
    - **Use the PDF for Accuracy**: Refer to the text and terminology in the PDF slides to ensure correct spelling of names, technical terms, acronyms, and specific data points mentioned by the speakers.
        
3. **Clean and Integrate the Dialogue**: Place the dialogue from your transcript under the appropriate headings established in Step 1. As you do, apply the following editing standards:
    
    - **Remove Filler Words**: Delete verbal tics and filler words (e.g., 'um,' 'uh,' 'like,' 'you know,' 'sort of') and stutters unless they are essential to the speaker's meaning.
        
    - **Allow Minimal Summarizing for Clarity**: The goal is a clean, readable record, not a strict word-for-word transcription. You may condense highly redundant phrases or lightly rephrase convoluted sentences to improve clarity. Crucially, you must preserve the speaker's original meaning and not omit any substantive points or information.
        
    - **Incorporate Slide References**: When a speaker directly refers to content on a slide (e.g., "As you can see in this chart..."), add a brief, italicized note to provide context. For example: _[Note: Speaker is referring to the Q3 sales chart on Slide 8.]_
        
4. **Format and Standardize**:
    
    - Correct any remaining spelling and grammatical errors.
        
    - Fix punctuation for readability.
        
    - Standardize all speaker labels to a consistent format, using bold (e.g., **SPEAKER NAME:**).
        

The final output must be a single, continuous markdown document that represents the complete content of the seminar, perfectly organized under a single main title.

---

**Example of Final Output Structure:**

Markdown

```
# [Title of the Seminar From PDF]

## Introduction and Seminar Goals

### Welcoming Remarks
**SPEAKER 1:** [Cleaned and slightly condensed text of Speaker 1's opening statement...]

### Review of the Agenda
**SPEAKER 1:** [Cleaned text describing the agenda...]
**SPEAKER 2:** [Cleaned text of Speaker 2's question about the agenda...]

## Core Topic 1: [Name of the First Major Topic From PDF]

### Initial Presentation of Data
**SPEAKER 3:** [Cleaned and edited text of the data presentation...] *[Note: Speaker is referencing the 'Historical Growth' graph on Slide 5.]*

```

Files to Process:

[Attach the audio file here]

[Attach the PDF file here]