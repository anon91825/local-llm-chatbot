# Local LLM Chatbot - CS1 Assignment

## Summary

The Local LLM Chatbot assignment introduces students to the fundamentals of programming with Large Language Models (LLMs) in a lightweight, privacy-preserving environment. Students build an interactive chatbot using a real LLM running locally in their browser, implementing conversation memory and exploring AI behaviors. The assignment emphasizes critical AI literacy by encouraging students to analyze and critique the limitations of LLMs. Designed for CS1 or early CS2 students, the assignment takes approximately 2-3 hours to complete and provides a mix of technical and conceptual challenges. Starter code and detailed instructions are provided to ensure accessibility.

While all the assignment resources are provided in the bundled zip file, we believe what makes this assignment truly **nifty** is its zero-cost, one-click setup infrastructure.  To demonstrate this, please visit the fully anonymized github repo: https://github.com/anon91825/local-llm-chatbot

A quick start video is also included in the zip file to help students get started quickly.

### What is the Local LLM Chatbot assignment?

The Local LLM Chatbot assignment provides students with an opportunity to create and experiment with a chatbot powered by a small, open-source LLM. Students implement conversation memory using Python data structures such as lists and dictionaries, while exploring the probabilistic and context-dependent nature of AI systems. The assignment is designed to be accessible, requiring only basic Python knowledge, and runs entirely in the browser using GitHub Codespaces, eliminating the need for complex installations.

### What makes the Local LLM Chatbot assignment great?

Unlike traditional programming assignments, the Local LLM Chatbot assignment immerses students in the world of AI by allowing them to interact with and modify a working chatbot. The assignment fosters engagement by providing hands-on experience with real AI systems, enabling students to:

- Discover the strengths and limitations of LLMs through direct experimentation.
- Develop critical thinking skills by analyzing AI behaviors and discussing their implications.
- Learn programming concepts in an authentic and motivating context.

The lightweight, browser-based platform ensures that students can focus on learning without being hindered by technical barriers. Additionally, the assignment encourages creativity by allowing students to extend the chatbot with new features, such as custom personalities or conversation summarization.

### How is the Local LLM Chatbot assignment structured?

The assignment consists of a single main.py file consisting basic chatbot scallfoldding code.  Thru a series of steps of increasing difficult, students refine their chatbot and explore ideas such as LLM memory, bias, and context engineering.

#### Part 1: Basic Chatbot (30 minutes)
Students create a simple chat loop using the provided `chat()` function:

```python
while True:
    user_input = input("You: ")
    response = chat(user_input)
    print("Bot:", response)
```

#### Part 2: Memory System (45 minutes)
Students implement conversation memory using lists and dictionaries. While the primary learning objectives are squarely on practicing with nested data structures, a secondary learning objective can be achieved as students are exposed to LLM concepts such as memory and context.

#### Part 3: Enhanced Features (30 minutes)
Students explores the nature of LLMs and prompt engineering by "planting memories" into a model.  This part is also where students can be creative and reflective on the nature of LLMs.

### Files and Resources

The assignment includes the following files:

- **Read-Only files:** `chat.py` contains several functions to simplify interaction with the local LLM.  For this assignment, they simply need to include the `chat()` function via 
```
import chat from chat
```

- **Support files:** Pre-configured environment files for GitHub Codespaces, i.e. everything in the `.devcontainer` directory including `devcontainer.json`, setup scripts, and pre-compiled binary code for the inference engine targeted for deployment in Github Codespaces

- **Starter code:** `main.py` provides starter code and is the only file students are expected to modify

- **Auto testing:**: `test_assignment.py` provides auto-grading.  Students can check if they have completed the assignment by calling `pytest` on the command line.

### Why this assignment matters

As AI becomes increasingly prevalent, it is essential for students to develop both technical skills and critical perspectives on these systems. The Local LLM Chatbot assignment achieves this by:

- Providing hands-on experience with real AI systems in a controlled, privacy-preserving environment.
- Encouraging students to think critically about the reliability, bias, and transparency of AI.
- Bridging the gap between theoretical knowledge and practical application.

This assignment equips students with the tools they need to navigate and contribute to the evolving field of AI.

---

## Topics

A practical application of lists, dictionaries, loops, and conditional logic in the context of AI interaction and conversation management.

---

## Audience

Appropriate for late CS1 or early CS2 students with basic knowledge of Python data structures.

---

## Difficulty

This is an intermediate assignment, taking approximately 2-3 hours for CS1 students to complete all parts.

---

## Strengths

Students are immediately engaged by building their own AI chatbot that actually works. The assignment naturally leads to discovery moments about AI limitations (like poor math skills) that spark genuine curiosity. The one-click setup eliminates technical barriers, works free at any scale, and students can experiment without cost concerns. Programming concepts are learned in an authentic, motivating context.

---

## Weaknesses

The underlying LLM behavior can be unpredictable, which may confuse some students initially. The small model sometimes produces inconsistent outputs that require instructor explanation. Students may become more focused on the AI novelty than the programming fundamentals being taught.

---

## Dependencies

Requires basic Python programming knowledge (variables, functions, input/output). Students need a GitHub account for Codespaces access. No prior AI or machine learning knowledge required. The assignment works entirely in a web browser with no local installation needed.

---

## Variants

The assignment can be extended in a varitey of ways.  Below are some ideas:

  - Implement selectable personalities by having multiple pre-build memories
  - Load personality from disk (Practice File IO)
  - Experiment the `chat()`'s temperature parameter to control randomness of response
  - Additional attempt to "jailbreak" the model via different prompt engineering techniques
  - Have multiple chatbots interact with each other programmatically

