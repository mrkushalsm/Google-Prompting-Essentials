# Use AI to untangle complex tasks

* Turn abstract ideas into step by step solutions
* Converse with a Gen AI tool
* Create an AI agent
* Build prompt library to help save time and reuse the prompts

# Discover prompt chaining

Prompt chaining guides a generative AI tool through a series of interconnected prompts, adding new layers of context or tasks each step of the way. Eventually, those linked prompts help the tools solve complex problems one step at a time, just like putting together a puzzle.

Have you ever taken time off work and needed to catch up on what you missed? You could prompt a gen AI tool to summarize your emails and any documents you received while you were gone. After reviewing the output, you may wanna prompt it again to focus on time sensitive requests. If the new output reveals an urgent issue, you could prompt the tool again for some solutions on how to handle it and on and on. With this technique, you're not just iterating. Instead, each prompt and response builds on the previous one. You're creating a chain of prompts together in a single sequence.

Let's see prompt chaining in action. We'll use Google AI Studio as it enables us to get access to Gemini models with a long context window.

You just finished writing a novel, huge accomplishment, right? Well, now the other work starts. You need to market and sell it, so you decide to create a marketing plan to promote the book. They claim you can't judge a book by its cover, but it's still important to make a good first impression. First, you'll need a catchy hook or tagline. We can use the prompt framework to generate some options in AI Studio. We upload the manuscript first and here is the prompt as follows,

Task \[Generate three options for a one-sentence summary for this novel manuscript.\] + Format \[The summary should be similar in voice and tone to the manuscript but more catchy engaging.\]

Maybe you want the tagline to focus on a specific theme in your book. We can write a follow up prompt to refine the taglines as follows,

Task \[Create a tagline that is a combination of options in the previous prompt, \] + Context \[with a special focus on the exciting plot twists and mystery of the book.\] + Format \[Find the catchiest and most impactful combination. The tagline should be concise and leave the reader hooked and wanting to read more.\]

Remember, prompt chaining isn't just about adding more context to your prompts. It's about expanding on what the gen AI tool has previously generated. This is a little different from iteration in the prompt framework. Since that focuses on adjusting a given prompt to improve the results. Here you wanna use its output as a building block for more complex requests.

This brings us back to the tagline you generated. It's a great starting point. For the next piece in your prompt chain, you wanna generate a blurb for the back cover of the book with the prompt as follows,

Task \[Create a \] + Format \[five sentence \] + Task \[summary of the entire manuscript below that expands on the one sentence summary.\]

Let's use this output as the first step in your chaining process. With your tagline and blurb set, it's time to think about your book tour, where you promote it in local bookstores, stores that specialize in your book's genre. Let's continue to build the chain and generate a plan based on what we've already told the gen AI tool about your book. Since the model has already analyzed your manuscript and remembers the conversation, thanks to the long context window, just provide the new task (prompt) as follows,

Task \[Generate a six-week promotional plan for a book tour, including what locations I should visit and what channels I should utilize to promote each stop on the tour.\]

You can iterate on any of these prompts, if you're not happy with the options the Gen AI tool provided

That's the power of prompt chaining. All it took was a series of prompts, and we guided the Gemini model and AI Studio to write taglines, summaries, and a plan for the book tour.

# Explore Chain-of-thought and Tree-of-thought prompting

Prompt chaining gives you the chance to explore more complicated ideas and generate interesting responses. You might even uncover some insights you could miss with a single prompt.

## Chain-of-thought prompting

first is chain of thought prompting, or COT prompting asks the gen AI tool to explain its reasoning or to describe step by step how it got to a specific result. It's similar to the way math teachers ask students to explain how they got to an answer. This method can help you understand the gen AI tool's reasoning methods, which can help you make better decisions based on its outputs. For example, you might need help deciding how to balance visiting all six book tour locations with a limited budget or time constraints. You could prompt the gen AI tool for ideas on how to solve this, but this time you include explain your thought process in your initial prompt. That way you can evaluate the logic behind each proposed solution.

## Tree-of-thought prompting

