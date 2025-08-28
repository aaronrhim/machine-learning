# Brainstorm #1: Interactive ML Concept Visualizer

## Project Vision

I want to do a project that helps users visualize machine learning concepts through prompt engineering. The unique aspect though is that I want the LLM to question the user's prompts, because one of the biggest problems now is that LLMs tend to just follow whatever they are asked to do without thinking about whether its an actually effective way to approach the problem.

Here is an example: often when a user wants to start a new project, they don't know what to do so they prompt cursor a general command such as "do this this and this" and expect cursor to be able to understand them perfectly and generate the whole project for them. The problem with this though is that this won't work but does the LLM usually question the user's prompt? No it doesn't.

Right so thats why i want to make an LLM that can correct things like this. However, I want it to be in the form of a visualizer.

One of the problems when it comes to LLMs is that, if a user tries to ask the model to explain something very broadly, then the model will often try to explain things in a way that makes sense to other people but not the user themselves.

Anyways do you see what I'm getting at? Can you sort out my thoughts and ask me more questions to clarify certain pieces?

## Your Project Concept (as I understand it):

**Core Idea**: An LLM-powered visualizer that teaches machine learning concepts through prompt engineering, but with a unique twist - it questions and challenges user prompts instead of just executing them.

**Key Problems You're Addressing**:
- LLMs blindly following instructions - They don't question whether the user's approach is effective
- Vague prompts leading to poor results - Users give broad, unclear instructions expecting perfect outcomes
- Generic explanations - LLMs explain concepts in ways that don't resonate with the specific user

**Your Solution**: An interactive visualizer that:
- Questions user prompts to help them think more critically
- Provides personalized explanations based on the user's level
- Visualizes ML concepts in a way that makes sense to that specific user

## Clarifying Questions:

### Visualization Focus
**Question**: What types of ML concepts do you want to visualize? (e.g., neural networks, decision trees, clustering, regression, etc.)

**Answer**: For now, I just want to stick to supervised and unsupervised learning and visualizing a few specific ideas such as convolution, max pooling, gradient descent, things like those. The reason being is that I want the AI to effectively listen to the user's prompts, force itself to think about what the user is really asking for, and creating a visualizer based on the best way it believes thee user might understand the concept. The idea is that not everyone learns the same way. Some visualizers might not be as effective on some users as other visualizers are. Things like these.

### Interaction Style
**Question**: How should the LLM question prompts? Should it:

#### Ask clarifying questions?
**Answer**: Well first the LLM should try to understand what the user is asking for. If the understandment requires multiple ideas to be tackled at the same time (e.g. if the prompt is build me a website that has a cool scrolling mechanism, this prompt is so general and vague and in most cases, the LLM might think that it would be better to create a whole website that includes buttons linked to pages, information etc, when in reality, all the user actually wants is to tackle one single thing: a cool scrolling mechanims). Right? So the idea is that if the LLM can understand, then it can ask clarifying questions: "do you mean to say... expand on this idea more... can you make your question more specific because your current command will waste millions of tokens" things like this.

#### Suggest better approaches?
#### Show examples of good vs. bad prompts?
**Answer**: Yes this honestly might be a good idea. I was thinking making the LLM suggests more specific, clear ideas of what it thinks the user is trying to say. For example, again, if the user just says "build me a website that has a cool scrolling mechanism" the follow up question would be "what do you mean? do you want me to build the whole website that includes yada yada or do you just want to learn how to do a cool scrolling mechanism..." something like this. Now of course, I am not trying to make an LLM that embeds itself into a repository like cursor does and for now I'm just interested in making a model that helps visualize concepts, but I hope you see what I mean.

#### Provide step-by-step guidance?
**Answer**: If the user is really struggling, this might be a good idea. In that the bot pushes the user to think more about what they truly want.

### User Experience
**Question**: What should the interface look like?

**Answer**: I was mainly thinking about a normal website with a homepage that pitches "learn about ML here" and while there are a couple features, the real main feature is just the chatbot that is trained to answer questions related to ML and help users learn about them, visualize a few of the processes, and improve their prompt engineering skills.

**Options to consider**:
- Web app with interactive diagrams?
- Chat interface with visual elements?
- Code playground with explanations?

### Target Audience
**Question**: Who is this for?

**Answer**: Anyone willing to use the application so it could be ML beginners who are just trying to learn the theory and visualization but it could also be people who actually want to get into the engineering side and are interested in improving and optimizing their abilities.

**Potential audiences**:
- ML beginners?
- Students?
- Developers learning ML?
- General public?

### Prompt Examples
**Question**: Can you give me a specific example of a "bad" prompt and how your system would respond to it?

**Answer**: I did a couple times above.