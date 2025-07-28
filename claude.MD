## Project Context & Tech Stack

You are working with a Laravel full-stack developer on the "$PROJECT_NAME" project. This is a Laravel application using:

- **Framework**: Laravel (latest version)
- **Frontend Stack**: Livewire + Livewire Flux + Alpine.js + Tailwind CSS
- **Database**: Sqlite
- **Development Focus**: Full-stack Laravel development with modern frontend tools

The project is always running `npm run dev` with Laravel Valet, and so the latest version of the project is always accessible at "$PROJECT_URL".

## Developer Preferences & Coding Style

### Domain Glossary (Claude, learn these!)

- **Agent**: AI entity with memory, tools, and defined behavior
- **Coder**: The human interacting with agents
- **Task**: Workflow definition composed of steps (NOT a Celery task)
- **Execution**: Running instance of a task
- **Tool**: Function an agent can call (browser, API, etc.)
- **Session**: Conversation context with memory
- **Entry**: Single interaction within a session

### How to interact with the coder

- Always be brief, save tokens, trust the coder's knowledge and don't try to praise them when speaking to them.
- When unsure about implementation details, ALWAYS ask the coder.
- Always work by doing a tasks, iterate through the task's steps to do your work _then_ after you are done with a task, ask the user if you can write to the change log and commit the changes or if there's anything else to do.
- After a task is done, remind the coder they might want to start a new session with you.

### What AI Must NEVER Do

1. **Never modify test files** - Tests encode human intent
2. **Never commit secrets** - Use environment variables
3. **Never assume business logic** - Always ask

Remember: We optimize for maintainability over cleverness. When in doubt, choose the boring solution.

# General development principles

Read @.claude/code-guidelines/tdd.md for my preferences.

### Laravel Best Practices

Read @.claude/code-guidelines/PHP.md for my preferences.

### Livewire Development

Read @.claude/code-guidelines/livewire.md for my preferences.

### Frontend Development

Read @.claude/code-guidelines/frontend.md for my preferences.

### Writing tests

Read @.claude/code-guidelines/tests.md for my preferences.

### Using basic-memory

Read @.claude/code-guidelines/basic-memory.md for my preferences.

## Available Tools

You have access to the following MCP servers:

- **Context7**: Access latest Laravel, Livewire, Livewire's Flux documentation and any other framework docs
- **sqlite**: Query and modify the SQLite database directly for data analysis and management
- **basic-memory**: Remember project decisions, patterns, and maintain context across sessions
- **GitHub**: Manage repository operations, issues, pull requests, and workflows
- **Playwright**: Browser automation to test and interact with the live site at boundaries.fyi.test
- **Filesystem**: File system operations within the project directory structure
- **Git**: Local git repository management following Gitflow branching strategy

Use these tools actively to understand the project structure, run commands, and maintain context across sessions.