Tree of Thought prompting, or TOT prompting involves asking the tool to explore multiple reasoning paths at once. Like branches growing on a tree, TOT enables the tool to explore multiple solutions to a given problem. It evaluates as it goes, which helps you get the best outcome. It's like going through a maze. Your goal is to get to the end, but you may have to follow a couple of different paths before you get there. This method is particularly helpful when solving abstract problems like developing a plot for the novel sequel with new characters and complex storylines. These techniques can be really useful for creating outlines or drafting small sections of longer documents at work too.

# Simplify multi-step projects with prompt chaining

Some projects are too big to be completed all at once—multi-part work often comes together one step at a time. When working with generative AI tools, some challenges are best overcome by breaking them up into smaller, interconnected tasks, and with prompt chaining, you'll do just that. And taking it step by step also maintains the human-in-the-loop approach, so you can _**evaluate**_ your prompts and results as you continue chaining them together to spot hallucinations.

## Prompt chaining

![Prompt chaining.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Prompt%20chaining.png)

Sometimes, for more complex tasks, it can help to take the output of a gen AI tool and use it as _**context**_ for a new prompt. Connecting prompts is like connecting links in a chain—which is why this process is called prompt chaining.

A great prompt chain is only as strong as the prompts within it, and specificity is the secret to success. Here’s an example: You’re the head of human resources for an advertising agency, and you’ve been tasked with designing an onboarding course for new hires. Creating a program from scratch involves a lot of moving parts, so you’re going to use prompt chaining to keep the workload manageable.

Here’s an example input:

Context \[_I’m the head of human resources for an advertising agency, and I’m designing an onboarding course for new hires._\] + Task \[_Generate an outline specifying the most important parts of an onboarding course for an entry-level hire._\]

And here’s an example of the potential output from that prompt:

_Onboarding Course Outline for Entry-Level Hires at an Advertising Agency_

1. _Introduce agency culture and values_
2. _Summarize duties and responsibilities_
3. _Explain advertising industry fundamentals_
4. _Break down agency tools and technology_
5. _Detail client relationships and communication practices_
6. _Review agency policies and procedures_
7. _Encourage professional development and growth_

Having that output as a foundation then allows the gen AI tool to carry out all sorts of related assignments. For the next part of the prompt chain, you’ll follow up on the second bullet, and expand on the expectations for a new addition to the design department. But keep in mind, some gen AI models don’t automatically retain context from one prompt to the next, and may require you to re-enter the relevant information into the prompt yourself.

Here’s an example input:

_Expand the second bullet point from the attached outline into a paragraph of 100 words, including expectations for their first year._

And here’s what that output might look like:

_As a new entry-level design hire at our ad agency, you will primarily focus on assisting our senior designers and art directors with various projects. Your responsibilities will include: researching design trends and industry best practices, creating concept sketches and mood boards, preparing presentation materials, and assisting with file organization and management. In your first year, we expect you to develop a strong foundation in design principles and software applications. Additionally, you will have the opportunity to contribute to client projects and gradually take on more independent design tasks._

Now that you’ve got a draft which will serve as context for your next prompt, you can continue planning the onboarding course. Keep building the chain by using the paragraph to create an activity to keep new hires attentive and engaged throughout the onboarding process.

Here’s an example input:

_Using the attached text, suggest a three-question quiz to test the reader’s familiarity with the content._

And here’s the output:

_Question 1:_
_What is the primary responsibility of the new design hire?_
_A) Managing the agency's design and copywriting resources_
_B) Creating visually appealing designs for advertising materials_
_C) Writing creative copy for advertisements_

_Question 2:_
_With whom will the new design hire collaborate?_
_A) Clients only_
_B) Copywriters and account managers_
_C) Designers from other agencies_

_Question 3:_
_What is expected of the new design hire in terms of professional development?_
_A) Staying steady in their current skills_
_B) Avoiding industry trends_
_C) Continuously learning and improving their design abilities_

You’d still like to strategize a little further. With the earlier prompt’s paragraph, the tool can also help you design a visual accompaniment.

Here’s an example input:

_Based on the attached text, generate a visually energetic graphic that congratulates the reader on a correct answer, and features images of art supplies and computers._

And the output:

