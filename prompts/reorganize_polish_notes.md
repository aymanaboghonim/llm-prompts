# 📝 Notes Reorganizer & Polish

## 📋 Prompt Overview
**Purpose:** Transform messy, unstructured notes into professional, well-organized documentation  
**Best Used With:** ChatGPT, Claude, Gemini, or any text-processing AI assistant  
**Difficulty:** Beginner (ready to use immediately)  
**Time Required:** 2-5 minutes depending on content length  

---

## 🎯 Master Prompt

```
## Subject:
Reorganize and Polish Notes for [Platform Name]

## Goal:
Please reorganize, reformat, and polish the following raw notes into a clear, well-structured text document suitable for reading and use on **[Platform Name - e.g., Microsoft Word, Microsoft Teams, Google Docs, a general document]**. The aim is to improve clarity, flow, and presentation without losing any original detail or meaning.

## Input Notes:
--- START OF NOTES ---

[PASTE YOUR RAW NOTES HERE - Make sure to paste the actual notes in this section when using the prompt]

--- END OF NOTES ---

## Core Actions Required:

1.  **Reorganize:**
    *   Structure the content logically using clear headings (use Markdown `#` syntax, e.g., `## Section Title`, `### Subsection Title`), subheadings where appropriate.
    *   Group related pieces of information together under relevant headings.
    *   Ensure a natural and coherent flow between sections and paragraphs.

2.  **Reformat:**
    *   Use standard Markdown formatting for lists (bullet points `*` or `-`, numbered lists `1.`, `2.`).
    *   Ensure consistent paragraph spacing (usually one blank line between paragraphs).
    *   Use **bold text** (`**bold**` or `__bold__`) or *italic text* (`*italic*` or `_italic_`) sparingly for emphasis on key terms or action items if appropriate, but maintain a professional tone.
    *   Format any code snippets appropriately using Markdown code blocks (``` ```).

3.  **Polish Language:**
    *   Improve sentence structure for better flow and readability. Break down overly long or complex sentences if necessary.
    *   Correct minor grammatical errors, typos, or punctuation mistakes.
    *   Replace awkward phrasing with clearer, more standard English where possible, using simple and common vocabulary.
    *   Ensure consistent terminology is used throughout the document for the same concepts.
    *   Maintain a professional and informative tone.

## CRITICAL Constraints (What NOT to Change):

1.  **Maintain ALL Factual Information:**
    *   Do **NOT** alter or omit any facts present in the original notes.
    *   This includes specific names (people, products, features, etc.), dates, technical terms, jargon, numerical data, and specific policy details.

2.  **Preserve Credits & Attributions:**
    *   If the notes mention who said something or attribute information (e.g., "By Eng. X:", "Source: Y"), this attribution **MUST** be accurately kept and clearly associated with the relevant information.

3.  **Maintain Links/URLs:**
    *   All hyperlinks present in the original notes **MUST** be preserved correctly and function if possible within Markdown (e.g., `[Link Text](URL)`).

4.  **DO NOT SUMMARIZE:**
    *   The objective is to reorganize and enhance the clarity of the *existing details*, **NOT** to create a shorter summary or remove information. All original points must be represented.

5.  **Preserve Core Meaning:**
    *   The final polished text must accurately reflect the intended meaning and nuances of the original raw notes. Do not introduce interpretations or opinions not present in the source.

## Output Format:
Provide the final, reorganized, and polished text formatted in clean, standard Markdown suitable for **[Platform Name]**. Ensure headings, lists, paragraphs, and any preserved links are correctly formatted.
```

---

## 📚 Usage Instructions

### **Step-by-Step Guide:**
1. **Copy** the entire master prompt above
2. **Replace** `[Platform Name]` with your target platform (e.g., "Microsoft Teams", "Google Docs", "Markdown document")
3. **Paste** your raw notes in the designated section
4. **Submit** to your AI assistant
5. **Review** and make any final adjustments

### **Platform-Specific Tips:**
- **Microsoft Teams**: Use for meeting notes and project updates
- **Microsoft Word**: Perfect for formal documentation and reports  
- **Google Docs**: Great for collaborative documents and sharing
- **Markdown**: Ideal for GitHub, technical documentation, and blogs
- **Notion**: Excellent for knowledge base and wiki-style content

### **Best Practices:**
- ✅ **Include context** about the meeting/session when possible
- ✅ **Specify formatting preferences** if you have any
- ✅ **Review output** for accuracy before using
- ✅ **Save original notes** as backup

---

## 🎨 Example Interaction

### **Input (Raw Notes):**
```
meeting w/ sarah today - discussed new project timeline
- need to finish backend by dec 15
- frontend team starts jan 2
- testing phase feb 1-14
- launch planned for feb 20
sarah mentioned budget approval needed from john
action items: 
me - create project plan doc
sarah - talk to john about budget
team - review tech stack options
```

### **Expected Output:**
```markdown
# Project Timeline Meeting Summary

## Meeting Details
**Date:** [Today's date]  
**Attendees:** Sarah, [Your name]  
**Topic:** New project timeline discussion

## Key Decisions & Timeline

### Development Schedule
- **Backend Development**: Complete by December 15
- **Frontend Development**: Starts January 2  
- **Testing Phase**: February 1-14
- **Launch Date**: February 20 (planned)

### Budget & Approvals
- Budget approval required from John
- Sarah to handle budget discussion

## Action Items

| Person | Task | Deadline |
|--------|------|----------|
| [Your name] | Create comprehensive project plan document | TBD |
| Sarah | Discuss budget approval with John | TBD |
| Team | Review and finalize tech stack options | TBD |

## Next Steps
- Await budget approval confirmation
- Finalize project documentation
- Confirm tech stack decisions
```

---

## 🔧 Customization Tips

### **For Different Note Types:**
- **Meeting Notes**: Add attendee list and action items sections
- **Course Notes**: Include learning objectives and key concepts
- **Research Notes**: Add sources and citations sections  
- **Project Notes**: Include timeline and deliverables sections

### **For Different Platforms:**
- **Teams Posts**: Keep it concise, use bullet points
- **Word Documents**: Add professional formatting, headers/footers
- **Google Docs**: Optimize for collaboration, use comments
- **Markdown**: Use standard formatting for GitHub compatibility

### **Advanced Options:**
```
Add these specific instructions to the prompt for enhanced results:

"Additionally, please:
- Add a table of contents for longer documents
- Include estimated reading time
- Suggest relevant tags or categories
- Highlight key decisions and action items
- Format any code snippets appropriately"
```

---

## 💡 Pro Tips

- **Batch Processing**: Process multiple note sets by running the prompt multiple times
- **Template Creation**: Save customized versions for recurring meeting types
- **Quality Check**: Always review AI output for accuracy and completeness
- **Version Control**: Keep original notes as reference

---

**Created by:** [Ayman Aboghonim](https://github.com/aymanaboghonim)  
**Part of:** [LLM Prompts Collection](https://github.com/aymanaboghonim/llm-prompts)  
**License:** MIT - Feel free to adapt and share!