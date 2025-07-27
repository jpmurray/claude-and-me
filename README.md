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

Choose one of the following installation methods:

#### Option 1: Use as Project Base

Clone this repository as the foundation for your new Laravel project:

```bash
git clone https://github.com/jpmurray/claude-and-me.git your-project-name
cd your-project-name
```

Then install Laravel within this directory or move your existing Laravel application files here.

#### Option 2: Copy to Existing Project

For existing Laravel projects, copy the necessary files from this repository to your project root:

```bash
# Clone temporarily
git clone https://github.com/jpmurray/claude-and-me.git temp-claude-tools

# Copy configuration files to your existing Laravel project
cp temp-claude-tools/mcp.json your-laravel-project/
cp temp-claude-tools/claude.md your-laravel-project/
cp -r temp-claude-tools/.claude your-laravel-project/

# Clean up
rm -rf temp-claude-tools
```

#### Install Dependencies

Install the required PHP development dependencies using Composer:

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
