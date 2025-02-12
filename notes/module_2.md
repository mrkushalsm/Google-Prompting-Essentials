# Emails with Gen AI

We use the same TCREI framework, as shown below,

Persona \[I am a gym manager\] + Context \[and we have a new gym schedule.\] + Task \[Write an email informing our staff of the new schedule. Highlight the fact that the M/W/F Cardio Blast class changed from 7:00am to 6:00am\] + Format \[Make the email professional and frinedly, and short so that the readers can skim it quickly.\] + Reference \[Here's the new schedule: \<link to the schedule\>\]

Evaluate :- The email is good, can be sent to formal executives in the given above example with square brackets "\[\]".

Iterate :- We shall ask Gen AI to make it more informal and engaging to be sent to gym members as follows, Task \[Now write a concise, consumer-facing email with this same information for our gym members and clients.\] + Context \[Explain that this new schedule will help us better serve them.\] + Format \[Make the tone fun, friendly and motivating to reflect the gym's energy and enthusiasm for our members' health goals. Include a pun about lifting weights.\]

# Prompt with personality: Match gen AI to your writing style

## How gen AI tools approach tone and style

Ever noticed how some AI-generated content can sound a bit robotic, while other times it feels like you’re chatting with a friend or professor? The reason for that is in how gen AI tools handle tone and style. The tools do this in a few different ways, but this reading will focus on just one.

## Contextual understanding

Think of a gen AI chatbot trained on a massive dataset of everyday conversations. When you ask "What's up?" it understands that you're probably asking how it’s doing. It recognizes this common greeting from its training data. Most likely, it will respond appropriately with something like "Not much, how about you?"

That’s thanks to contextual understanding, which allows a gen AI tool to interpret information in a specific setting and use that comprehension to generate an output. This helps the tool:

- Identify audiences.
- Recognize linguistic cues, like a question mark at the end of a sentence.
- Learn language from provided _**references**_.
- Adapt to your preferences.
- Stay consistent in the language it uses.
- Understand inputs and generate outputs in the tone and style you provide it.

![[images/Strategies for tone and style in prompting.png]]

## Strategies for tone and style in prompting

When it comes to matching tone and style, a gen AI tool’s contextual understanding is a key ingredient—but it doesn't make up the whole recipe. That’s where you come in. Here are a few ways to adjust your prompts to help fine-tune tone and style.

### Specify your tone and style

When using the **prompting framework**, enter your desired tone and style within the _**task**_. 

Maybe you have a report you want summarized for a colleague or manager. For example, you could write:

_Summarize this report into three short paragraphs._

![[images/Specify your tone and style.png]]

Instead, specify the tone in your prompt_:_ 

_Summarize this report into three short paragraphs in a friendly, professional, and easy-to-comprehend tone._

![[images/Specify your tone and style 2.png]]

Your inputs will continue to impact your outputs as you _**iterate**_ in the same conversation thread, so being explicit and detailed from the initial setup is important. Bottom line: Don't leave things to interpretation. The more specific you get about the tone you’re after, the better the tool can match your expectations.

For example, specify “witty banter” instead of “humorous,” or “like talking to a friend” instead of “casual.” Here are some other examples of tone you could include in your prompts, with more specific alternatives:

- Academic, or “scholarly and in-depth, like a professor”
- Persuasive, or “compelling and convincing”
- Sarcastic, or “dryly funny, like a wry comedian”
- Inspirational, or “motivating and uplifting”
- Simple, or “like you’re a kindergarten teacher explaining this to their students”

Finally, you might want to add constraints in your first prompt to ensure the language stays on track, such as “avoid using jargon that would be confusing to people who are unfamiliar with the subject.” 

### Provide tone and style references

You can specify your tone and style even further by providing a reference for the gen AI tool to work from. 

Suppose you’re prompting a gen AI tool to help you write a description for a new line of products. You should use specific descriptors of the tone and style you’re interested in based on the audience of the products. 

For example, you might write:

_Help me draft a description for a new line of rock climbing apparel. The target audience is young outdoor enthusiasts and climbers. I want the description to speak to the audience's desire for durable, attractive rock climbing apparel for indoor and outdoor climbing. Keep the language upbeat, informative, and inspiring. Imagine you're talking to a friend who's an avid rock climber._ 

This prompt will work as is, but you could get even more specific about the tone and style you want by providing a reference in your initial prompt rather than waiting to see the output and deciding if it needs one. In that case, you’d just add something like this to the end of your prompt: 

_Consider the tone and style of interviews with history’s most renowned climbers as a reference._

If you’d rather try your luck, you can generate the output without a reference, edit it to your liking, and then use _that_ as a reference for the gen AI tool in your next iteration.

### Iterate on tone and style

If your initial output doesn’t feel quite right, that’s a good time to get more specific by _**iterating**_ on your prompt and adding more details and directions.

Consider the example above. Maybe the message is too bland or the language feels like it won’t appeal to the climbing community. To iterate, you could inject more of the voice you want into the prompt, explain the exact type of apparel you’re selling, add more tone descriptors, and emphasize an emotional connection to the sport of climbing, like this:

_I need this product line description to speak to the heart of young climbers of all kinds. I want to evoke their passion for pushing limits both indoors and out. The shirts, jackets, pants, shorts, tanks, and carabiners enable climbers to express their personal style without sacrificing quality, comfort, or durability, ensuring they look sharp and climb smart. Channel the spirit of climbing legends, and inspire them to reach new heights. Make the language less cheeky and more reverent of the sport._

Remember, **A**lways **B**e **I**terating! Continuing to refine your prompt provides the gen AI tool with more information so you can get closer to a final output that suits your needs.  

## Why prompting for tone and style matters

Whether you’re crafting a professional email, a fun social media post, or a persuasive essay, the right tone and style can make all the difference in how your message is communicated and received. When you specify voice and tone in a prompt, a gen AI tool will use contextual understanding to figure out what you mean, and match outputs to the voice you’re hoping for. If it’s not what you want, you can always provide references and iterate. To get the best results from a gen AI tool, treat it like you’re giving directions to an actor—the clearer your instructions, the better the actor can embody the character you’re envisioning. 

Put briefly, nuance matters! And the more you teach gen AI tools about it, the more helpful they can be. So get specific with your prompts, and narrow in on how you want the outputs to sound. By doing so, you equip gen AI tools to serve you better, whether as an individual or within the unique context of your workplace.

# Generate Ideas with Gen AI

## Plan a launch for the new video game

Persona \[I'm a marketer for a well-known video game producer known for creating immersive story-based online video games./] + Context \[I'm planning the launch of a new medieval fantasy roleplaying game that follows the path of a young protagonist searching for their missing partner. The game's primary audience is young adults. The game is reaching the end stages of development, and I need help creating a timeline before it goes live.\] + Task \[Provide a rough timeline for the year leading up to its launch. Also provide some pre-launch ideas to help generate buzz around the game.\]

### Iterate

More context \[Now provide pre-launch ideas that will appeal to a global audience of young adults.\]

# Build tables and trackers effortlessly

## You need to create a schedule to plan your employee staffing each week and want to prompt Gemini to create a table

Context \[I have 10 employees. Their employee numbers are 1 through 10.\] + Task \[ Create a table that tracks weekly staffing. Create columns for day, name and shift (morning or afternoon).\] + Constraints \[
* There should always be 2 employees scheduled for the morning shift and 2 employees scheduled for the afternoon shift.
* Employees should not be scheduled for a morning shift on the following day after they were scheduled for an afternoon shift.
* Employees should not be scheduled for both morning and afternoon shifts on the same day.
* Every employee should have roughly the same number of total shifts per week.
\]

Gemini gives an option to export it to Google Sheets. We can continue to iterate through it and ask it to make changes based on new data added and add formulas relevant to them or to quickly analyze the information. But remember to avoid entering any sensitive information that you wouldn't want a tool reviewer to have access to. In this case, we used anonymous employee numbers instead of using their specific names. Basically, Always consult your organization's policies regarding sensitive data and Gen AI use.

# Gemini with Google Workspace

## Summarize information and surface insights

With Gemini in **Gmail** (link:- https://support.google.com/mail/answer/14355636), **Docs** (link:- https://support.google.com/docs/answer/14355406), **Slides** (link:- https://support.google.com/docs/answer/14355071), **Sheets** (link:- https://support.google.com/docs/answer/14356410), and **Drive** (link:- https://support.google.com/drive/answer/14356148), you can generate, summarize, and analyze materials to speed up your workflows. Want to quickly get the key points from a lengthy email? Or turn a disorganized collection of data into an easy-to-read table? The side panel feature across those apps helps you tap into the power of gen AI to work faster and smarter directly in your browser tab.

## Improve your writing

Whether it’s a speech, an email, or a research report, sometimes the most difficult thing with writing is getting started. With **Gemini in Docs** (link:- https://support.google.com/docs/answer/14355406), you can generate completely new text or refine existing work so it’s exactly what you need. Maybe you aren’t sure how to start your sales pitch, or your lesson plan runs a bit over 45 minutes. Gemini in Docs can help at all stages of your writing process to kickstart ideas, get words on the page, or revise your work until it’s just right. The best part? You don’t even have to leave your Doc to use it. 

To rewrite your existing work, highlight the text that needs a makeover. Then select the “Help me write” icon to access a few preset options. No copying and pasting your work into a different tool—Gemini in Docs is embedded right there in your first draft to sharpen the tone, add or cut details, and more. 

Now think of how good it feels to find the _exact_ right words when communicating something. **Gemini in Gmail** (link:- https://support.google.com/mail/answer/14199860?hl=en&co=GENIE.Platform%3DAndroid) is your built-in writing assistant, helping you craft new messages or refine existing drafts, so you can write exactly what you mean. Using tech to message people doesn’t have to make things feel impersonal—it can actually enhance how you engage with your team, clients, and others by keeping your message focused, useful, and true to what you want to get across.

Once you’re in an email draft, select the “Help me write ” button and write your prompt. If you’re starting with a draft that you’d like to freshen up, select “Help me write” and choose from the same options.

## Organize your data

**Gemini in Sheets** (link:- https://support.google.com/docs/answer/13951830?hl=en) makes it easier than ever to track and organize spreadsheet data. It offloads the tedious tasks, like filling out cells and formatting tables, so you can get to work building meaningful stories out of your data. Instantly build custom templates, visualize your information, spot trends, and draw conclusions without even leaving your spreadsheet.

## Create original images 

Whether you’re addressing a group of visual learners or just want to keep your audience engaged, well-designed visuals can elevate your work. Luckily, **Gemini in Slides** (link:- https://support.google.com/docs/answer/14355071?hl=en&sjid=18317434446311439557-NA) can help you bring your presentations to life. Generate custom images that reinforce your message, simplify complex information, and capture people’s attention right in your Slide deck.

## Communicate with others

AI can even help make virtual collaboration more seamless. With Gemini in Meet, you can **create custom background images** (link:- https://support.google.com/meet/answer/13954947?sjid=3314721440421800539-NA) for calls; adjust your video **quality** (link:- https://support.google.com/meet/answer/9302964?sjid=3314721440421800539-NA#Studio_look), **lighting** (link:- https://support.google.com/meet/answer/14441737#studio_lighting), and **sound** (link:- https://support.google.com/meet/answer/14441737#studio_sound); and **create translated captions** (link:- https://support.google.com/meet/answer/10964115). You can even **join meetings with multiple laptops** (link:- https://support.google.com/meet/answer/14263133) in the same room without clunky conferencing hardware, so you can work and connect with your team in ways that feel natural, personal, and productive. 

To generate a background image, choose the meeting on your calendar. At the bottom right of your self view, select “Apply visual effects,” then “Generate a background” to add in a custom prompt. You can also select a design style out of the same options we mentioned earlier.

# Capturing meeting notes instantly

Using Google Docs and Gemini, you can make explaining already pre-existing notes easier and more concise, or to your particular liking. Log in to Google Docs and Gemini.

Let's say you want to summarize return policy for your future reference. Add the respective document, and you get an option to summarize this document with access to adding in your own prompt. This should be the following following prompt,

Task \[Summarize this content\] + \[to write a\] + Context \[clear and concise product return policy\] + \[and\] + Format \[outline five steps for customers to take in sequential order\]

Now you have a solid return policy to reference when assisting customers as well as a list of ways customers can begin their returns.

We can also create notes we want from meetings. This can be achieved with Gemini in Meet. First we get the transcript using Gemini in Meets and submit the document to Google Docs and use Gemini there. Then, this should be the following prompt,

Task \[Create meeting minutes for this meeting.\] + Format \[Section the meeting minutes by speaker, and create a bulleted summary key points made by that speaker. If applicable, highlight action items for each speaker.\]

The meeting notes might be useful if formatted in a clearer way with more defined roles and responsibilities from the meeting. Let's iterate in our prompt to achieve that and we'll use the same task,

Task \[Create meeting minutes for this meeting.\] + Format \[Create sections based on key points extracted from the minutes. Attribute each key point to a speaker, and then assign action items to the speaker who is most appropriate to complete them.\]

Through this, if desired output received, the action items will be clearly displayed and we have the most important takeaways from each attendee.

Now you can use these notes to align with your colleagues on a project, share updates to keep stakeholders informed, help your teammates complete their responsibilities and monitor the progress of deliverables.

# Summarize lengthy documents

When you're doing research, writing a report, or investigating market trends, you're bound to come across some especially complex or lengthy materials. Luckily, a generative AI tool can summarize long blocks of texts, extract key insights, and even transform them into new resources. You can also specify your preferred format in your prompt, so you get exactly the type of output you want.

What's a report you've been meaning to read it you haven't had the time to? You wanna summarize it and pull out key insights, but since the report is so long, you'll have to use a Gen AI tool with a long context window.

A long context window allows for the processing of a large amount of information in different formats at once. The long context window also enhances the Gen AI model's ability to understand and generate more coherent and contextually relevant responses to our prompts.

We can use Google AI Studio and use the prompting framework.

We can name our prompt, then we upload the following document. And then this should be the following prompt,

Task \[Summarize this report\] + Format \[in an outline.\] + Format \[Focus only on the most essential points.\]

We get almost what we desire, and if not, we can still iterate through it again and again till we get what we desired. Then, you can name the prompt window to whatever you like.

Let's say you need to use this specific Gen AI tool, but it cannot read the entire lengthy text. Break the text up into chunks, prompt to summarize each chunk, then summarize the summaries.

Getting a summary of what you're reading can help you understand the material in a shorter amount of time. Not only Gen AI tools can summarize lengthy documents, but then can also explain it to you in different ways by incorporating a persona specifying who the audience is and personalize the summary for different people. Eg:- Summarize this for people who don't understand numbers, Summarize this for a small business owner, Summarize using 80s movie quotes.

# Advanced summarization techniques

## Chain of density prompting

With this method, you get increasingly concise summaries and end up with a chain of refined outputs. 

Think of it this way, you're working on the perfect elevator pitch for your company. Your first draft is way too long and includes too many details, but as you refine it, it gets shorter and more direct, all without losing the important points you need to get across. Eventually, you land on the perfect elevator pitch, quick, direct, and effective.

Iterating on our last prompt, we want to update the task and format. This is the following prompt,

Task \[Provide a shorter summary, focusing on the report's, top two to three trends\]

We can get more specific with our prompt to ensure the output not only provides a simpler summary, but is also really targeted to your needs. Let's go shorter. We'll ask for a single sentence with the following prompt,

Task \[Condense the summary\] + Format \[into a single sentence\] + Context \[and highlighting the most dominant trend.\]

We kept asking it to refine further and we were direct and specific about the desired output. We can repeat this process until we generate the most useful and helpful outputs for the task. We can even get ahead of these extra iteration steps and ask that the gen AI tool provides multiple increasingly short iterations in the initial prompt.

 Iteration helps us check for hallucinations as we go from something super detailed to an output that's more direct and to the point. It also helps us stay informed about what information is being taken out as the outputs get shorter, hence not getting the shortest output right away.

Chain of density prompting also works in the other direction. If the output is too short, we can also prompt to increase the length and add more detail.

## Adjusting the prompting framework

There are a few best practices to keep in mind when guiding a gen AI tool to summarize information, like lengthy documents. Here’s how to adjust the different parts of the **prompting framework**:

- **Task:** Specify which content you want the gen AI tool to summarize, such as a portion of a document or a specific sub topic. Include the desired _**format**_ of the summary, such as bullet points, as well as the length and tone of the summary you want. You also want to add a _**persona**_, such as asking for the output to fit a 9th grade reading level.
	
- **Context:** You may need to add additional context about what the summary is for or why you’re creating it. This helps a gen AI tool anchor its response to something tangible. 
	
- **References:** If there’s a summary that matches what you’re looking for, consider adding both the summary and the document it’s summarizing as a reference so the tool knows what approach to take.
	
- **Evaluate:** When you’re inputting large amounts of text or data, there’s a lot of information for a gen AI tool to process. This can increase the chance of misinterpretations, irrelevant chains of thought, or even hallucinations. To ensure the output is helpful and accurate, evaluate it based on the task you input. You can also cross-reference the output or run it by a subject matter expert if you have access to one. 
	
- **Iterate:** If a gen AI tool doesn’t deliver a useful summary, you’ll need to iterate by asking it to adjust the format, the length, or specific details about the output that aren’t working for you. Keep iterating until you receive a summary that serves your purpose.

## Long context 101

Gen AI tools are constantly improving, and some are now capable of handling much larger pieces of text and data in a single input. This is made possible by an increase in the token limits of gen AI tools and the use of long context windows. 

### AI model and token limit

Tokens are the fundamental building blocks of text that AI models use to process and understand language. Tokens can be as small as a single character, a part of a word, or even multiple words. When you give a gen AI tool a prompt, it breaks it down into tokens. The longer the prompt, the more tokens it needs to generate an output for it. If you were building a house out of bricks, you could think of each individual brick as a token in the building process. 

Early AI models could only process up to several thousand tokens at once, but now some models can process _millions_. It’s important to understand which AI model you’re using and its token limit since it varies from model to model. As developers find new ways to increase token limits, gen AI tools become more and more capable of handling larger quantities of data in a single prompt.

### Long context windows

**Long context windows** (link:- https://blog.google/technology/ai/long-context-window-ai-models/#:~:text=Previously%2C%20Gemini%20could%20process%20up,can%20take%20in%20and%20process.) allow gen AI tools to process large amounts of information, or larger amounts of tokens, in different formats at once. Using a long context window means you can share much more context and background information in your input, which allows you to complete more complex tasks that include a lot of nuanced details—like creating a multi-part marketing campaign or a thorough business plan.

With more context and detailed information about your task, a gen AI tool can then understand and generate more comprehensive, personalized, and relevant responses. For example, with a long context window, a gen AI tool can process a lengthy PDF report with dozens of pages, graphs, and illustrations in a single input, and then generate a summary based on what you need. This saves you time by eliminating the need to manually break down text or information into smaller chunks when designing your prompt. 

Have you ever forgotten something, like what you ordered to eat last week or someone’s name in the middle of a conversation? Recalling past details can be tricky for gen AI tools, too. Long context windows help solve this by acting as a working memory for gen AI tools so they can remember what you shared earlier in the same conversation thread. Think of it like talking with someone who is already familiar with a problem you’re trying to solve versus explaining your situation to a stranger who has no context. 

Just a word of caution: Most gen AI tools will only remember what you put in a long context window in the same conversation thread or prompt chain (we’ll learn about **prompt chaining** (link:- https://www.coursera.org/learn/google-prompting-essentials/supplement/IEkjN/simplify-multi-step-projects-with-prompt-chaining TODO CHECK HERE) in more detail later in the course). In other words, if you close the window and re-open it after entering your screenplay, for example, the tool won’t recall, and you’ll need to enter your materials again before the tool can provide outputs related to it.