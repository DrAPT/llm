### Workshop 2: Your new role - the Prompt Engineer

Topic: Prompt Engineering

Last updated: April 20, 2025

|  |  |
| -------- | ------- |
| **LEARNING OUTCOMES** | - Craft more effective prompts <br> - Personalize the experience |
| Model Type | We will use `Azure AI: gpt-4o` unless otherwise indicated |
| Prompts | Appear *in italics*. You can copy/paste them into the LLM GUI |
| Instructions | Run each prompt, save the response, and note the result. <br> We will discuss findings as a team |

We will do the first exercise together

---

1 | **Memory**: Storing information that will persist across sessions.

In the Personalization feature, add memory that you think will be useful. 

Run a prompt to test that it works properly.

---

2 | **System Prompt**: Storing information to set the framework. Persists for the current session.

Click the slider at top right and include a system prompt. 

Change the settings by clicking slider button at top right of page:  
![image](https://github.com/DrAPT/llm/blob/main/quad_c/session1/chatgpt_settings.png)

Run a prompt to test that it works properly.

---

3 | **RAG**: Grounding the response in context.

Ask the model to determine the best company in the spreadsheet `fictitious_company_financials.csv` by equal weighting the financial metrics. 

See if you can get the correct answer (**Company 36**) by experimenting with different prompts (e.g., asking it to write and run the code).

---

4 | **Finding a Comfortable Temperature**: Exploring different temperatures for a use case requiring precision.

Write a short memo making an investment case for Company 36 from the uploaded file.

Experiment with different temperatures to find one that you like. 

Note: From the documentation, lower values (0 to 0.3) result in more predictable and consistent output. Higher values (0.7 to 1) can be diverse and creative, but potentially less coherent. 

When you are finished, reset temperature to the default (0.8).

---

5 | **Extracting and Saving Results**: Extract metrics and store in machine-readable format.   

Given your favorite memo, you will ask the model to extract the company metrics and store them in a CSV file.
This will make it easy for you or others to process the data in the future.

You might see a download button like the one circled here:
![image](https://github.com/DrAPT/llm/blob/main/quad_c/session2/download_file.png)

---

6 | **Few-Shot Prompting**: Providing examples to get desired output.

If we have specific requirements in mind, providing one or more examples can help get desired output.

Task: Craft an example using few-shot prompting to get a better answer.

Here is one such example, first using *Zero-Shot Prompting* and then *One-Shot Prompting*:

*Write a memo header*

```
To: [Recipient Name]
From: Steve, Financial Analyst
Date: [Insert Date]
Subject: [Insert Subject]
```

*Write a memo header from John based on this example:*

```
Memo header 1 example:
Date | [Insert Date]
To | [Recipient Name]
From | Steve, Financial Analyst
Subject | [Insert Subject]
```

Output:

```
Date | [Insert Date]
To | [Recipient Name]
From | John, Financial Analyst
Subject | [Insert Subject]
```
---

7 | **Memory**: What does the model remember from our session / between sessions?

Run the prompt:

*What was the first thing I asked?*

Start a new chat by clicking `New Chat` at top left of screen.

Rerun the prompt.

Check the memory under Personalization. Are your saved memories still there?

Is your system prompt still there?

What are your conclusions?

---

8 | **RAG**: Extracting information from a CIM.

For this exercise, you will upload and work with this file: *Project Eagle CIM - Quad-C Management.pdf* 

8a | You will run the prompt below to extract several pieces of information at once:

```
Extract each of these items based on the file. Cite the page of the source information.

- Brands
- EBITDA in 2015
- EBITDA margin in 2015
```

8b | Modify the prompt to extract Brands, EBITDA and EBITDA margin from 2010 through 2015, inclusive.

8c | Feel free to verify results and experiment with other prompts.

---



