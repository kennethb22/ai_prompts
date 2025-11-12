### **The Prompt:**

 "Your task is to act as an advanced multimedia editor, using both a Zoom `.vtt` transcript file and its corresponding video recording to create a highly accurate, action-oriented outline in markdown. The video contains software demonstrations, and it is crucial to document the on-screen actions.
 
 Follow these rules in sequence:
 
 1. **Create a Comprehensive, Action-Oriented Transcript:** Your first task is to create a high-fidelity master transcript by cross-referencing the two provided sources. Simultaneously listen to the audio and watch the on-screen actions in the video.
     
     - **Verify Dialogue:** Use the audio to correct any errors in the `.vtt` transcript and fill in any `[inaudible]` sections.
         
     - **Describe On-Screen Actions:** In addition to transcribing the dialogue, you must also describe the key on-screen software demonstrations. When a speaker performs an action on screen (e.g., navigating menus, clicking buttons, typing text, highlighting information), describe it concisely.
         
     - **Format for Clarity:** Use **italicized text in square brackets** for these action descriptions to distinguish them from spoken words. Place them chronologically within the dialogue. The goal is a rich master transcript that combines spoken words with visual context.
         
 2. **Analyze the Conversation Flow:** Next, read through the comprehensive master transcript you just created to identify the main topics, sub-topics, and shifts in conversation.
     
 3. **Create a Title:** The very first line of the final output must be a single Level 1 markdown heading (`#`) for the title of the meeting. You can use a placeholder like `# [Meeting Title]`.
     
 4. **Establish the Outline Structure:** Based on your analysis, all main topics of the meeting should be Level 2 headings (`##`), sub-topics should be Level 3 headings (`###`), and so on.
     
 5. **Clean and Integrate Content:** Place the dialogue and action descriptions from your master transcript under the appropriate headings. As you do, apply the following editing standards:
     
     - **Discard Timestamps:** Remove all timestamps from the final output.
         
     - **Remove Filler Words:** Delete verbal tics and filler words (e.g., 'um,' 'uh,' 'like') from the spoken dialogue.
         
     - **Allow Minimal Summarizing for Clarity:** You may condense highly redundant phrases or lightly rephrase convoluted sentences. **Crucially, you must preserve the speaker's original meaning and not omit any substantive points, information, or demonstrated actions.**
         
 6. **Format and Standardize:**
     
     - Correct any remaining spelling and grammatical errors.
         
     - Fix punctuation for readability.
         
     - **Standardize Speaker Labels:** Use the speaker names from the `.vtt` file and format them consistently in bold (e.g., "**Jane Doe:**").
         
 
 The final output must be a single, continuous markdown document that represents the complete, verified content of the meeting, perfectly organized under a single main title.
 
 **Example Structure:**
 
 Markdown
 
 ```
 # [Title of the Meeting]
 ```

 ## Core Topic 1: Q3 Financial Review
 
 ### Accessing the Report
 
 SARAH CHEN: Okay, so first, I'm going to open the quarterly report from the shared drive.
 
 [Sarah navigates to the 'Reports' folder and double-clicks the file 'Q3_Financials.xlsx'. The spreadsheet loads on screen.]
 
 SARAH CHEN: As you can see, the revenue numbers are in column C. To get the total, I'll just use the SUM function here.
 
 [She clicks into cell C25 and types '=SUM(C2:C24)' and presses Enter. The total appears in the cell.]
 
 JOHN SMITH: That looks great. Can you show us the marketing expenses tab as well?
 
 ```
 
 **Zoom Transcript (.vtt) to Process:**
 [Paste the full content of your Zoom transcript file here]
 ```

 Corresponding Video File:
 
 [Attach the video file here]"