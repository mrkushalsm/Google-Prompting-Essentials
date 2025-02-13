# AI to uncover hidden patterns in data

We use the TCERI prompting framework to unlock insights and patterns from data using Gen AI tool. Remember that not all Gen AI tools work with data and to check what the tool can do before using it, and always review your organization's policies before including sensitive or confidential data in your prompt.

For this example, we'll be using publicly available data found on Kaggle. Let us say we have the following dataset with information about a grocery chain,

![Grocery chain dataset.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Grocery%20chain%20dataset.png)

We can use Google AI Studio to help analyze all the data and to find trends and patterns that could help inform how the company operates.

Since there are a lot of variables here, so to make it easier to work, we shall organize the data to make it easier to work with.

We first ask for step-by-step help, by first uploading the data directly to Google Drive where the Google sheet is stored. But if we are using it locally, we'll have to upload it from our computer.

Then we get ready to write the following prompt,

Context \[Attached is a Google Sheet of stored data.\] + Task \[How can I create a new column in Sheets that calculate the average sales per customer for each store?\]

If given given output is not what was desired, we can iterate on our prompt to get an output that's closer to what we need.

Discovering trends in a dataset can help us make informed decisions and we can prompt a Gen AI tool to help find those trends.

We re-iterate as follows, keeping the above sentence in mind,

Task \[Give me insights into the relationship between "Daily Customer Count", "Items Available", and "Sales" based on the given data.\]

We get an output that the Gen AI caught as relationships between the following columns, give what they are and their reason to exist to investigate further, and think about potential sales strategies.

# Strategies for Data Analysis

Have a dataset you’ve always wanted to explore? Lots of numbers you need to make sense of? In seconds, generative AI can help you spot patterns, notice connections between data points, and identify trends, all of which can empower you to make data-backed decisions with confidence.

All it takes is the right prompt. Writing a prompt to analyze a dataset can come with some quirks. But one thing to keep in mind throughout this reading is that the trusty **prompting framework** will guide you. That means you’ll **T**houghtfully **C**reate **R**eally **E**xcellent **I**nputs, only this time, you’ll tweak your strategies slightly to make them more dataset-friendly. Here are a few prompting strategies to help you get the most out of your data. And remember—always review your company’s policies before including sensitive or confidential data in your prompts.

## Shape your prompt to the model’s abilities

When it comes to using gen AI tools to analyze your data, your prompts needs to account for the strengths and limitations of the technology you are using. Understanding what sort of data analysis a gen AI tool is good at will help you tailor your prompts and get the most from your outputs. 

Here are a few examples: 

- **Text analysis:** Easily surface themes, determine tone, and classify key topics in text-based data. Have a few thousand open-ended responses from a community survey? Gen AI can help you quickly understand what’s most important to people, how they feel about the town’s proposed plans, and where the final initiative should make an impact. 
	
- **Data augmentation:** Expand a limited dataset with simulated data to make it more robust. Say you work in fraud prevention. You want to analyze your company’s data about fraudulent purchases, but there are only a handful of data points. You can prompt a gen AI tool to generate new data from your current dataset to get a more comprehensive view of how fraud might happen and what to look out for. The key with data augmentation is to be transparent about what's real and what's augmented data, and the augmentation should be as realistic as possible. Augmentation can’t give you hard facts, only suggest trends. Like with the other data uses, you should always check your organization's policies. 
	
- **Question and answering:** Get answers about your data in plain language, like whether your sales from last quarter were up or down. It’s like checking in with your colleague who compiled the information—just with fewer emails.
	
- **Scenario analysis:** By noticing patterns in past data, gen AI tools can make educated guesses about what might happen in the future. That means you can play out different scenarios to check what kind of impact they might have, like prompting to ask how a change in traffic patterns would impact your commuting time, or which days of the week your office space should expect the highest number of visitors.
	
- **Image and visual analysis:** Gen AI can help you quickly identify patterns and come to conclusions about your visual data without having to sift through stacks of images or watch hours of footage. You could even paste in a chart displaying your team’s sales figures for the past two years in your prompt, and ask questions about it for more focused analysis. 
	
