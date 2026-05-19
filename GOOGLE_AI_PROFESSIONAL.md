
## AI Fundamentals

### Module 1 - Collaborate with AI

- First video is an introduction to the course
- It's stressed that you want to develop a collaborative mindset with AI
- Three ways to collaborate:
	1. Helping you understand information
	2. Creating brand new things
	3. Refine your own work



### Module 2 - Practise using AI

- first video is a survey
- Some more info regarding how lab works

**Brainstorming ideas with Gemini**

The first lab of the course which showcases how one could collaborate with AI to create the beginning of a presentation. The actual prompts with assignment text:

Lab tasks:
Step 1: Brainstorm presentation structures
Click the “New chat” button on the left side menu to start a new chat with Gemini. Then, paste the prompt below and replace the text in [brackets] with your own details.

I'm preparing a presentation on [your topic, e.g. AI]. My primary goal is to [your main objective, e.g. show how AI can be useful at work]. Help me brainstorm [number] compelling ways to structure my presentation for an audience of [your specific audience, e.g. professionals].

Step 2: Find a "hook" statistic
In the same chat with Gemini, paste the prompt below and replace the text in [brackets] with your own details.

I like [your favorite option from step 1, e.g. the value of AI at work]. Now I need a powerful hook for my introduction. What's a surprising statistic about [your topic from step 1, e.g. the value of AI at work]?

Step 3: Draft your first paragraph
In the same chat with Gemini, paste the prompt below and replace the text in [brackets] with your own details.

I like [your favorite hook from the previous step]. Using that, draft an opening paragraph for my presentation. Generate [number] options that range in tone from [one tone, e.g. casual] to [another tone, e.g. professional].


### Module 3 - Learn how AI works

- AI models: computer programs that are trained on tons of data like articles, images etc.. The model finds patterns in the data and then are able to apply those patterns to new situations
- Training: the model learns are being fed data that it learns on.
- Generative AI: AI's that are able to create new content
- Multimodel: models that are able to udnerstand more than just text
- AI agents: basically genAI x able to use tools

#### Fundamentals of Machine Learning

AI and ML are closely related but there are some key differences:

- AI referes to a broad set of tools that can complete tasks mimicking human int. 
- AI models are trained with ML

**Approached to ML**

Three common ways to use ML to develop AI

1. Supervised learning

Train AI from a large dataset labeled by humans. Often used when there is a specific know output in mind. Labeled picture of zebras and horses. Use AI to identify on a new picture if it's a z or h.

2. Unsupervised learning

Train AI from a large dataset not labeled by humans. Used when there isn't a specific outcome in mind. Feed the AI unlabeled pictures of zebras and horses. The AI learn to differentiate on it's own

3. Reinforcement learning

Trains the AI through a trial-and-error process that is guided by a reward system

"Win a match in Starcraft" or give the AI pictures where certain contains images of zebras. If the model guesses correcly => reward. If wrong => penalty

Many AI model uses a combination of these 3 approaches.

#### Understanding AI limitations 

- the output of a AI model is directly related to it's training data. Bias in training => bias in output
- To avoid:
	- be specific of the output you want. Add lots of context
	- use follow-up prompts to iron out inaccuracy. Ask the model to correct the biased output
- Gradually, a model will probably give worse fashion advice

 
 - The AI model is the engine
 - the AI app is the driver seat

### Module 4 - Design great prompts

- It works the best when given clear instructions - if you ask your coworker to buy you a sandwich it could be 50 different sandwiches 
- general structure of a prompt:
	- persona
	- task
	- format
	- context

- Follow the three C's when writing your prompt:
	1. Be concise: simple prompt. Avoid long an complex ones.
	2. Be clear: "make this better" is to vague. Give clear and specific directions instead
	3. Be consistent: if you use the word spreadsheet. Continue with that word in the rest of the chat

**Apply the prompting framework in Gemini lab**

Lab tasks:
Step 1: Define your initial task
Click the “New chat” button to start a new chat with Gemini. Then, paste the prompt below and replace the text in [brackets] with your own details.

I want to learn a new skill to [your high-level goal, e.g. advance my career, get a new job], but I'm not sure where to start. Help me brainstorm some ideas.

Review Gemini’s suggestions. You will refine these results in the next step.

Step 2: Use meta-prompting to refine the results
In the same chat with Gemini, paste the prompt below to ask Gemini how to improve its own suggestions.

What questions can I answer to help you tailor your suggestions?

Read Gemini's questions. You will use them to provide more context in the next step.

Step 3: Add context about yourself
In the same chat with Gemini, answer the questions from the previous step to provide additional context. Paste the prompt below and replace the text in [brackets] with your own details.

Here are some more details about me:

