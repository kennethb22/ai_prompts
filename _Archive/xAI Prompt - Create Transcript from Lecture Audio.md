Here is the modified prompt, which now relies only on an audio file as the source:

---

Your task is to act as an advanced editor, using a single audio recording to create a highly accurate and well-organized outline in markdown. 

Follow these rules in sequence:

1. **Transcribe the Audio and Identify Speakers:** Your first task is to listen carefully to the attached audio file and generate a high-fidelity transcript. As you transcribe, identify and distinguish between the different speakers. If their names are mentioned in the audio, use them. Otherwise, use generic but consiste nt labels (e.g., 'Speaker 1', 'Speaker 2'). The result of this step is a master transcript which will be the source for all subsequent steps.
    
2. **Analyze the Conversation Flow:** Next, read through the master transcript you just created to identify the main topics, sub-topics, and shifts in conversation.
    
3. **Create a Title:** The very first line of the final output must be a single Level 1 markdown heading (`#`) for the title of the meeting. You can use a placeholder like `# [Meeting Title]` if one isn't provided.
    
4. **Establish the Outline Structure:** Based on your analysis, all main topics of the meeting should be Level 2 headings (`##`), sub-topics should be Level 3 headings (`###`), and any further nested points should continue with Level 4 headings (`####`), and so on.
    
5. **Clean and Integrate the Dialogue:** Place the transcribed dialogue under the appropriate headings. As you do, apply the following editing standards:
    
    - **Discard Timestamps:** Remove all timestamps from the final output.
        
    - **Remove Filler Words:** Delete verbal tics and filler words (e.g., 'um,' 'uh,' 'like,' 'you know,' 'sort of') and stutters unless they are essential to the speaker's meaning.
        
    - **Allow Minimal Summarizing for Clarity:** The goal is a clean, readable record, not a strict word-for-word transcription. You may condense highly redundant phrases or lightly rephrase convoluted sentences to improve clarity. Crucially, you must preserve the speaker's original meaning and not omit any substantive points or information.
        
6. **Format and Standardize:**
    
    - Correct any spelling and grammatical errors.
        
    - Fix punctuation for readability.
        
    - **Standardize Speaker Labels:** Use the speaker names or labels you identified during transcription (e.g., **Jane Doe:** or **Speaker 1:**) and format them consistently in bold.
        
    - **Speaker Change Formatting:** Start a new paragraph each time the speaker changes. Ensure the speaker label is at the beginning of the new paragraph, followed by their dialogue.
        

The final output must be a single, continuous markdown document that represents the complete, transcribed content of the meeting, perfectly organized under a single main title.

**Example Structure:**

Markdown

```
# [Title of the Meeting]

## Introduction and Goals

### Welcoming Remarks

**Speaker 1:** [Cleaned and slightly condensed text of the opening statement...]

### Review of the Agenda

**Speaker 1:** [Cleaned text describing the agenda...]

**Speaker 2:** [Cleaned text of a question about the agenda...]

## Core Topic 1: Q3 Financial Review

### Initial Presentation of Data

**Speaker 3:** [Cleaned and edited text of the data presentation...]
```

Audio File to Process:

[Attach the audio file here]