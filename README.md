# Claude and Me

This repository provides a collection of tools and configurations to integrate Anthropic's Claude AI into a Laravel development workflow.

## Overview

The goal of this project is to streamline development by leveraging Claude's capabilities directly within your Laravel environment. It provides a pre-configured setup for common tools and a structure for project-specific context.

## Getting Started

Follow these instructions to get the environment set up.

### Prerequisites

- **Claude Configuration**: Ensure you have a `~/.claude.json` file. This file should contain your API keys and configurations for the following tools:
  - `playwright`
  - `github`
  - `context7`

### Installation

1.  **Add as a Git Submodule**: In your Laravel project's root directory, add this repository as a Git submodule. This keeps the tooling separate from your application code and makes it easy to receive updates.

    ```bash
    git submodule add https://github.com/jpmurray/claude-and-me.git
    git commit -m "Add claude-and-me submodule"
    ```

2.  **Install Dependencies**: Install the required PHP development dependencies using Composer.

    ```bash
    composer require --dev # None specific for now.
    ```

### Configuration

1.  **Configure the Memory Tool**: Add your project to the `basic-memory` tool. You have to edit `mcp.json` directly and run the following command (replace the placeholders with your project's actual name and path):

    ```bash
    basic-memory project add YOUR_PROJECT_NAME '~/PATH/YOUR_PROJECT_PATH/.memory'
    ```

2.  **Set Project Details**: Update the `claude.md` file with your project's specifics. This file is used to provide context to Claude. Replace these placeholders:
    - `$PROJECT_NAME`: Your project's name.
    - `$PROJECT_URL`: Your project's local development URL (e.g., `http://your-project.test`).

### Verify Your Setup

Run your Claude integration to check that all tools and configurations are loaded correctly. This will confirm that the previous steps were completed successfully.

## Usage

With the setup complete, you can now leverage the full power of Claude in your Laravel development. The pre-configured tools are ready to use.

Happy coding!