- [Answer 1]

- [Answer 2]

- [Answer 3]

- [Answer 4]

Based on this information, suggest [number, e.g. three] skills that would be relevant to me.

Step 4: Define a persona
In the same chat, ask Gemini to adopt a specific persona to help analyze the previous suggestions. Paste the prompt below and replace the text in [brackets].

Now, act as a [specific persona, e.g. career coach or hiring manager]. Which of the skills above would you recommend I focus on first? Explain your reasoning.

Step 5: Decide on next steps
In the same chat with Gemini, paste the prompt below and replace the text in [brackets].

Suggest [number, e.g. three] actions I can take [timeframe, e.g. this week] to start learning that skill. Format this as a [output format, e.g. table] with [format details, e.g. column names].

Next steps: 
Think about what next steps you’d like to take based on Gemini’s output. Also, consider how you can use the prompting framework in other ways.

When you are satisfied with your outputs from this lab, you can close this page and return to the main screen of this course.

**Prompting tip**

At the end of the prompt after all context and so forth, add:

"please aks me any follow-up or clarifying questions before you continue doing work"

### Module 5 - Level up your prompts

You've already learned the prompting framework (persona, task, context, and format) for writing a good prompt.

Next up are two advanced techniques that can help you with more complex tasks:

#### Powerful prompt phrases: think of this as leveling up your communication with every prompt you write

Certain phrases can be more effective

Give AI a process to follow:
- think step-by-step
- first x, second y, ...

Define the audience and tone:
- write this for an audience of x
- the tone shuld be x

set hard constraints
- write a one paragraph summary
- focus exclusively on X and don't mention topic Y

Request a critique
- Critique this text from the perspective of a X
- play the devil's advocate. What is the strongest counterargument to this?

Generate alternatives
- give me 3 different versions of this
- what's an alternative approach to solving this problem?

Deepen or expand on the initial output:
- Elaborate on point 2
- provide more detail and specific examples for the section about X

#### Prompt chaining: break down a big task that is to big for a single prompt

It works like a factory assembly line: The output from one prompt is used as the inout for the next.

Example: you are planning a vaction in Paris.

Prompt 1: I'm going to paris for 3 days. I like art, historical sites, and parks. Suggest a few well-know places I could visit on my trip.

Prompt 2: Using those locations, create a logical day-by-day itinerary that minimizes travel time

Prompt 3: For each day of the itinerary, suggest a few restaurants located near the suggested locations

#### Practice prompt chaining in Gemini

Lab tasks:
Step 1: Brainstorm options
Click the “New chat” button to start a new chat with Gemini. Then, paste the prompt below and replace the text in [brackets] with your own details.

I want to expand my [company description, e.g. painting company]'s service offerings. Act as my business advisor and list 3 complementary services we could provide. Keep in mind: [context and constraints, e.g. we have a team of 4 painters and tight office space].

Read Gemini’s response. The next steps will build on this foundation.

Step 2: Evaluate the options
In the same chat with Gemini, ask questions to evaluate the options Gemini provided in the previous step. You can ask about specific criteria or potential challenges. For example:

Which of these can we launch within 6 months?

Read Gemini’s response. The next steps will build on this foundation.

Step 3: Create an action plan
In the same chat with Gemini, paste the prompt below and replace the text in [brackets] with your own details.

If I want to move forward with [1 option from Gemini’s response in the previous step], what tasks should I complete this week?

Use Gemini's response to build your task list for the week.

**A hack for giving Gemini context in a new windows**

Ask the model to summarize everything you talked about -> go into a new chat, say you already working on an something in an old chat and paste summary. Re-upload any attachements and go

### Module 6 - Use AI responsibly




## Notes

2026-05-19
- a simple framework for writing good prompts: persona, task, format, context which I think is simple but very useful
- Nothing super-surprising yet
- It's still unclear to me when I shuld apply all the techniques I have learned. Hopefully it will be clear after next session

These tips can be used right away:

- It works the best when given clear instructions - if you ask your coworker to buy you a sandwich it could be 50 different sandwiches 
- general structure of a prompt:
	- persona
	- task
	- format
	- context


Certain phrases can be more effective

Give AI a process to follow:
- think step-by-step
- first x, second y, ...

Define the audience and tone:
- write this for an audience of x
- the tone shuld be x

set hard constraints
- write a one paragraph summary
- focus exclusively on X and don't mention topic Y

Request a critique
- Critique this text from the perspective of a X
- play the devil's advocate. What is the strongest counterargument to this?

Generate alternatives
- give me 3 different versions of this
- what's an alternative approach to solving this problem?

Deepen or expand on the initial output:
- Elaborate on point 2
- provide more detail and specific examples for the section about X