![A cartoon-style graphic featuring a blue banner with the word 'Congratulations' written in bold, playful font. The banner is hanging above a desk that.webp](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/A%20cartoon-style%20graphic%20featuring%20a%20blue%20banner%20with%20the%20word%20'Congratulations'%20written%20in%20bold%2C%20playful%20font.%20The%20banner%20is%20hanging%20above%20a%20desk%20that.webp)

_Note: This image is_ _AI-generated. Results are for illustrative purposes and may vary._

The chain can go on and on; its only limit is your creativity. You can even double back and use chained outputs in different prompts, such as creating onboarding courses for other departments. And if you’re not getting the results you’re searching for, consider how the prompts in your chain might be split up into chains of their own.

## Types of advanced prompt chaining

### Chain-of-thought prompting

When you get the details on how a gen AI tool reaches its conclusions, you can ask smarter questions that lead to more effective outputs. With the chain-of-thought prompting technique, you can ask the tool to retrace its path from input to output, listing out the reasoning behind its response step by step. And if your prompt’s results miss the intended target, chain-of-thought prompting can help you pinpoint the source of the confusion and understand why gen AI makes the decisions it does.

- You can ask the tool to use chain-of-thought prompting with key phrases like “explain your reasoning” or “go step by step.” You may also notice some variety between models, with some gen AI tools requiring more detailed instruction.
	
- With chain-of-thought prompting, you can also single out a particular step in the tool’s process and redirect its decision-making from there. 

![Chain-of-thought prompting.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Chain-of-thought%20prompting.png)

At the top, a box labeled "Prompt input" points with a downward arrow to a box labeled "Reasoning," then another downward arrow points to a second box also labeled "Reasoning," then another to a third box labeled "Reasoning," and then a final arrow to a box labeled "Prompt output."

For example, maybe the suggested paragraph from the onboarding course example isn’t covering everything you need it to, and you want to know how the tool arrived at its recommendation. Returning to your prompt and evaluating the line of reasoning might help you find a new direction. Here’s what a potential input might look like:

_Draft a paragraph of approximately 100 words detailing the major duties and responsibilities of a new entry-level design hire at an ad agency. Explain your reasoning step by step._

And a potential output from that prompt:

_Reasoning:_

_Step 1: Identify Core Responsibilities_

_Step 2: Highlight Essential Skills_

_Step 3: Emphasize Collaboration_

_Step 4: Address Industry Standards_

_Paragraph: As a new entry-level design hire at our ad agency, you will primarily focus on assisting our senior designers and art directors with various projects. Your responsibilities will include: researching design trends and industry best practices, creating concept sketches and mood boards, preparing presentation materials, and assisting with file organization and management. In your first year, we expect you to develop a strong foundation in design principles and software applications. Additionally, you will have the opportunity to contribute to client projects and gradually take on more independent design tasks._

You’d also like the paragraph to mention joining the agency’s community of coworkers, so instructing the tool to incorporate that item specifically could get you back on track.

### Tree-of-thought prompting

There are times when you might not be sure about the most productive way to go from one prompt in a chain to the next. Tree-of-thought prompting can help you compare many possible solutions at once and evaluate which will be most useful. In tree-of-thought prompting, a gen AI tool shows you multiple responses to your prompt, and allows you to choose which ones you’d like to pursue as you explore different possibilities, solutions and troubleshooting. If you land on an unsuccessful output, you can return to the previous step in your chain and explore other options until you’ve reached your desired result.

![Tree-of-thought prompting.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Tree-of-thought%20prompting.png)

The chart begins with a bubble labeled "Prompt" at the top, branching off to three sub-prompts beneath it, with unsuccessful options represented by blue boxes and possibly successful options in green. At center, a green possibly-successful sub-prompt box branches off to four more in the next row down. Those branch off to another row, and in that row, a green box branches down once more to a successful output.

Returning to the earlier example, maybe you’d also like to generate a splashy image for your course’s cover page. With tree-of-thought prompting, you can brainstorm a handful of choices at once and find the best option. Here’s a potential input:

_Imagine three different designers are pitching their design to me._

_All designers will write down one step of their thinking, then share it with the group. Then all experts will go on to the next step, etc. If any expert realizes they're wrong at any point, then they leave._

