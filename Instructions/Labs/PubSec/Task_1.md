---
task:
    title: 'Task 1: Streamline Data Analysis & Insights with Microsoft 365 Business Chat'
---

# Task 1: Streamline Data Analysis & Insights with Microsoft 365 Business Chat

In this task, you'll use Microsoft 365 Business Chat (BizChat) to uncover actionable insights from your People Matter Survey results. Leveraging Copilot, you’ll identify key departmental trends that can guide informed decision-making and strategic planning.

### Prepare your Document

<div style="background-color: #ffe6e6; padding: 10px; border-left: 5px solid #ff5c5c;"> <strong>Important:</strong> Download the Word version of the 2023 survey results for your respective departments <a href="https://vpsc.vic.gov.au/workforce-data-state-of-the-public-sector/data-sets-and-results/people-matter-survey-2023-results-by-organisation/" target="_blank">here</a> or, if you have a more recent version on hand, feel free to use that as your data source. </div> 

1. In **Word**, open the People Matter Survey document you’d like to use for this task.
1. Ensure your document is saved to OneDrive. If it’s not already saved to OneDrive, select **File** > **Save a Copy** > select **OneDrive** from the top of the list > **Save**.

1. Copy the URL of the document by selecting the **Share** button in the upper-right corner above the ribbon and selecting **Copy Link** from the drop-down menu that appears.

    ![Screenshot showing the Share menu and the Copy Link option highlighted.](../Media/share-menu-with-copy-link.png)
    
<div style="background-color: #e0f7ff; padding: 10px; border-left: 5px solid #0078D4; margin-bottom: 15px;">
    <strong>Note:</strong> Copy the Word document URL to Notepad or store it in the input box below.
</div>
<label for="inputBox" style="font-weight: bold;">Enter your URL here:</label>
<input type="text" id="inputBox" placeholder="Type something..." style="margin-left: 10px; width: 300px;" />
<button onclick="copyText()" style="margin-left: 10px; padding: 5px 10px; background-color: #0078D4; color: white; border: none; border-radius: 4px; cursor: pointer;">
    Copy
</button>
<p id="statusMessage" style="margin-top: 10px; color: #0078D4;"></p>

<script>
    function copyText() {
        const textBox = document.getElementById("inputBox");
        textBox.select();
        textBox.setSelectionRange(0, 99999); // For mobile devices
        navigator.clipboard.writeText(textBox.value)
            .then(() => {
                document.getElementById("statusMessage").innerText = "Text copied to clipboard!";
            })
            .catch(err => {
                document.getElementById("statusMessage").innerText = "Failed to copy text.";
            });
    }
</script>

### Steps:

1. Launch **BizChat** by opening a new Edge browser tab and navigating to <a href="https://m365.cloud.microsoft/chat" target="_blank">m365.cloud.microsoft/chat</a>.

1. Log into your work account if prompted.

1. With **BizChat** open, ensure that the **Work tab** is selected:

    ![Screenshot showing web tab in BizChat.](../Media/work-tab.png)

1. Explore one or more of the prompting techniques below to help guide your research in Business Chat:

    - Single-Shot Prompting
    - Role Prompting (Persona-based Prompting)
    - Chain of Thought Prompting

1. Once you have finished analyzing your survey results, save Copilot's responses to the Word file you created earlier, titled **Copilot Research.docx**, for use in the next task.

## Choosing Your Prompting Technique

Each prompting technique below offers unique benefits depending on the depth of analysis you need. Choose the one that best aligns with your objectives:

- **Single-Shot Prompting** is ideal for a quick overview or broad insights.
- **Role Prompting** adds a personal and professional perspective, helping you analyze data from a specific role's viewpoint.
- **Chain of Thought Prompting** enables a deeper exploration of complex issues through a logical series of connected prompts.

## Single-Shot Prompting

