# Local LLM Chatbot - CS1 Assignment

While all the assignment resources are provided in the bundled zip file, we believe what makes this assignment truly **nifty** is its zero-cost, one-click setup infrastructure.  To demonstrate this, please visit the fully anonymized github repo: https://github.com/anon91825/local-llm-chatbot

A quick start video is also included in the zip file to help students get started quickly.

## Summary

What makes the Local LLM Chatbot assignment nifty are two intertwined innovations:

  - One-click, zero-cost setup with GitHub Codespaces: Students can launch a pre-configured virtual environment in GitHub Codespaces that runs a local large language model (LLM) entirely within the cloud-based development container. Normally, enabling LLM inference requires complex installation steps or costly server-side infrastructure—both impractical in introductory courses. By bundling pre-compiled binaries and environment scripts, this assignment reduces setup to a single click, eliminating all technical barriers.

  - Authentic AI literacy through hands-on programming: As students interact with their chatbot, they quickly discover a fundamental property of LLMs—their stateless nature. Memory, learning, and context management must be implemented outside the model. This realization naturally leads to discussions about prompt engineering, context windows, and the limits of AI systems, all while practicing with core Python data structures like lists and dictionaries.

Together, these elements make the assignment engaging, accessible, and pedagogically powerful. Students not only implement and extend a working LLM-powered chatbot from the command line, but also confront the technical and conceptual realities of modern AI in a way that sparks curiosity and critical reflection—all within a 2–3 hour CS1-level exercise.

### Files and Resources

The assignment includes the following files:

  - `chat.py`: contains several functions to simplify interaction with the local LLM.  For this assignment, they simply need to include the `chat()` function via
    ```
    import chat from chat
    ```

  - `.devcontainer/`: Pre-configured environment files for GitHub Codespaces, contains setup scripts and pre-compiled binaries for the llama.cpp inference engine targeted for deployment in Github Codespaces

- `main.py`: provides starter code and is the only file students are expected to modify

- `test_assignment.py`: provides auto-grading.  Students can check if they have completed the assignment correctly by calling `pytest` in the terminal


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

Students need a working and reliable Internet connection a GitHub account for free Codespaces access. No prior AI or machine learning knowledge required. The assignment works entirely in a web browser with no local installation needed.

---

## Variants

This assignment can be extended in a varitey of ways.  Below are some ideas:

  - Implement selectable personalities by having multiple pre-build memories
  - Load personality from disk (Practice File IO)
  - Experiment the `chat()`'s temperature parameter to control randomness of response
  - Additional attempt to "jailbreak" the model via different prompt engineering techniques
  - Have multiple chatbots interact with each other programmatically

While the assignment itself is a simple exercise—a basic command line app with only a handful of lines of code—the true strength lies in the versatility of the platform. Once the infrastructure is in place, it can support a wide variety of LLM-based assignments. For example, it could be seamlessly adapted to projects like the “Infinite Story” nifty assignment from last year, or to new explorations of creativity, ethics, and AI capabilities.