_The question is: Generate an image that's visually energetic, and features images of art supplies and computers. Show me three suggestions in very different styles from simple to detailed and complex._

And its output:

![Generate an image that's visually energetic, and features images of art supplies and computers. Show me three suggestions in very different styles from simple to detailed and complex.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Generate%20an%20image%20that's%20visually%20energetic%2C%20and%20features%20images%20of%20art%20supplies%20and%20computers.%20Show%20me%20three%20suggestions%20in%20very%20different%20styles%20from%20simple%20to%20detailed%20and%20complex.png)

_Note: These images are_ _AI-generated. Results are for illustrative purposes and may vary_

The gen AI tool’s evaluation reasons that the second image is getting closer to the solution, and will use it to continue building out the tree. For example,

_I really like the 2nd image. Generate 3 more images that are variations of the 2nd image, they should look similar but distinctively identifiable_

And the next resulting output:

![Generate 3 more images that are variations of the 2nd image, they should look similar but distinctively identifiable.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Generate%203%20more%20images%20that%20are%20variations%20of%20the%202nd%20image%2C%20they%20should%20look%20similar%20but%20distinctively%20identifiable.png)

_Note: These images are_ _AI-generated. Results are for illustrative purposes and may vary_

With an entire gallery of pictures to pick from, you can work your way down the tree until you reach a choice that suits your needs, or keep on chaining.

And in some cases, combining tree-of-thought with chain-of-thought can give your prompting the boost it needs. When you need insight on a tool’s reasoning _and_ other options to take within that reasoning, the two techniques can work perfectly together.

Be mindful, however, that advanced prompt chaining may work differently in various gen AI models. Some more advanced AI models, for example, will automatically detect opportunities for chain-of-thought or tree-of-thought reasoning without being specifically instructed to do so. In those situations, experimentation confirms the best results; repeat your prompt with various models and compare their outputs.

Prompt chaining makes difficult projects easier by dividing a large task into simpler, sequential prompts. But remember, this process still needs a human’s critical thinking skills to work best. With your guidance,  prompt chaining can help you evaluate, direct, and correct your prompting process, so you can meet your deadlines with ease.

# Using meta-prompting to improve and generate new prompts

Half the challenge of getting the most out of generative AI tools is knowing how to ask the right question. With meta-prompting, you can ask a gen AI tool _what sort of prompts_ might work for the problem you’re trying to solve. If you get stuck and don’t know what to include in your prompt, recruit the gen AI tool as your assistant prompt designer. Knowing the basics of meta-prompting can help you design better prompts that get you more useful responses.

## Meta-prompting

Meta-prompting techniques are sometimes referred to as “automatic prompt engineering.” And much like the **prompting framework (**_**Task, Context, References, Evaluate, Iterate**_**)** that gives us a strong foundation for designing prompts, meta-prompting comes with its own set of best practices, or power-up strategies. These guide meta-prompts down the most effective paths, and they fall into two main categories:

- **Prompt generation strategies**: To help design a prompt from scratch
- **Prompt refinement strategies**: To fine-tune the prompts you’ve already designed

## Prompt generation strategies

|Strategy|Use case|Example prompt|
|---|---|---|
|**Direct generation**<br><br>Asking a gen AI tool to generate a prompt for you.|You’re a human resources representative heading up a job search, and you’re ready to welcome your office’s newest teammate.|You write: _Generate a prompt that could help write a job offer letter to our top candidates._|
|**Template request**<br><br>Asking a gen AI tool for an outline to organize the contents of your prompts.|You’re the manager of a baseball team, and you’re all going to hit the road for some away games.|You write: _Create a template specifying the most important elements of a gen AI prompt meant to plan travel for a baseball team and its personnel._|
|**Image**<br><br>Using an image as a reference to generate a prompt, or to shape a prompt you’ve already tried.|You’re the owner of a small dog food start-up, and you want your logo to evoke an old oil painting you found online, but describing the painting isn’t working.|You paste the image into the prompt, and write: _Generate a prompt I can use to create the perfect logo for my dog food company that evokes the style of the attached image._|
|**Text**<br><br>Using text as a reference to generate a prompt, or to shape a prompt you’ve already tried.|You’re struggling with an instruction manual for your new computer.|You could upload the manual by attaching a PDF or pasting the text into the prompt window, and write: _Using the text, generate a prompt to begin an explanation of the most important concepts in this manual._|
|**Meta-prompt chaining**<br><br>Breaking the process of drafting a prompt into a series of sub-prompts.|You need a prompt to create a grant proposal, but with all the detail involved, direct generation isn’t working out.|You write: _Generate a prompt that identifies the most important qualities of an intelligent and accessible intro paragraph for a grant proposal._<br><br>From there, you can use the response to construct additional prompts as you build out your proposal.|