- **Customer and market research:** A gen AI tool can analyze surveys, social media, and other industry-specific data like charts and graphs to uncover what customers want and how your market is changing.

If you’re eager to use gen AI tools, but need to complete a data analysis task they’re not really built for—like rigorous statistical analysis, or really anything with highly structured data—don’t worry. You’ll just need to adapt _how_ you prompt the tech to best suit its capabilities. For example, instead of having the gen AI tool do statistical analysis _for_ you, ask it to suggest the most effective methods based on your data with step-by-step instructions. Even if you’re not a coding expert, you can use gen AI to help you learn about different analysis methods quicker than if you were learning on your own. Designing your data analysis prompts to align with the limitations of gen AI doesn’t have to restrict your work. Keeping the tech adaptable to and useful for your needs can open doors to unexpected creativity.

|                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| P.S. Since we’re discussing the limitations of AI, now’s a good time to remind you about hallucinations. If you’re following our prompting framework, you’ll be _**evaluating**_ outputs as you go. But keep in mind that spot checking doesn’t really work for datasets—out of 100 generated data points, only 10 might be hallucinations. So keep a close watch on your outputs, and try to only generate information that can be easily cross-referenced. |

## Get your dataset ready

An output is only ever as good as the data it’s based on. That means you need to validate your data and continually check the information you’re analyzing with gen AI.

Before entering data into a gen AI tool, make sure the data is:
* Up to date
* Consistent
* Accurate
* Relevant
* Complete
* Bias-free

![Get your dataset ready.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Get%20your%20dataset%20ready.png)

Luckily, gen AI tools can help you get your dataset prepared and ready. Try using a gen AI tool to identify errors, spot strange-looking data points, and standardize how things are formatted.

For example, maybe you want to figure out if your dataset is inaccurate. Here’s a prompt for that:

