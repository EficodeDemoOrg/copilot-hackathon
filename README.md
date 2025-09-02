# 🚀 Copilot Hackathon

Assignments for the GitHub Copilot hackathon

## 📚 Exercise Repositories

Choose one of the following three options:

- [Copilot Data Analysis Exercise](https://github.com/EficodeDemoOrg/copilot-data-analysis-exercise)
- [Copilot Backend Exercise](https://github.com/EficodeDemoOrg/copilot-backend-requirement-exercise)
- [Copilot Fullstack Exercise](https://github.com/EficodeDemoOrg/copilot-fullstack-exercise)

DB Admins, test automation engineers, IaC engineers and other non-developers: come up with your own project idea. If needed, use Copilot to ideate.

## 📋 Instructions

- The objective is to implement an application according to the requirements.
- Use the advanced features discussed during the first part of the workshop as much as possible
- Divide the work between the members or use mob programming
- The results of each group are reviewed and discussed at the end of the hackathon. Make notes during the exercise about what worked well with Copilot, what didn't!

The main objective of the exercise is not to solve a programming problem, but to put Copilot features to the test. During the exercise, remember to utilize as much as possible the features discussed in Workshop 1:

- Chat participants, Slash commands
- Ask, Edits and Agent mode, depending on the situation
- Custom instructions (for inspiration: [awesome-copilot](https://github.com/github/awesome-copilot/tree/main/instructions))
- MCP servers (e.g. Playwright for browser testing, Context7 for up-to-date docs)
- Generate unit and/or browser tests for the application using Copilot
- Try out different models
  - General purpose programming tasks: GPT-4.1 (GPT-4o is deprecated)
  - Deep reasoning and debugging: GPT-5, o3, Claude Sonnet 3.7 (Thinking) and 4

## ❌ The Don'ts of Using Copilot

- Do NOT vibe code, e.g. try to implement the app solely by relying on Copilot!
  - Key to using Copilot successfully is to retain the control and understand each line of code produced by the LLM
  - Giving complete control to Copilot will result in losing touch with the codebase
- Do NOT feed the entire backlog file to Copilot and ask it to implement all the requirements
  - Prompts with too wide a scope will often result in endless agentic iteration cycles that eventually result in an application that doesn't work

## ✅ The Do's of Using Copilot

- Begin by brainstorming with Copilot
  - Use Copilot to better understand the exercise assignment and its requirements
  - What should the architecture be like? What are the options?
  - Which framework / tech stack could we use for this?

- Use a project-specific custom instructions file
  - `.github/copilot-instructions.md`
  - Create one before doing anything else
  - Make a simple one initially, keep updating as your understanding of the project increases
  - Add a very high-level project description, preferred tools and frameworks and most important coding conventions to the initial version

- Let Copilot help you in initializing the project
  - How do I initialize the project using the framework of my choice? For consistent and standard results, it's better to use tools like create-react-app, Maven, etc. rather than let Copilot scaffold the project.
  - Which unit testing framework could I use for the project?
  - Ask Copilot to create a stub test case and test that it's runnable

- Progress iteratively
  - Even when using the agent mode, progress in small steps
  - Implement e.g. a REST API stub or an empty page first
  - Add one REST API endpoint, UI component (e.g. a form) etc at a time
  - Go through the changed lines and see that they make sense
  - Ask Copilot to explain parts of the code that you don't understand
  - If the implementation offered by Copilot isn't satisfactory, explain why and ask it to iterate on the solution
  - Accept the solution when you're satisfied with it. Commit often.
  - Generate and update unit tests after each change

- Try Test Driven Development with Copilot Agent Mode
  - If you're using VS Code, create a custom chat mode that
  - Describe a change / feature to Copilot
  - Ask it to implement unit tests only for the change
  - Ask Copilot to implement just enough code to make all the tests pass using TDD approach
  - Adjust your prompt if Copilot doesn't understand that it's supposed to run the tests automatically in order

- Try using MCP servers
  - E.g. Playwright MCP if you're doing web development
  - PostgreSQL MCP if you have a local PostgreSQL database
  - Context7 if working with a very recent version of a framework/tool
