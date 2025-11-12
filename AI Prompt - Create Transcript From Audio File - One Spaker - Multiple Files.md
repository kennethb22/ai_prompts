Your task is to act as an advanced editor, using the provided audio recording(s) to create a highly accurate and well-organized outline in markdown.

Follow these rules in sequence:

1. **Transcribe and Combine Audio:** Your first task is to generate a high-fidelity transcript.
    
    - Check for the attached audio files.
        
    - If there is a single file (e.g., `audio.mp3`), transcribe it.
        
    - If there are multiple sequential files (e.g., `audio_part001.mp3`, `audio_part002.mp3`, etc.), you must transcribe them **in their correct order** and combine them into one single, continuous master transcript.
        
    - This master transcript will be the source for all subsequent steps.
        
2. **Analyze the Lecture Flow:** Next, read through the master transcript you just created to identify the main topics, sub-topics, and shifts in the lecture's content.
    
3. **Create a Title:** The very first line of the final output must be a single Level 1 markdown heading (`#`) for the title of the lecture. You can use a placeholder like `# [Lecture Title]` if one isn't provided.
    
4. **Establish the Outline Structure:** Based on your analysis, all main topics of the lecture should be Level 2 headings (`##`), sub-topics should be Level 3 headings (`###`), and any further nested points should continue with Level 4 headings (`####`), and so on.
    
5. **Clean and Integrate the Dialogue:** Place the transcribed dialogue under the appropriate headings. As you do, apply the following editing standards:
    
    - **Discard Timestamps:** Remove all timestamps from the final output.
        
    - **Remove Filler Words:** Delete verbal tics and filler words (e.g., 'um,' 'uh,' 'like,' 'you know,' 'sort of') and stutters unless they are essential to the speaker's meaning.
        
    - **Allow Minimal Summarizing for Clarity:** The goal is a clean, readable record, not a strict word-for-word transcription. You may condense highly redundant phrases or lightly rephrase convoluted sentences to improve clarity. Crucially, you must preserve the speaker's original meaning and not omit any substantive points or information.
        
6. **Format and Standardize:**
    
    - Correct any spelling and grammatical errors.
        
    - Fix punctuation for readability.
        
    - **Paragraph Formatting:** Format the text as standard paragraphs. Start a new paragraph for logical breaks in thought or topic, similar to how you would format an essay.
        

The final output must be a single, continuous markdown document that represents the complete, transcribed content of the lecture, perfectly organized under a single main title.

**Example Structure:**

Markdown

```
# [Title of the Lecture]

## Introduction and Topic Overview

### Learning Objectives

[Cleaned and slightly condensed text of the opening statement...]

[Continued text, formatted as a new paragraph after a logical break in thought...]

## Core Topic 1: Historical Context

### The Preceding Era

[Cleaned and edited text explaining the first main topic...]

### Key Event Analysis

[Cleaned and edited text detailing the key event...]
```

Audio File(s) to Process:

[Attach the audio file(s) here]