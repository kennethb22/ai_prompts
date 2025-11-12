"Your task is to act as an advanced editor, using both a Zoom `.vtt` transcript file and its corresponding audio recording to create a highly accurate and well-organized outline in markdown. The audio recording of the meeting is in two parts. The first part meeting_audio_00.m4a and the corresponding vtt file is meeting_transcript_00.vtt. The second part meeting_audio_01.m4a and the corresponding vtt file is meeting_transcript_01.vtt. You are to create a transcript that includes both parts of the meeting. 

Follow these rules in sequence:

1. **Verify and Correct the Transcript:** Your first task is to cross-reference the two provided sources. Use the `.vtt` file as a guide for speaker names and the general flow. Listen carefully to the attached audio file to verify the text. Correct any transcription errors, fill in words marked as `[inaudible]` if you can discern them from the audio, and ensure the dialogue in the transcript accurately reflects what was actually said. The result of this step is a high-fidelity, corrected master transcript which will be the source for all subsequent steps.
    
2. **Analyze the Conversation Flow:** Next, read through the corrected master transcript you just created to identify the main topics, sub-topics, and shifts in conversation.
    
3. **Create a Title:** The very first line of the final output must be a single Level 1 markdown heading (`#`) for the title of the meeting. You can use a placeholder like `# [Meeting Title]` if one isn't provided.
    
4. **Establish the Outline Structure:** Based on your analysis, all main topics of the meeting should be Level 2 headings (`##`), sub-topics should be Level 3 headings (`###`), and any further nested points should continue with Level 4 headings (`####`), and so on.
    
5. **Clean and Integrate the Dialogue:** Place the corrected dialogue under the appropriate headings. As you do, apply the following editing standards:
    
    - **Discard Timestamps:** Remove all timestamps from the final output.
        
    - **Remove Filler Words:** Delete verbal tics and filler words (e.g., 'um,' 'uh,' 'like,' 'you know,' 'sort of') and stutters unless they are essential to the speaker's meaning.
        
    - **Allow Minimal Summarizing for Clarity:** The goal is a clean, readable record, not a strict word-for-word transcription. You may condense highly redundant phrases or lightly rephrase convoluted sentences to improve clarity. **Crucially, you must preserve the speaker's original meaning and not omit any substantive points or information.**
        
6. **Format and Standardize:**
    
    - Correct any remaining spelling and grammatical errors.
        
    - Fix punctuation for readability.
        
    - **Standardize Speaker Labels:** Use the speaker names from the `.vtt` file and format them consistently in bold (e.g., "**Jane Doe:**").
        
    - **Speaker Change Formatting:** Start a **new paragraph** each time the speaker changes. Ensure the speaker label is at the beginning of the new paragraph, followed by their dialogue.
        

The final output must be a single, continuous markdown document that represents the complete, verified content of the meeting, perfectly organized under a single main title.

**Example Structure:**

Markdown

```
# [Title of the Meeting]

## Introduction and Goals

### Welcoming Remarks

**JANE DOE:** [Cleaned and slightly condensed text of Jane's opening statement...]

### Review of the Agenda

**JANE DOE:** [Cleaned text describing the agenda...]

**JOHN SMITH:** [Cleaned text of John's question about the agenda...]

## Core Topic 1: Q3 Financial Review

### Initial Presentation of Data

**SARAH CHEN:** [Cleaned and edited text of the data presentation...]
```

**Zoom Transcript (.vtt) to Process:**

```
[Paste the full content of your Zoom transcript file here]
```

**Corresponding Audio File:**

[Attach the audio file here]"