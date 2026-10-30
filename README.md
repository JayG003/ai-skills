# Personal AI Skills

A portable collection of reusable instructions for coding, learning, research, and development workflows.

## Design principles

- **Supplement, never replace:** These skills extend an assistant's capabilities. They must not disable or restrict native reasoning, tools, built-in skills, connectors, or other independently available capabilities.
- **Use the best tool:** Choose the most effective available capability for the task, whether native or provided by this repository.
- **Load selectively:** Read `INDEX.md`, identify relevant skills, and load only the files needed for the current task.
- **Progressive disclosure:** Start with a skill's description and load its full instructions only when relevant.
- **User intent comes first:** Follow the user's current request and explicit constraints, subject to applicable higher-priority safety requirements.
- **Be honest about access:** A repository URL in instructions does not automatically make its contents available. Retrieve the files through an actually available GitHub connection, file access, or by opening the repository in an environment that can read it. If retrieval fails, say so; do not pretend the skills were loaded.

## Repository map

- `INDEX.md` — skill catalogue and activation guide.
- `GLOBAL_RULES.md` — shared rules for using this repository.
- `coding/` — general coding philosophy.
- `programming/` — language and database guidance.
- `learning/` — study and technical research workflows.
- `workflows/` — debugging and code review procedures.

## Using this repository with ChatGPT

1. Connect the GitHub repository if a GitHub integration is available, or make the files accessible through an approved local-file workflow such as ChatGPT Work.
2. Keep a short Custom Instructions entry pointing to this repository and asking the assistant to retrieve relevant files before applying repository-specific skills.
3. At the beginning of a task, the assistant should inspect `INDEX.md`, then retrieve only the relevant `SKILL.md` files and `GLOBAL_RULES.md` when needed.
4. If the assistant cannot access the repository in the current chat or mode, provide the relevant file or use an environment with access. Do not assume ordinary ChatGPT chats automatically fetch GitHub files.

## Agent Skills format

Each skill is stored in its own directory with a `SKILL.md` file and YAML frontmatter containing `name` and `description`. The format is designed to be portable, but availability and automatic activation depend on the host application and its supported skill mechanism.