## Prompt refinement strategies

|Strategy|Use case|Solution|
|---|---|---|
|**Leveling up**<br><br>Asking the gen AI tool outright to elevate your prompting.|You’re drafting copy for a local auto body shop’s new ad campaign, and your output is missing that fast-and-furious feeling.|From: _I’m working on an ad campaign for a local auto body shop’s sale on tires and windshields. Generate an announcement for the sale._<br><br>To:  _How can I change my initial prompt to produce an ad campaign that uses more engaging language and creates a more memorable impression?_|
|**Remixing**<br><br>Asking the gen AI tool to synthesize multiple attached prompts into a super-prompt including the key context from each one.|You’re working on an intro paragraph to brief potential contractors on a graphic design project, but each prompt’s results leave out some key piece of the job.|You can copy all your prompts and instruct the gen AI tool to combine them into a single prompt that retains the most important parts of each one.|
|**Style swap**<br><br>Dictating the mood and tone for a prompt to bring out a more colorful, vivid final product.|Your initial prompt asking for a description of Irish folk music returned technical results. It’s the right information, but it’s boring! You want to know about the soul of the music, and so your meta-prompt should reflect that.|You can instruct the gen AI tool to rewrite your prompt with an emphasis on emotionality, and to use more expressive, passionate language to communicate the experience of the music.|

With meta-prompting, you can enlist gen AI’s help to design the perfect prompt, or take one you’ve already written to the next level. And with power-up strategies to guide your meta-prompting, you’ll know just what to do the next time you’re having trouble building your prompt into the best it can be. In prompt design, meta-prompting is your roadmap to a successful output.

# Create an AI agent for simulations

One great thing about generative AI tools is that they can create a safe space for me to ask questions. Instead of getting embarrassed or avoiding it, I can get expert advice from a gen AI tool with just a few prompts. With the right prompting techniques, you can transform your gen AI tool into your own team of experts ready to help you take on any challenge. These are called AI agents, and while they don't have secret night vision glasses or rocket powered sports cars, they are incredibly effective at helping you do your job. You can create AI agents for different purposes, depending on what you need, a coding partner, a creative soundboard, or even an accountability buddy to keep you on track with your goals.

Two types of AI agents, with assigned names as Agent Sim and Agent X.

8. Agent Sim:-
	* Simulates scenarios
	* Interviews
	* Roleplays difficult conversations

9. Agent X:-
	* Gives expert feedback on your topic of choice
	* Provides personalized consulting

## Agent Sim

You've been asked to create a training program to help interns improve their interview skills to help them get new positions. Let's go through a series of prompts that will help us create this AI agent in Gemini.

The prompt is as follows,