Data \[Here's a sample of my data.\] + Task \[Identify any potential issues or inconsistencies in the data, and suggest ways that I can address them.\]

Cleaning up your data before conducting further data analysis is also a good example of how you might use multiple different tools to investigate one single dataset. For example, you could use one gen AI tool to convert a dataset’s format, then another to ask questions about the newly organized information. Regardless, preparing a quality dataset is an important first step in conducting all kinds of data analysis, so make sure your information is updated, clear, and complete.

## Encourage exploration

Gen AI is really good at uncovering insights that may be hiding within a large dataset. You just need to know how to prompt the tool the right way.

You want to ask broad, open-ended questions. By not being prescriptive, you’re giving the gen AI tool a chance to identify patterns and detect insights with some freedom, which may introduce or reveal trends you weren’t expecting. Above all, stay curious. You might find something unexpected just by keeping your perspective open.

For example, you’re a journalist conducting research for an article about the real estate market. You’ve been provided with a large dataset showing vacant residential properties by district in a handful of cities, but you’re not sure what conclusions can be drawn from it. You might write:

Persona \[You’re a journalist investigating housing trends.\] Task \[How would you use this vacant property data to tell a compelling story about the real estate market?\]

As always, follow the prompting framework to evaluate your output for credibility and accuracy.

## Take advantage of embedded AI tools

Plenty of existing data analysis platforms embed AI right into their user interface, making it even more convenient for you to analyze information. You might already work in these platforms, or at least have some familiarity with them. But even if not, these integrations make analyzing your data a seamless process by bridging the power of AI and specialized data analysis systems, like in the following platforms:

- **Gemini in Google Sheets** (link:- https://support.google.com/docs/answer/13951830?hl=en)**:** Create tables, establish formulas, and summarize Drive files or Gmail messages to organize and analyze your data directly in your spreadsheet. 
	
- **Tableau Pulse** (link:- https://www.tableau.com/products/tableau-pulse?d=7013y0000020Gu8AAE&nc=7013y0000020ID1AAM&utm_content=7013y0000020Gu8AAE&utm_source=google&utm_medium=paid_search&utm_campaign=21313557030&utm_adgroup=162407950469&utm_term=tableau%20gpt&utm_matchtype=e&gad_source=1&gclid=CjwKCAjwk8e1BhALEiwAc8MHiCWb_7MC6A-an9rAamMbEqsagkfOkJhCC9-E1IwVjjtIVwkYlRGsjhoCo94QAvD_BwE&gclsrc=aw.ds)**:** Receive personalized, automated insights about your data (link:- https://help.tableau.com/current/online/en-us/pulse_intro.htm) as snapshots on the Tableau Cloud platform, or regular digests sent through Slack or email. 
	
- **Looker Studio** (link:- https://cloud.google.com/looker-studio)**:** Access a robust library of report templates, easily explore underlying data through prebuilt data connectors, and embed final reports into any web page or intranet to share your findings with the audience that needs them most. 
	
- **BigQuery data insights** (link:- https://cloud.google.com/bigquery/docs/data-insights)**:** Uncover patterns, assess data quality, and perform statistical analysis by generating automated queries based on your information’s metadata. 

When you’re preparing to analyze your data, determine whether you can use embedded AI tools to help. When it comes to prompting in these platforms, remember to follow the prompting framework to get the most out of your output. For example, maybe you’ve saved that vacant property dataset in Google Sheets. You can open the side panel and type:

Task \[Create a table\] + Format \[that includes the median rate of vacancy for each city in the dataset.\] 

The next time you’re working with a dataset, remember you’ve got a powerful assistant in gen AI tools. By crafting the right prompts for the right tools, keeping your data tidy, asking broad questions about your information, and taking advantage of all kinds of tools, you’ll find stories and insights that might have otherwise stayed buried. Who knows what you’ll uncover next.

# Decipher spreadsheets

Imagine your coworker at a restaurant went on vacation and gave you a spreadsheet full of data and formulas. Some of them seem familiar, but there are others that are a little more complicated. You need to order inventory today, but you don't wanna bother your colleague, so you turn to a Gen AI tool for some guidance.

We write the prompt as follows,

Persona \[I work at a large restaurant and I need to order inventory while my co-worker is on leave.\] + Context \[They left me with a formula to calculate how much food to order, but I don't understand it.\] + Your Formula + Task \[Explain what the formula means\] + Format \[in simple, step-by-step terms.\]

We now, if output is what we desired, get a clear sense of what the formula is trying to accomplish so that you can get the stock order handled quickly.

Now that you understand the formula does, let's say you get stuck somewhere. You can ask Gen AI to help you out through iteration. Taking another example, let's say we received an error message in your spreadsheet and not known what to do. We shall ask the Gemini for help to learn how you can figure out where those errors are coming from.

Let's use the following prompt,

Context \[The Google sheet I have uses this formula to calculate orders: YOUR FORMULA. However, I have received an error message in one of the cells.\] + Task \[Give me\] + Format \[step-by-step\] + Task (contd.) \[process for finding the error and fixing it in Google Sheets.\]

Gemini, if desired output received, will give you clear instructions for resolving the error message and with those out of the way, we can get that inventory order moving.

# Decipher almost anything with the help of AI

Want to learn faster or more effectively? No matter what your job is, chances are you've come across information that you didn't understand. Or maybe you had the answers you needed, but they were hidden behind dense jargon, unknown formats, or even new languages. Luckily, generative AI can act as your personal translator and help make the unfamiliar more accessible. 

Below are a few ways you can use a gen AI tool to deepen your understanding of something you might be struggling with. (Keep in mind that the example prompts below are only highlighting the _**task**_ from the **prompting framework** to show you specific ways to decipher content with gen AI.)
### Translate to another language

Working with clients who speak a different language? Or curious about an unfamiliar word you heard on a podcast? Gen AI tools are capable of simple translations and more, so you can use them whether you need a word-for-word conversion or something more nuanced and idiomatic. You can prompt them to:

- **Translate text:** _Translate this email to Spanish…_
- **Provide definitions:** _What does “hygge” mean in English?…_
- **Explain idioms and figures of speech:** _Explain the phrase “saru mo ki kara ochiru…”_

### Interpret jargon

Whether your company is adopting a new software or you’ve come across some unfamiliar industry lingo, a gen AI tool can break down jargon so even the most complex or new-to-you concepts are understandable. Try prompting a tool to:

- **Define terms:** _What is compound interest in simple terms? …_
- **Explain concepts:** _Explain what social-emotional learning (SEL) is in one paragraph …_
- **Provide contextual examples:** _Can you give five examples of how natural language processing (NLP) is used in everyday life? ..._

### Demystify spreadsheets

Have you ever received a dense spreadsheet with hundreds of cells, complicated formulas, and numerous tabs? What about one that’s full of errors? Whether you’re a novice or a spreadsheet wiz, these files can be complex. The good news is that if you input the spreadsheet into a gen AI tool or prompt Gemini in Google Sheets, gen AI can help you understand it. Next time you’re stuck or just want some help, prompt a tool to:

- **Explain formulas:** _Explain the formula in cell B12 in three sentences ..._
- **Identify errors:** _Are there any inconsistencies in this data? If so, share them in bullet format ..._
- **Extract specific data:** _What were the total Q3 sales for our hair gel versus our shampoo? Provide them in percentages, as well as dollar values ..._
- **Summarize key findings:** _Write a one-paragraph summary of the trends in this spreadsheet of monthly website traffic ..._

### Understand error messages

Have you ever received an unfamiliar error message on one of your devices that you needed to understand quickly? A gen AI tool can help you decode it, _and_ find solutions fast, so you can get back on track. Next time you get an error message, try prompting a tool to:

- **Explain the error:** _What does “Error 404: Not Found” mean? ..._
- **Troubleshoot the problem:** _My computer says “Kernel Panic.” How can I fix this? ..._
- **Identify potential causes:** _Why am I getting a “Connection timed out” error message in my browser? ..._

### Get help with coding

If you’re just starting out with coding or need to get familiar with specific languages for things like web development or data analysis, a gen AI tool can act as a coding assistant. Some tools like **Google Colaboratory (Colab)** (link:- https://colab.research.google.com/) and **Vertex AI Codey** (link:- https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/code-completion) are designed with coding in mind, and can help you do things like generate code or identify functions and bugs.

Remember that it may be difficult to evaluate a coding output if you’re just starting out with code. You may need some extra research or expertise to check for hallucinations in the results. After you’ve entered the code into your input, try prompting the gen AI tool to:

- **Explain code snippets**: _What does this Python code do? Explain it so a true beginner could understand ..._
- **Generate code**: _Write an R program that finds the common information between two input lists ..._
- **Debug code**: _This JavaScript function is supposed to calculate the area of a rectangle, but it's returning the wrong answer. Can you find the error and tell me how to fix it?_ ...

### Explain complex data

If you’ve ever looked at a chart or graph and had trouble finding an insightful data point, a gen AI tool can provide assistance if you prompt it to:

- **Summarize trends**: _What are the main trends shown in this line graph? Provide one-sentence explanations of each ..._
- **Identify outliers**: _Are there any unusual data points in this scatter plot? ..._
- **Explain correlations**: _Does this bar chart show a correlation between advertising spend and sales? ..._

Beyond interpreting charts and graphs, gen AI tools can also help you create your own CHECK LINK[but more on that later](https://www.coursera.org/learn/google-prompting-essentials/item/lbk7b).

Gen AI tools can help you explore new ideas, solve problems more effectively and quickly, and ultimately, learn and grow with the knowledge you’ve gained. 

One final note: Always remember to _**evaluate**_ outputs when you’re using gen AI to find answers about topics that are new to you. When you’re asking questions about unfamiliar concepts, or working with new languages, you need to be even more discerning with the outputs. Think back to the CHECK LINK [tips for responsible prompting](https://www.coursera.org/learn/google-prompting-essentials/supplement/7AaAb/tips-for-responsible-prompting) to make sure you’re receiving accurate information about the topics that interest you.

# Bring data to life with visualizations

You just need to know what to ask for. You can prompt a gen AI tool to get advice on the best types of charts and graphs to illustrate your data. The prompting framework should still be your guide. Add your task, context, and references if needed. Evaluate the output and iterate. The clearer you are about the kind of chart you want and what the parameters are, the more useful your output will be.

Let's assume we are co-owners of a bookstore. Here's a list of best-selling books and how many copies have been sold around the world since they've been published,

![List of best-selling books.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/List%20of%20best-selling%20books.png)

Remember, not all gen AI tools can analyze data. Be sure to check what your tool can do before using it.

We'll use Google AI Studio here to visualize this data. If you don't know what type of chart to use, you can always prompt a gen AI tool for suggestions.

This shall be our prompt to find out what kind of chat might work best, after uploading the spreadsheet,

Context \[My data set is a spreadsheet that uses columns: Title, Published, Genre, First published and Approximate sales in millions.\] + Format \[Give me options for a chart that shows correlation between genre and sales.\] + Task \[Explain how genre and sales are correlated according to the information.\]

If we have got the desired output, the model will give the best way to represent this as a chart, along with explanation on what columns should be on the X and Y axis along with an interpretation of how the chart will be.

You're not always gonna know what type of chart you want to use, which is where adding a reference to your prompt can be helpful. You can use charts that are similar to what you want or charts you found helpful, and include those as a reference in your prompt. Then ask for recommendations on how to create a similar chart using your data.

Start by uploading the sample chart and then prompt the model to get some information about what it's depicting. Remember, it's sometimes better to start simple and then gradually add complexity. The prompt is as follows,

Task \[Describe this chart. What kind of data relationships are highlighted in the chart\]

If desired output obtained, it will tell you what type of chart it is and what the chart is highlighting and explaining, and also giving an in-depth explanation on what each input does with data relationships highlighted.

Now we shall use this example chart to tell the model to generate a chart based on the chart given above, as follows,

Context \[My data set is a spreadsheet that uses columns: Title, Published, Genre, First published and Approximate sales in millions. I'm interested in showing the relationship between genre and sales.\] + Task \[\Suggest modifications to make this chart work better with my specific data using Google Sheets.]

If desired output obtained, the model will give you an explanation on how to create a new chart, how to prepare your data for the new chart, and the output even explains how to modify a bar to illustrate the relationship between genre and sales more clearly. And remember, if your output doesn't match what you need, you can always tweak your prompt and iterate.

# Get a head start on presentation speaker notes

Gen AI tools can help,
* Organize your presentations
* Build talking points
* Create images

Here, we'll be using Gemini to bring it all together.

In this scenario, you work for a company that designs, makes and sells headphones. You're preparing to pitch your team on some cool new features. There's a lot of information and insights to convey, so you'll need to distill what you learned into a clear presentation.

First, let's prompt Gemini to help figure out how to structure the presentation and summarize the findings, as follows,

Persona \[\I'm a product designer at a headphones brand.] + \[I'm putting together a presentation for my team about what new features should be included in our next product line. The presentation includes findings from our market research on features that our 18 to 34 year old customers want their headphones to have. These features include new colors, the ability to control playback with head movements and noise-cancelling capabilities. Consider the relationship between our demographics' disposable income and their most important considerations when buying headphones.\] + Task \[How should I structure my presentation?\] + Format \[List each slide's topic with its key points and visuals.\]

If obtained output is what was desired, though the following might not be same for your output, Gemini has suggested a structure for your presentation that includes key points and visuals for each slide, including a title slide, an intro that sets the stage and details on the three features that the audience is interested in. Gemini might have even suggested a call to action at the end of the presentation.

There are a few other things that you can do to make it more engaging, like adding visuals that compliment the information on the slides.

When using gen AI for image generation, you want to use the prompting framework with a few additional things added in. You want your input prompt to be as vivid and detailed as possible to help the Gen AI tool determine the type of image you want to create. Image generation prompts should specify,
* Size
* Color
* Position
* Aesthetic

We shall generate the images with the following prompt,

Task \[Generate close-up images\] + Context \[of a pair of sleek silver headphones on a desk in a college dorm room. They should have musical notes floating around the headphones to show that they're playing music.\]

If obtained output is what was desired, Gemini will have generate several images (probably 4) matching your prompt.

You can even choose between photography, vector art, sketches, or watercolors for the style. You still want to evaluate the output just like you would when generating text. Check your images to make sure you're getting what you want and that there aren't any mistakes, like a headphone cord that's not plugged in or anything else that seems off. 

And remember, part of being a responsible gen AI user is disclosing when you've used these tools. So add a disclaimer whenever you're including an AI-generated image in your work.

# Receive instant feedback on a presentation

Now you've got your presentation ready, you can still continue to use the same Gen AI tool to to give you a head-start and generate speaker notes for you. For this example, we need a long context window. Remember, long context windows aren't available on every AI tool. Different tools have different capacities. For this example, we'll switch to Google AI Studio.

We upload our slide to the Untitled prompt, and then give the following prompt,

Persona \[I'm a product designer at a headphones brand.\] + Context \[I'm presenting a Google Slides presentation for my team about what new features should be included in our next product line. The presentation includes findings from our marker research on features that our 18 to 34 year old customers want their headphones to have.\] + Task \[Provide multiple options of\] + Format \[concise, personable and engaging\] + Task \[speaker notes I can use while presenting this slide.\]

You can get more specific. You learn that your company's marketing director will attend the presentation. You can prompt the model to adjust the speaker notes for a more senior audience.

We shall iterate through the following prompt,

Task + \[Provide alternate speaker notes for this slide\] + Context \[that are specifically directed toward my headphone company's marketing director. The director values precision and their priorities for the organization are to stay on top of industry trends and foster a strong community of loyal customers.\]

And just like that, you have new speaker notes that are more appropriate for a marketing director.

You have the presentation and the speaker notes, but you wanna fit in some practice before the big day. You can upload a recording of yourself to get specialized feedback.

Then we can give the following prompt specifying the tone and what we want to accomplish,

Context \[I'm giving a presentation to my manager pitching new product features and I want to sound authoritative and confident. I'm going to read my presentation aloud.\] + Task \[Afterward, give me a feedback on whether I've accomplished this goal.\]

Since you're using a gen AI tool with a long context window or large memory, you can save your prompt and come back to where you left off. You can continue practicing without starting all over again.

# Fine-tune gen AI outputs by adjusting tool settings

Have you ever noticed that the same prompt can produce different results? That’s because generative AI tools use probability to decide what information to draw from when selecting its output. It’s like rolling a die to help you decide what to choose. But, you can actually influence the probability of an output being selected by changing the settings called sampling parameters. Knowing when and how to adjust these settings will allow you to pursue AI generated solutions with greater specificity or creativity, cutting down on hallucinations or generating more helpful results.

## Temperature

Think of sampling as taking a bite-sized piece of a much larger pie. When AI generates text, it doesn't consider every possible word or sentence at once. Instead, it samples a few possibilities based on the data it has been trained on. Sampling parameters are the guardrails that influence this process, allowing you to expand or limit the pool of options that a gen AI tool chooses from as it crafts its output. And the sampling parameter that dictates the probability of those options within that pool is called the temperature. You can think of it as giving your gen AI tool instructions on whether to give you a narrow, straightforward response, something much more creative, open-ended or surprising, or a response that’s somewhere in between. 

Imagine that you're trying to decide what to eat. You have a menu of options, but you're not sure which one to choose, so you roll a die. You can give your favorite dish three sides of the die, your next preference two, and your third preference one—or you can give them each two sides. Temperature determines the chances that you try something unexpected.

Here’s how it all works.

## Temperature sampling

Imagine that you’re telling a friend about the errands you ran earlier that day. A sentence beginning, “This morning, I went to the” could end in a bunch of different ways, but there’s a better chance that your next words will be “grocery store” or “parking lot” than “haunted house” or “moon.” By changing the temperature, you can adjust the degree of randomness in a gen AI tool’s output.

- A lower temperature favors more likely, expected results. When you need realistic results or  hoping to create an accurate output, like summarizing an academic paper or generating a timeline of events, a low temperature is recommended to have the highest likelihood of getting factually accurate results.
- A higher temperature gives less likely results a better chance of being selected. If you’re working on a creative task like writing a short story or thinking up an original product, and the gen AI tool is producing repetitive or generic responses, try raising the temperature.

![Temperature sampling.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/Temperature%20sampling.png)

Setting the temperature to a low score like 0.1 would give the most-likely option (“grocery store”) the highest chance of selection and the other options a significantly lower chance. A higher temperature score like 1.5 would still leave the most-likely option with the highest chance of selection, but it’ll also give the less-likely options a much better chance, though that can also lead to unlikely (“volcano”) or even highly improbable (“the moon”) responses. 

You can configure these settings in most gen AI models’ API, but when you open a new chat thread, the settings will revert to default.

## Top-k sampling

While the temperature score determines the probability that a gen AI tool will choose an individual response, other sampling parameters determine _how many_ responses gen AI can choose from. The top-k value sets the total number of tokens—the basic units of information—from which the gen AI tool selects for its output, letting you hone in on your desired results with more precision.

- Setting the top-k value to the minimum of 1 (or setting the temperature to 0) will always guarantee the most likely result, which is called “greedy decoding.” This output is no longer random, it is deterministic, meaning the same result will be generated from the same prompt every time.
	
- A lower top-k value will narrow the field of available options for output, which can help with reducing hallucinations. When you’re doing market research but the results don’t make sense, it’s time to lower the top-k value.
	
- A higher top-k value can produce surprising results that can be useful for thinking outside the box. If you’re getting ready to launch a new service (or putting together a trivia team) and looking for a name that really pops, a higher top-k value might lead to a breakthrough.

## Top-p sampling

Where the top-k value sets the number of tokens from which gen AI selects, the top-p value further refines that pool using total combined probability. Each token has a probability score between 0 and 1.0, quantifying the chances that gen AI will randomly select it in its response. Gen AI tools will only choose from tokens (starting with the most likely and going in descending order) until the sum of their probability scores reaches the given top-p value, which is another way of telling the tool what you need from it. Think of sampling like looking for a new comic-romance book to read at the library: You might grab 10 different books off the shelf (that’s your top-k score), but then you’ll further refine your selection based on which books best fit your preference, and that’s where top-p comes in. At a very low top-p score of 0.1, you’re guaranteed to read the most popular best-seller, but a higher top-p score like 0.8 might lead to a pleasant surprise from a lesser-known choice.

- At the default setting of 1.0, the top-p value has no effect on sampling.
	
- A lower top-p value (less than 1.0) removes the least likely responses from the gen AI tool’s consideration. When asking a gen AI tool to process statistics and present analysis to answer a specific question, a lower top-p value may work best.
	
- A higher top-p value allows the gen AI tool to choose between responses more freely, which can help with tasks that require comparisons between different outcomes. If you’re stuck while deciding what sort of promo event will raise awareness of your brand, repeating your prompt with a higher top-p value will bring you a wider variety of suggestions.

## The effect of temperature score on top-p and top-k selection

![The effect of temperature score on top-p and top-k selection.png](https://github.com/mrkushalsm/Google-Prompting-Essentials/blob/main/images/The%20effect%20of%20temperature%20score%20on%20top-p%20and%20top-k%20selection.png)

With all three sampling parameters, a high score can spark surprising insights—but that increase in randomness can also lead to hallucinations, so don’t forget to check the output. 

In creative brainstorming, the best idea isn’t necessarily the first one that comes to you, and AI’s most productive suggestions won’t always have the highest probability. Tinkering with temperature score, top-k value, and top-p value can open up new pathways for exploration or narrow it down to the one you need.
