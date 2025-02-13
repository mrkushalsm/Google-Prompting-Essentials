# Basic Framework for generating good prompts

Simple Framework **TCREI** (Thoughtfully Create Really Excellent Inputs),
* T - Task
* C - Context
* R - References
* E - Evaluate
* I - Iterate

![TCERI](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/TCREI.png)

Minimally need only Task and Context.

The prompting framework sets you up to give gen AI tools the information they need to generate useful outputs—and it’s designed to apply across all kinds of tools and models. So whatever your gen AI tool of choice, make sure you specify your task, provide context and references, evaluate your outputs, and iterate your inputs.
## Task

Crafting a great prompt starts by describing the task you want the tool to help you with. The task is the foundation of any prompt. It’s what you’re asking the gen AI tool to do for you. Adding a task to your prompt is like writing a sentence asking someone to do something for you: 

_Write a list._

_Draft a speech._

_Create an image._

These are all tasks that a gen AI tool can help with.

When you’re writing a task, you need to be clear and specific about what you want. If you write a task with vague instructions, it can result in an output that’s irrelevant or incorrect. 

To avoid that, give your tasks some specific details. That includes providing a _**persona**_ and a _**format**_:-
- Persona
- Format

Here’s an example of a prompt that includes task, persona, and format: 

_You’re a movie critic that specializes in Italian film. Create a table that contains the greatest Italian films of the 1970s, and separate them into genres like thrillers, dramas, and comedies. Provide a 100-word summary of each movie as well as details about the production including director and release year._
### Persona

Refers to what expertise you want the gen AI tool to draw from. For example, a professional speech writer or a marketing executive with 15 years of experience. You can also ask it to create output for a specific audience, a customer or even your manager.

Think of a persona as the expertise you want the gen AI tool to draw from. You can ask the tool to take on the perspective of a science expert or an industry analyst, or ask it to create an output geared towards a specific audience, like your manager or team.
### Format

Refers to how you want the output to appear, whether that's a bulleted list, short sentences, or a table.

The format is what you want the output to look like. Want a bulleted list? Or maybe a table so you can compare results side-by-side? Include those details in your task.
## Context

Refers to the necessary details to help the gen AI tool understand what you need from it. There are two types of context,

* Vague = Give me some ideas for a birthday present **under $30**.
	
* Precise = Give me five ideas for a birthday present. **My budget is $30. The gift is for a 29-year-old who loves winter sports and has recently switched from snowboarding to skiing.

When it comes to prompting, oversharing can be good. The more relevant details you include, the better your output will be. Providing lots of background information—like your goals, the reason for the task, or what you’ve tried before—rounds out the model's understanding of what you're looking for. These details are called context, and they’re a vital part of creating great prompts.

For example, you could write: 

_How was DNA discovered?_

Instead, write a prompt that includes detailed context or background information:  

_You’re a science expert developing a new curriculum at a local college. Tell me in a couple of engaging paragraphs how DNA was discovered and what kind of impact it had on the world. Write it in a way that people unfamiliar with science would understand. You have gotten feedback from students that they found this course dry and unintelligible before, so you want to make sure that the explanation grabs the students' attention and makes a good first impression._

Context has the potential to be the longest piece of a prompt. As you add more of it to your prompts, you may want to consider using delimiters, which not only act as extra pieces of context, but help differentiate parts of your inputs. Delimiters are special symbols that keep prompts tidy and increase the likelihood of generating a useful output. Think of them like labels or guard rails that tell the tool, "This is the task," "This is the context," and so on.

Some popular delimiters include:

