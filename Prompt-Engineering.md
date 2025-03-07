# Prompt Engineering Guide

Quick reference guide for getting better results from large language models.

# Prompt Structure Guidelines

| Component | Purpose | Example |
|-----------|---------|---------|
| Instruction | Defines the task. | "Summarize this article in 3 bullet points." |
| Context | Provides necessary background information. | "Summarize the impact of AI on e-commerce based on this blog post." |
| Constraints | Sets rules like length, style, or format. | "Write in a formal tone, limit to 150 words." |
| Example (if needed) | Shows what kind of response is expected. | "Respond in the style of a Twitter thread." |

## Six Key Strategies

### 1. Write Clear Instructions

- **Include specific details** in your query (e.g., "Write a brief, expert-level response" instead of just "Tell me about...")
- **Ask the model to adopt a persona** (e.g., "Act as an experienced software engineer")
- **Use delimiters** (quotes, XML tags, etc.) to separate different parts of your input
- **Specify step-by-step instructions** for complex tasks
- **Provide examples** of desired outputs when possible
- **Specify desired output length** (in words, paragraphs, or bullet points)

### 2. Provide Reference Text

- Include reference material in your prompt when possible
- Use phrases like "Use only the information in the following text to answer..."
- Request citations (e.g., "Cite the specific parts of the text that support your answer")

### 3. Split Complex Tasks into Smaller Steps

- Break down difficult problems into simpler sub-problems
- For multi-stage tasks, feed the output of earlier steps as input to later steps
- For very long conversations, summarize or filter previous dialogue
- For long documents, summarize sections separately, then combine summaries

### 4. Give the Model Time to "Think"

- Ask the model to solve a problem step-by-step before giving the final answer
- Use phrases like "Think about this carefully" or "Work through this systematically"
- For complex reasoning, use techniques like "inner monologue" (hidden reasoning)
- Follow up with "Did you miss anything?" to encourage checking work

### 5. Use External Tools

- For factual tasks, provide relevant information in the prompt
- For calculations or code execution, ask the model to output code that can be run
- Consider function-calling capabilities for structured outputs and API integration

### 6. Test Changes Systematically

- Test your prompts with diverse examples
- Create evaluation procedures to compare prompt performance
- Use automated testing with many examples for greater confidence

## Quick Tips for Better Results

- If outputs are too long/short, explicitly ask for your desired length
- If answers are too simple/complex, specify your expertise level
- If you dislike the format, show exactly what format you want
- For creative tasks, provide examples of style, tone, and quality
- For factual questions, ask the model to cite its sources
- For math or complex reasoning, tell the model to "think step by step"
- Try adding "I'll tip $X for a better solution" to encourage more effort

## Common Patterns to Use

1. **For problem-solving**: "Think through this step-by-step and explain your reasoning"
2. **For writing**: "Write in the style of [author/publication] about [topic]"
3. **For creativity**: "Generate 5 unique ideas for [goal] that incorporate [constraint]"
4. **For analysis**: "Analyze the following text and identify the main themes, supporting evidence, and any logical fallacies"
5. **For refinement**: "Here's my first draft. Please improve it by [specific improvements]"

## When Things Go Wrong

- If the response is factually wrong, provide correct information as context
- If the model misunderstands, clarify your request with more specific instructions
- If output quality is poor, try specifying evaluation criteria ("A good answer will include...")
- If the answer is incomplete, ask follow-up questions

Remember: The models can't read your mind - be explicit about what you want!