Single-shot prompting uses a single, well-crafted prompt to get a comprehensive response from the AI, ideal when you need a quick summary or broad perspective.

Prompt examples (choose one):

```text
Compare the current People Matter Survey results [Paste link to this year's survey results] with last year's results [Paste link to last year's survey results] to identify the top three areas where employee satisfaction has shown the most improvement. 
```
or

```text
Identify and summarize the top three areas where employees feel most supported and engaged based on the survey results from [Paste link to People Matter Survey results]. Highlight any unique strengths that the department could build on.
```

This approach is more efficient when seeking a broad summary but may not allow the same depth as Chain of Thought prompting.
<strong>Note:</strong> Be sure to copy Copilot's responses into the Word file you created earlier, titled **Copilot Research.docx**, so you can use them in the next task.
<br>
<div style="background-color: #e0f7ff; padding: 10px; border-left: 5px solid #0078D4; margin-top: 15px; margin-bottom: 15px;">
    <strong>Note:</strong> Be sure to copy Copilot's responses into the Word file you created earlier, titled <strong>Copilot Research.docx</strong>, so you can use them in the next task.
</div>



## Role Prompting (Persona-Based Prompting)

Role prompting involves instructing the AI to assume a specific role for tailored insights. Here, participants can take on the role of a senior manager responsible for a particular focus area, such as employee wellbeing, team engagement, or inclusion. This adds a personal perspective, aligning insights with specific responsibilities.

Example prompt:

```text
You are a senior manager responsible for [employee wellbeing]. Using data from [paste link to People Matter Survey], identify key strengths within your focus area where the department’s scores are above the comparator group. Then, propose specific actions or initiatives that could help reinforce these positive outcomes and support the department’s values.
```
<div style="background-color: #e0f7ff; padding: 10px; border-left: 5px solid #0078D4; margin-top: 15px; margin-bottom: 15px;"> <strong>Note:</strong> Replace the bracketed text with your specific focus area as needed. </div>
This technique allows you to develop recommendations that feel aligned with real-world responsibilities.
<br>
<div style="background-color: #e0f7ff; padding: 10px; border-left: 5px solid #0078D4; margin-top: 15px; margin-bottom: 15px;">
    <strong>Note:</strong> Be sure to copy Copilot's responses into the Word file you created earlier, titled <strong>Copilot Research.docx</strong>, so you can use them in the next task.
</div>


## Chain of Thought Prompting

Chain of Thought (CoT) prompting breaks down complex issues into a sequence of steps, enabling detailed analysis through a logical sequence.

Example sequence for exploring employee engagement challenges:

- **Prompt 1:**

    ```text
   Based on the People Matter Survey results, [paste link to People Matter Survey], what are the primary factors contributing to high employee engagement and satisfaction within the department? Highlight any patterns that stand out as strengths.

    ```

- **Prompt 2:**

    ```text
    Considering these engagement strengths, can you suggest strategies or initiatives that could reinforce and build upon these areas, supporting sustained engagement?
    ```

- **Prompt 3:**

    ```text
    Finally, given these strategies, how could the department track continued success in engagement? Identify specific metrics or indicators that would demonstrate progress and recognize ongoing positive outcomes based on future survey results.
    ```

This structured approach helps you explore engagement challenges in a way that builds toward actionable strategies and measurement plans.
<br>
<div style="background-color: #e0f7ff; padding: 10px; border-left: 5px solid #0078D4; margin-top: 15px; margin-bottom: 15px;">
    <strong>Note:</strong> Be sure to copy Copilot's responses into the Word file you created earlier, titled <strong>Copilot Research.docx</strong>, so you can use them in the next task.
</div>


**Next**: [Task 2](https://microsoftlearning.github.io/Microsoft-365-Copilot-Immersion-Experience/Instructions/Labs/PubSec/Task_2.html)

[Back to Index](https://microsoftlearning.github.io/Microsoft-365-Copilot-Immersion-Experience/)