- **Triple quotes (""")**: These create a distinction between the different elements of the prompt, like your task and context. They’re useful for when you want to clearly separate text within a prompt to signify different meanings, purposes, or other distinguishers.  For example:
    
    _Write a social media post based on the following announcement:_
    
    _""" Our annual company picnic will be held on Saturday, June 24th at Bicentennial Park. We'll have food trucks, lawn games, and live music from 11am to 4pm. All employees and their families are welcome to attend. """_
    
- **XML tags**: These are like labels that mark different sections of more complex prompts. For example, add “<task>” to make it super clear where your task begins and “</task>" to indicate where it ends.
- **Markdown tags**: These are symbols you can use in prompts to add formatting. For example, if you were to use a gen AI tool to copy-edit your work, you could surround text with “\_” to italicize it or “\*\*” to bold it. This preserves your formatting as you move it into a gen AI tool, which generally uses plain, or unformatted text.
## References

Referring to the previous example, add examples of birthday presents you've given in the past as references, the gen AI tool can give you a more useful output. There are three types,
* Few shot prompting = Multiple references
* Single-shot prompting = One reference
* Zero-shot prompting = No references

There aren't always going to be clear references of what you need, especially if you're working on something more abstract or searching for ideas and inspiration.

References are examples or any additional resources that resemble what you want the gen AI tool to produce. Including references in a prompt is like showing your hairstylist an image of someone with the new haircut you’d like to try.

Depending on the gen AI tool you’re using, you can include text, images, and even audio references to sharpen your input. Whether you share your own work or include external references, clearly identify how they fit into your overall objective so the gen AI tool understands exactly what to emulate. And no need to build an exhaustive set of references—two to five should be enough.

For example, you could write: 

_Write a product description for a watch like it’s in a magazine._

Instead, write a prompt that provides relevant details, references two external resources, and identifies a format:

_Write a one-paragraph product description for a high-end watch with features like a scratch-resistant case and a water resistance rating of up to 30 meters. Base the description style on these examples from our website:_

- _Sunglasses: Our latest collection of handcrafted, heritage-inspired sunglasses features details like UV-protective lenses in shades specifically chosen to complement each frame—all at a price that won't break the bank. Plus, we made these sunglasses with vintage-inspired acetate frames and a keyhole bridge._
	
- _Cardholder: Crafted in smooth Italian leather, this double-sided cardholder is designed to carry your cash and credit cards without the bulk of a full wallet. Fun fact: this cardholder is made in Naples, Italy, and will look great when you treat your friends to a round of summer spritzes."_

Sweet spot for Gen AI tools are **two to five references**.
## Evaluate

Once you have your output, it's time to evaluate. Ask yourself if the input you provided gave you the output you needed. We technically not only do this at the second last, but do this after each and every step of the framework and iterate.

Different AI models are trained on unique data and rely on different programming techniques. Some models may be better suited to specific uses like writing code or brainstorming ideas, while others might have limited outputs because of their training sets. No matter the model, running the same prompt multiple times will likely render different results because of how gen AI tools process data. 

That’s why it’s so important to evaluate your output. Before you use any AI-generated information, text, or materials, critically evaluate that the output is accurate, unbiased, relevant, and consistent before incorporating it into your workflows. If the output isn’t what you’re looking for, you should iterate on your prompt.
## Iterate

If you evaluate your output and determine that you're not getting what you need, you can try again by adding more information or tweaking your prompt. And this is a key part of prompting effectively. We technically not only do this at the last, but do this after each and every step of the framework and evaluate, then iterate. There will be times when your prompt simply isn’t leading to the output you need. That’s where our **ABI** advice comes in: 

* **A** = Always
* **B** = Be
* **I** = Iterating

If you find an output lacking, continue clarifying what you need until it’s just right. There are four iteration methods,
1. Revisit the prompting framework = Re-iterate through the task, context and references.
	
2. Separate your prompt into shorter sentences = Break long prompt into shorter follow-up prompts. It can further improve precision of the output as Gen AI works on each shorter prompts rather than spending time on figuring out the relationships between each part of framework in one long prompt.
	
3. Try different phrasing or switching to an analogous task = Two prompts with same meaning, but both yield different outputs, latter being more precise. For example **"Write a marketing plan."**  vs **"Write a story about how this product fits into the lives of our target customer demographic"** (Analogous Task = A variety of tasks that use analogies to measure a person's performance or behavior).
	
4. Introduce constraints = Basically giving your context more depth and details. For example, you give enough context as your favorite singers in your prompt for a travel playlist, but these are songs you've already heard. We can add constraints like exclude this genre from this singer (For example, Metal and Jazz), include this time of song of this singer (For example, from the 90's). This help Gen AI to narrow down your output and give more helpful and unique responses to your satisfaction.

# Generate better outputs through iteration

Even with the **prompting framework** to guide you, sometimes you may still get an output that misses the mark. That’s what _**iteration**_ is for: to clarify and refine your prompt to better direct a generative AI tool towards the result you had in mind. But some types of iteration have the potential to be especially effective in breaking through creative blocks during prompt design, leading gen AI to new solutions and sharper output.

To iterate most effectively, prompt your AI tool in the same chat. That way, the tool can reference information you've provided it with in previous prompts and build on that knowledge.

Here’s how iteration works in action. Consider this example prompt: 

_Identify the latest developments in the restaurant industry._

It’s a simple prompt that only includes the _**task**_, and it might generate some broad insights, but chances are that you’ll need to iterate in order to get an output closer to what you want. You can try these four iteration methods to generate more useful outputs:

- **Revisit the prompting framework:** Make sure your prompt is clear about your desired task and includes a specific _**persona**_ and _**format**_, plenty of _**context**_, and offers relevant _**references**_ that help inform the output. Here’s an example:  _Create a bulleted list including the latest developments in the restaurant industry specific to urban areas that could impact the public reception of a dining experience using only ingredients native to the region._
    
- **Break the prompt into shorter sentences:** Instead of packing everything into a complex and lengthy prompt, address each individual step in a separate prompt until you’ve accomplished everything: Prompt one: _Create a bulleted list including the latest developments in the restaurant industry._ Prompt two: _Summarize the trends that would specifically impact restaurants in urban areas._ Prompt three: _Write a pros and cons list on how those developments could impact the public reception of a dining experience using only ingredients native to the region._
    
- **Introduce constraints:** Focus the gen AI tool’s output by adding constraints, or limitations, to your prompt. When you set boundaries for specific categories, lengths, formats, or other details in your prompt, you help the tool provide a more precise output. It’s like asking for a list of food recipes but specifying that the recipe should only use seasonal ingredients and take less than 30 minutes to prepare. Adding constraints can actually encourage more inventive, targeted results that better match your needs. Here’s an example: _Create a bulleted list including the latest developments in the restaurant industry specific to urban areas that could impact the public reception of a dining experience using only ingredients native to the region. This list should only include trends from cities with a population of more than 500,000 people, and should only include trends relevant to vegetarian and vegan restaurants._
    
- **Tweak your phrasing or switch to an analogous task:** Shift your language to explain what you mean in a different way. Or, try a different task that’s similar to what you’re trying to complete but different enough to trigger a new response. Here’s an example: _I’m starting a restaurant that will only include produce from within 50 miles. You’re a diner that lives in a major city and keeps up with the latest restaurant trends. Write a list of questions that I should consider before opening up the restaurant._

![Generate better outputs through iteration](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Generate%20better%20outputs%20through%20iteration.png)

# Multimodal Prompting

Basically prompts and outputs are not restricted to just text-based. We can use text-based prompt to create an image output (generate pictures) , an image prompt to create a document out or a video output (bunch of images to create a study document), an document prompt to create a text-based output (explanation of the contents of document in a easier manner), and so on. For example,
- You ask a gen AI tool to suggest recipes based on a photo of the ingredients in your fridge.
- You need to create a digital teaser to promote an event between two brands on social media. So you input both brands’ logos and colors into a gen AI tool, and ask it to generate a visual for the joint event.
- You’re working on a short story about a forest you just visited and need help describing the sounds and atmosphere. So you add some audio you recorded while visiting the forest to your prompt, and ask the gen AI tool to use it to inspire the atmosphere and details of the story.

## Benefits and considerations

Think about it like this: the world is multimodal. When you’re giving a presentation at work, you’re probably using text, images, and your own voice to help your audience understand your point. Multimodal prompting works in the same way. It reflects how you experience the world by building connections between text, images, audio, and other modalities, helping you provide clearer instructions to a gen AI tool.

Including multiple modalities isn’t a one-size-fits-all solution, but it can improve your prompts. For instance, if you ask a gen AI tool to write a poem about a sunset and include a photo of one in your input, the gen AI tool can use the photo to describe specific colors and details. The result is a much more vivid poem.

While multimodal prompting is versatile, it has some limitations. Gen AI tools sometimes struggle with abstract ideas, handling complex combinations of modalities, and occasionally, just plain old common sense. For example, while gen AI tools are always evolving and improving, multimodal prompting isn’t reliable for counting just yet.

## Multimodal prompting examples

Multimodal prompting is most effective in situations where you need to transfer information from one media to another. Here are a few examples:

- You ask a gen AI tool to suggest recipes based on a photo of the ingredients in your fridge.
    
- You need to create a digital teaser to promote an event between two brands on social media. So you input both brands’ logos and colors into a gen AI tool, and ask it to generate a visual for the joint event.
    
- You’re working on a short story about a forest you just visited and need help describing the sounds and atmosphere. So you add some audio you recorded while visiting the forest to your prompt, and ask the gen AI tool to use it to inspire the atmosphere and details of the story.

## Generic prompting framework

- **Task**: Along with being specific about a _**persona**_ and _**format**_, be specific about how you want different modalities to be used and why you’re including them in the task. 
	
- **Context**: Just like in a text-based prompt, you’ll need to add context so the gen AI tool knows exactly what you want it to do. Consider which modalities you’re using in your prompt when providing context and if there are any specific constraints or considerations that are important to include. For example, if you input an image of the inside of your refrigerator, you may only want the gen AI tool to consider the fruits and vegetables in the image and not any of the packaged goods.
	
- **References**: Share written, visual, or audio references to help gen AI tools understand the type of output you’re trying to create. Not every tool supports every sort of reference, so make sure you’re using a gen AI tool that supports the references you want to give it.
- **Evaluate**: Run the prompt as usual, but take extra care to evaluate how the output looks or reads. Since you’re using different modalities, that might involve a more detailed review of the output than simply evaluating a text response.
	
- **Iterate**: If the output is not meeting your needs, try one of the four iteration methods: you can revisit the prompting framework, break the prompt down into shorter tasks, introduce constraints, or tweak your phrasing or switch to an analogous task to help trigger a different, potentially better, response.
## Text -> Image

We use same principles as the basic framework. First the task, and since it's an image next will be the format, then some little context, and at the end, the next sub-heading.
Image generation prompts should specify:
* Size
* Color
* Position
* Aesthetic
Then we evaluate and iterate accordingly with the format of generating images, and continue doing this until we get out desired image.

## Image + Text -> Text

We use same principles as the basic framework. First the task along with a format, then some little context and give our image as a reference. We can also use other references to give more context in a way, further fine-tuning Gen AI to give a more desirable output. For example, caption for a social media post.

## Document + Text -> Text

We use same principles as the basic framework. First the task along with a format of how we want it to extract details from our reference, then some little context and give our document as a reference. We can also give more formats on how we want to the document to be analyzed and what we want from the document in a easier and readable manner in a way, further fine-tuning Gen AI to give a more desirable output. For example, study guide or short-hand explanations from a document with college notes.

# Hallucinations

When a gen AI tool provides an output with false information, it’s called a hallucination. Hallucinations can happen at any time and may happen when a gen AI tool gets vague or unclear instructions or when it generates an output about something it hasn’t been trained very well on. For example, a gen AI tool might miscalculate a math problem or include an incorrect ingredient for a recipe. To navigate hallucinations:
- **Fact-check and cross-reference:** Some gen AI tools have features that provide sources for where information was found. You can also fact-check an output by using a search engine to confirm information. You can even enlist the help of an expert if they’re available to you. Running a prompt through two or more resources helps you identify possible discrepancies in your output. 
	
- **Use clearer or more detailed language:** Sometimes, a gen AI tool will misunderstand something in your input, or if your input is wrong in some way, it could impact how a gen AI tool processes it. For example, if you wrote “Why is Toronto the capital of Canada?”, the gen AI tool may use your input as if it’s correct and give you a false history of Canada choosing Toronto—instead of Ottawa—as its government seat.