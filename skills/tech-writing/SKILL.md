---
name: "tech-writing"
description: "Teaches the technical writing methodology from 'How to Write Technical Texts'. Invoke when user needs to write, review, or improve technical documentation, articles, tutorials, or code examples."
license: "CC-BY-NC-SA-4.0"
---

# Technical Writing Methodology

This skill distills the writing methodology proposed in *How to Write Technical Texts* (https://azat.io/en/blog/how-to-write-technical-texts).

## When to Invoke

- User asks to write or polish a technical article, document, tutorial, or blog post.
- User wants to review and improve an existing technical text.
- User asks how to make technical content clearer, more concise, or easier to understand.
- User includes code examples in a technical text and needs guidance on presenting them.

## Core Principle

A good technical text does more than transmit information. It makes complex ideas accessible and interesting to readers at different levels. Complex things can be explained simply.

## 1. General Rules

### 1.1 Narrative Style

- Keep the narrative relaxed and natural.
- **Do not** flirt, use memes, or tell jokes.
- In educational content, jokes distract from the material and annoy readers.

### 1.2 Avoid Verbal Nouns

- Verbal nouns bloat the text, remove action, and make it dry.
- Replace nouns that describe actions with the corresponding verbs.

| Avoid | Prefer |
|---|---|
| The developer is engaged in creating interfaces | The developer creates interfaces |
| TrackJS provides error tracking | TrackJS tracks errors |

**Rule:** Do not use verbal nouns.

### 1.3 Avoid the Passive Voice

- Passive voice increases reading friction and resembles official jargon.
- Active voice is more direct and clear.

| Avoid | Prefer |
|---|---|
| The Node.js version has been updated | We’ve updated Node.js |
| The interface was developed using Svelte | We developed the interface on Svelte |

**Rule:** Eliminate passive voice whenever possible.

### 1.4 Use the Imperative Mood

- The imperative mood adds momentum and tells the reader exactly what to do.
- Use it for instructions, manuals, and step-by-step guides.
- It also makes sentences shorter.

| Avoid | Prefer |
|---|---|
| A Vue project can be initialized using the following command: | Run the command to create a project with Vue: |

**Rule:** Use the imperative mood when giving instructions.

## 2. Structure

### 2.1 Paragraphs

- Divide the text into paragraphs.
- **One paragraph = one thought.**
- Start each paragraph with the main idea so readers immediately know what it is about.
- Remove anything unrelated to the paragraph's main idea.

### 2.2 Short Sentences

- Avoid long sentences.
- Everyday communication uses short sentences; technical text should feel close to spoken language.
- Separate each idea into its own sentence to reduce cognitive load.

### 2.3 Simplify Syntax

- Readers pause at every punctuation mark.
- The more commas a sentence has, the harder it is to read.
- If you run out of breath while reading a sentence aloud, it is too long.
- **Avoid:** participial phrases, parenthetical words, dashes, colons, and explanations in brackets.
- **Read the text aloud.** If you stumble, simplify it.

### 2.4 Headings and Lists

- Like code, technical text should be modular.
- Use subheadings and bulleted lists so readers can quickly find what they need.
- Good structure makes learning more efficient and enjoyable.

### 2.5 Writing the Introduction

- The introduction helps readers decide whether the article is worth their time.
- Answer three questions:
  1. What concept will the article introduce?
  2. What will the reader be able to do after reading it?
  3. Why is it necessary?

### 2.6 Writing the Conclusion

- The conclusion should summarize the material and give practical advice on how to use it.
- It may include references to additional materials for further study.
- It may express a personal opinion about the material.

## 3. Editing Guidelines

### 3.1 Accessibility

- Minimize terminology and abbreviations.
- Unfamiliar terms repel newcomers.
- If a complex term is necessary, explain it.
- If the explanation uses another unfamiliar term, explain that one too.
- Remember that readers have different levels of technical knowledge. Make the text accessible to everyone.
- Explain cause and effect. In technical texts it is important not only to show *how* something is done, but also *why* it matters.
- Do not over-explain trivial concepts.
- Beware of the [curse of knowledge](https://en.wikipedia.org/wiki/Curse_of_knowledge): experts often forget what it is like to be a beginner.

### 3.2 Concision

- Readers have limited time and want value quickly.
- Long introductions distract from the point and bore readers. Keep them short.
- Avoid phrases that disrupt the natural flow of the text:
  - "pay attention"
  - "it is worth mentioning"
  - "it is important to specify that"
- Get to the point as quickly as possible.

### 3.3 Brevity

- If the text can be shortened, shorten it.
- Avoid:
  - introductory words
  - participles
  - de-particles
  - passive voice
  - synonyms piled up in descriptions
- After writing, spend time editing and read the text aloud.
- Remove unnecessary words.

### 3.4 Objectivity

- Never give biased assessments.
- Remove vague language or support it with facts.

| Avoid | Prefer |
|---|---|
| TinyJS is a fast and lightweight state management library | TinyJS is a lightweight library (2 kB) for state management in React and Preact. Benchmarks: … |

### 3.5 Clearness

- Ambiguity confuses novice developers.
- Be unambiguous and direct.

| Avoid | Prefer |
|---|---|
| TypeScript offers strict typing, which can be useful for increasing code stability and reliability. | TypeScript provides strict typing to improve code stability. |

### 3.6 Avoid Subjective Evaluations

- Reject subjective evaluations; they undermine reader trust.
- Do not include biased or unfounded judgments.
- Any evaluative claim must be accompanied by evidence.

**Examples to avoid:**
- React is by far the best framework out there.
- Everyone knows what OOP is.

### 3.7 Visualization

- Diagrams, schemes, screenshots, and code samples help readers understand technical details.
- Visual material is easier to read than plain text.
- If something can be shown with a code sample, do not describe it only with words.

## 4. Code Examples

### 4.1 Variable Names

- Code examples should not be detached from reality.
- **Avoid `foo` and `bar`.**
- Expressive names let you write code without comments.
- For objects or primitives, use a noun:
  - `user`
  - `age`
- For arrays, use a plural noun:
  - `users`
- Function names must begin with a verb:
  - `getUserInfo()`
  - `downloadCSV()`
- For event handlers, use the `on` or `handle` prefix:
  - `onSubmit`
  - `handleNameChange`
- Boolean values usually begin with `is` or `has`:
  - `isAdmin`
  - `hasValue`
- Never use magic numbers.

| Avoid | Prefer |
|---|---|
| `let blockSize = 20 * 8` | `let elementWidth = 20`<br>`let numberOfElements = 8`<br>`let blockSize = elementWidth * numberOfElements` |

### 4.2 Imports

- When using code from a module for the first time, show the import statement.
- Otherwise readers will copy the code and be surprised when it does not work.

### 4.3 Simplicity

- Code examples make the text practical and useful.
- When explaining a complex concept, start with a simple example and gradually add details or functionality.
- Keep code clear and simple. Complex designs intimidate readers.
- If a sample is still large or complex, add comments and explain how it works in the text.
- **Note:** Code comments do not replace the surrounding text.

### 4.4 Commands

- After showing a terminal command, always show the expected result.
- Example: after installing Node.js, show the output of `node -v`.

### 4.5 Anti-patterns

- If the text includes examples of code not to write, highlight them explicitly.
- Example: a condition that causes an infinite loop.

### 4.6 Relevance

- Regularly update published texts.
- Technology changes quickly, so content should stay current.
- Make sure code samples actually work.
- Nothing is more frustrating than broken, irrelevant, or outdated code examples.

## 5. Editing Workflow

1. After finishing a draft, spend time editing.
2. Read the text aloud.
3. Check for:
   - verbal nouns
   - passive voice
   - long sentences
   - complex syntax
   - subjective evaluations
   - unexplained terms
   - unnecessary words
4. Verify that code examples run correctly.
5. Ask colleagues or friends to review and give feedback.
6. Proofread carefully before publishing.

## 6. Response Format

When this skill is invoked, respond according to the request type:

1. **Writing request:** Start by identifying the target audience and the three introduction questions, then generate content following the structural guidelines.
2. **Review request:** Walk through the rules above, identify issues, and provide Before/After revision suggestions.
3. **Improvement request:** Prioritize accessibility, concision, objectivity, and clearness, then check code examples.