Persona \[Act as a career development training simulator.\] + Task \[Your task is to help interns master interview skills and conduct conversations with potential managers.\] + Context \[\You need to support the following types of conversations:
* Articulating strengths and skills
* Communicating professionally and confidently
* Discussing future career development goals
] + Task \[Once an intern has picked a conversation topic, provide details about the situation and the interviewer's role. Then act as the interviewer and allow the intern to participate as the employee.\] + Format \[Make sure to guide the conversation in a way that will allow the intern to exercise their interview skills.\]

Continue the roleplay until the intern replies with "JAZZ HANDS". After the intern gives the stop rule "JAZZ HANDS", provide them with key takeaways from the simulation and skills they can work on.

You will probably be interviewed like it was a normal interview, which will help you to prepare for real-life interviews. This is one of the most interesting ways to interact with a gen AI tool because there are so many possibilities. You could even upload a job description and prompt the tool to ask interview questions based on the jobs criteria.

Another example, you can design a prompt to make the AI agent take on different roles you might encounter in the workplace and use it to simulate conversations, meetings, and feedback sessions.

## Agent X

Think of Agent X as your personalized consultant. With the right prompt, you can instruct your agent to be an expert on anything you need. In this example, we need our AI agent to provide expert feedback on a pitch for a potential client. Since this prompt will include a lot of context and information about the potential client, we'll need to use a long context window that allows the generative AI tool to retain and utilize more information leading to better responses. So we'll switch to Google AI Studio.

The campaigning pitch document can be uploaded and the prompt will be as follows,

Persona \[You're my potential client, the VP of Advertising at a world-famous sports car company known for its innovation, performance and engineering excellence.\] + Context \[You're considering hiring a creative agency to develop a new campaign that will attract a younger generation of buyers. You are in a meeting with me, the design director of a creative agency that's pitching a new campaign for your company.\] + Task \[Act as my potential client. When I provide answers, critique the answers. If needed, ask follow-up questions. Continue the conversation until I give the stop rule "BREAK". Then give me a summary of the whole conversation, highlighting ways I can improve my pitch.\] + Reference \[I've included the brief the car company provided me that has all the relevant information for this project. Use the information from this brief to inform your answers.\]

Here, upload any brief given by the client to increase the quality and precision of the criticism given by the model to give a more better experience of how it will happen in real life.

The AI agent will have given a summary of the conversation so far, what's working and what needs improvement and recommendations to strengthen the pitch. Now that the gen AI tool is acting as your client, you can continue asking for feedback on the pitch. Remember to save your prompt so you can return to this conversation after you revise your pitch to help you test more ideas as you hone in on a final version.

You can even create customized versions of Gemini called GEMS. Simply describe what you want your GEM to do and how you want it to respond, and Gemini will take those instructions and help you create a GEM for your specific needs.

# Ideas for AI agents

What if you could turn a generative AI tool into your own team of experts, ready to help you take on any challenge? What if they were speedy, creative, and able to roleplay through all kinds of scenarios to help you with work? Well, there’s no “what if” required—that’s what an AI agent is designed to do. You can create an AI agent to help you with whatever you need, from writing a speech to learning about coding. Here, you’ll learn how to craft your own and start working smarter.  

## Design AI agents

To create an agent, you’ll prompt the gen AI tool as you usually would, following the **prompting framework,** but you’ll focus on _**persona**_ and _**context**_ more than ever. The more detail you include about what you want the AI agent to do, and how you want it to respond, the more effective it will be. 

Here’s how to create an AI agent: 

- Assign the persona you want the gen AI tool to take on. Example: “Act like a successful personal fitness trainer and talented nutritionist.”
	
- Give context and details about the scenario and conversation. Example: “I’m looking to improve my overall fitness and adopt a healthier lifestyle.”
	
- Specify conversation types or the kinds of interaction you want the tool to support, and set some “rules” for the AI agent to follow. Example: “Ask me about my workout routines and meal planning and give me feedback.”
	
- Provide a stop phrase you can use to end the conversation. Example: “When I want the conversation to end, I’ll write, ‘no pain, no gain.’”
	
- Ask the tool to provide takeaways or improvement areas after the conversation ends. Example: “At the end of our conversation, provide a summary of the advice you provided.”

![Design AI Agents.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Design%20AI%20Agents.png)
## AI agent applications

You know what goes into a prompt to create an AI agent, and earlier, you learned about two examples of how to use them: Agent Sim and Agent X. Now, you’ll uncover a couple more situations for AI agents that you might find really useful at work or in your personal life. But just so you know, these are only a few of the ways an AI agent can help you out! Because AI agents simulate conversations and are capable of roleplaying, they’re great for a ton of different scenarios. 

### Practice skills

Have you ever wanted to improve your public speaking skills? Or practice a difficult conversation you’re planning to have? AI agents can help by acting as a digital coach that can give you feedback on a wide range of scenarios, and build your skills in the process. 

Consider this one: you’re a freelance web developer looking to improve your negotiation skills to close more deals, build stronger relationships, and lock in better rates and terms. You can create an AI agent that takes on the persona of a seasoned negotiator and business consultant to help you do just that. To practice a skill with an AI agent, add in a lot of context about the expertise you're honing, and be specific about what it can do to help you achieve your goals. 

Here’s an example:

_I’m a freelance web developer. I want to brush up on my negotiation skills so I can demand higher rates, establish clear project boundaries, and create mutually beneficial relationships with my clients. Take on the persona of a seasoned business consultant with serious expertise in negotiation strategies for freelance web developers. I’d like you to assess and improve my negotiation skills by roleplaying with me through example negotiation scenarios that I might encounter at work and practical exercises, providing industry-specific advice and feedback as I respond. When I want to end the roleplay, I’ll write “I’m finished.” When our conversation is over, provide me with a list of personalized, actionable ways I can improve my negotiation skills._

### Get specific feedback

An AI agent can give you suggestions and recommendations for a particular task. For example, you can create an AI agent that takes on the persona of an editor and helps you change or improve a piece of your writing and provides feedback on your style, format, tone, and more.

Suppose you want to submit a piece of writing to a magazine. Before you submit it, an AI agent can provide critiques and suggestions. To receive feedback on a writing piece, paste your work into your prompt and get specific about your desired outcome, the context, and the persona you want the tool to take on. Note that depending on how much text you want to include in your input (how long of a document you need critiqued), you might need a gen AI tool with a long context window, which allows for the processing of a large amount of information in different formats at once. With that in mind, you could craft a prompt like this:

_I’m submitting a creative writing piece to a literary magazine for a prize. The magazine is known for its fantasy and sci-fi content. The judges are accomplished fantasy writers and will be choosing a winner based on worldbuilding, originality, and technical skill._ 

_Take on the persona of one of the magazine’s judges and critique my piece through the lens of those key areas. Provide suggestions for changes and improvements to further meet the competition criteria._ 

_The stop phrase will be “I’m ready to submit.”_

_Attached are the submission and judging guidelines, a reference piece that won the prize last year, and my story: [upload documents]._

### Learn something new

An AI agent can help you learn more about an unfamiliar topic or even help you learn a whole new skill by taking on the persona of an expert.

Imagine you have Spanish-speaking clients who prefer to communicate in Spanish. You don’t know the language, but you want to learn so you can build more of a rapport and collaborate more closely with them on your projects. An AI agent can help you learn the language by taking on the persona of a Spanish tutor who delivers increasingly difficult lessons, crafts activities and scenarios, chats with you in Spanish, quizzes you, provides feedback based on your responses, and even gives you a little bit of homework. To learn something new, write a prompt that includes a lot of information and detail about what you want the AI agent to do for you.

_I'm trying to learn Spanish to better communicate with my clients who live in Guatemala. Take on the persona of a skilled Spanish tutor and help me learn Spanish. I want you to teach me Spanish by delivering increasingly difficult lessons, crafting educational activities and scenarios, chatting with me in Spanish, and quizzing me. Correct my errors when I respond and call out areas of improvement. Provide feedback in English only. When I want to end the lesson, I'll write "adios." After we finish our conversation, provide me with a personalized list of vocabulary words, conjugations, and tips I should study to become a better Spanish speaker._

### Collaborate on a project

While AI agents are great at helping with broad goals and tasks, they’re also great at honing in on super specific items you need to cross off your to-do list.

Pretend you’re a city planning researcher looking for some additional funding for a new project. If you create an AI agent that takes on the persona of a grant writer and give it information about the grant by providing a link or uploading an image of it, you can have it act as your partner to help you complete the proposal based on the grant’s requirements and evaluation criteria. Provide the context, specify the persona, and add as much detail as possible for what you want to achieve, like this:

_I’m a city planning researcher seeking a grant for a revitalization project. I need assistance crafting a compelling and competitive grant proposal. Take on the persona of an experienced grant writer with expertise in revitalization grants and act as my collaborative partner. Let’s work together on the proposal, brainstorming ideas, refining the language, and ensuring it aligns with the grant’s requirements and evaluation criteria. We’ll focus on developing the following key components:_

- _Project Summary: A concise and engaging overview of the project's purpose, goals, and expected outcomes_
	
- _Project Description: A detailed explanation of the project's activities, methodology, and timeline_
	
- _Budget breakdown: A comprehensive and itemized budget, justifying each expense and demonstrating financial responsibility_

_As I write each section with you, provide insights for how to strengthen them, making sure my work is clear, persuasive, and impactful. The goal is for the proposal to align with the funder’s priorities and showcase the project’s potential for significant impact. When I want to end our session, I’ll write “We’re done.” After our conversation ends, provide a list of takeaways and learnings from our working session that I can consider next time I write a revitalization grant._

_Here is information about the grant and its evaluation criteria: [upload document]._

## More AI agent ideas

These are only a few ways you can utilize gen AI tools to build AI agents to accomplish your goals. For more ideas on how best to use AI agents, check out the following resources:

- **Professor Ethan Mollick’s newsletter,** **One Useful Thing** (link:- https://www.oneusefulthing.org/): While not solely focused on AI agents, this newsletter does feature practical gen AI tips and prompts, as well as research-based insights and thought-provoking discussions on how AI is transforming different areas of our lives.
	
- **Langchain** (link:- https://www.analyticsvidhya.com/blog/2024/07/langchains-agent-framework/): This is a popular open source framework that uses low code or no code to string AI agents together to accomplish tasks. 
	
- **Google Vertex AI Agents** (link:- https://cloud.google.com/dialogflow/vertex/docs): These allow users to design and integrate a conversational user interface into their mobile apps, web applications, devices, bots, interactive voice response systems, and more. They can analyze multiple types of input from customers, including text or audio inputs (like from a phone or voice recording), and respond through text or with synthetic speech. Using Vertex AI Agents, users can provide new and engaging ways for people to interact with their product. 
	
- **Gems** (link:- https://blog.google/products/gemini/google-gems-tips/): These are customizable AI personas you create within Gemini, each with specific skills and knowledge, that are ready to assist you with specific tasks or delve into any topic you’re interested in. A specific feature built into Gemini, they provide a structured way to create and manage AI agents. There are a few premade Gems you can work with, including a learning coach, brainstormer, career guide, writing editor, and coding partner. 

An AI agent can act as your trusty sidekick across all kinds of use cases. They’re not just here to make things fun (though they certainly do that), they’re also powerful tools to help you level up at work and in day-to-day life. Go ahead and give it a try—you might be surprised at what you can accomplish with the help of an AI agent.

# Prompt Versioning

Prompt versioning is a way to keep track of the different versions of your prompts over time. It's a powerful way to capture your most effective prompts, track your progress, and develop your gen AI prompting skills.

You can name your most effective prompts and store them in your personal prompt library for easy access in the future. In fact, some generative AI tools allow you to name and save your prompts right inside the tool.

Imagine you're doing meal prep for your family. You found a set of meals you really like, but you wanna start experimenting with new cuisines. You wouldn't scrap your entire meal plan and start again, right? You'd use what you've already learned about things like preferences, portions, and allergies, and use that as a base to create a new weekly menu for your family.

The same goes for prompt versioning. Once you have a prompt that works, you don't need to reinvent the wheel. You can experiment with different tasks, context, and references to get different results based on what you need. For example, you can develop a reusable prompt for emails. The gen AI tool will draft the email for you, but you can adjust the tone and format based on the audience you're communicating with. You could use a single source of information to create different frequently asked questions, sections dedicated to different types of customers that visit your website. You can tweak the prompt that generated the FAQ for individual consumers and change the persona to make an FAQ for enterprise customers.

Types of prompts we've created:
* Email prompt
* FAQ prompt
* Brainstorming prompt
* Scheduler prompt
* Meeting notes prompt
* Data analysis prompt
* AI agent prompt

Playing and experimenting with prompts is the best way to figure out how to get what you want. And the only way to get there is to get comfortable, explore and learn what path works for you. There's a big community of folks out there that are sharing prompts that have worked for them, so that people can learn from each other's successes, find inspiration and support. Participating in that community is a great way to improve your prompting skills and build a network.