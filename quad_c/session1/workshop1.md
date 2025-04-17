### Workshop 1: Easter Egg Hunt

Topic: Primer on LLMs

Last updated: April 17, 2025

|  |  |
| -------- | ------- |
| **LEARNING OUTCOMES** | Discover GenAI principles, techniques, Quad-C fun facts |
| Model Type | We will use `Azure AI: gpt-4o` unless otherwise indicated |
| Prompts | Appear *in italics*. You can copy/paste them into the LLM GUI |
| Instructions | Run each prompt, save the response, and note the result. <br> We will discuss findings as a team |

We will do the first exercise together

---

1 | **Search**: In slides `01. llm_intro` there are easter eggs with question / answer in the slides. 

Upload the file to ChatGPT and prompt the model to find the easter eggs, returning them as a list.

---

2 | **Adjust Temperature**: How do results change at different temperatures?

Change the settings by clicking slider button at top right of page:  
![image](https://github.com/DrAPT/llm/blob/main/quad_c/session1/chatgpt_settings.png)

What is the current temperature?

You will run each of these prompts at a lower temperature of 0.2 and a higher temperature of 2.0.  
Save each response and note how it changed with temperature.

Prompt 1:  
*What was the first private equity firm in the United States? Answer in 50 words or less.*

Prompt 2:  
  *Who started the personal computer revolution? Answer in 50 words or less.*

Finally, set the temperature to the default (0.8).

---

3 | **Prompt Sensitivity Experiments**: How much does the output change if we change our prompts?  

[EXPERIMENT 1]: Change punctuation  
*What was the first private equity firm in the United States. Answer in 50 words or less.*

**NOTE**: LLMs are designed to use randomness, so it's not uncommon for results to differ even with the same prompt.

Here, we are checking for drastic differences. Early LLMs would produce drastic differences.

[EXPERIMENT 2]: Drop the length requirement  
*What was the first private equity firm in the United States? Make the response as long as necessary.*

---

4 | **Memory**: What does the model remember from our session / between sessions?

*What was the first thing I asked?*

Log out of the site and then log back in.

Rerun the prompt and save the response.

What are your conclusions?

---

5 | **Training Data**: We query the model to understand its training data.  

*What is the timeframe of your training data?*
 
*What is today’s date? How do you know this?*

Change to a different model by clicking this dropdown at the top of the page:  
![image](https://github.com/DrAPT/llm/blob/main/quad_c/session1/chatgpt_model_dropdown.png)

Rerun the prompt below and note any difference.  
*What is today’s date? How do you know this?*


---

6 | **Privacy and Security**: How private are the sessions? Does OpenAI use them to train their models?

*Will this session be used to train models?*  

*How long are my interactions saved?*


