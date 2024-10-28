# Software Development Prompt Library

A collection of AI-powered prompts designed to streamline software development workflows. Each prompt is crafted to work directly with AI coding assistants, providing consistent guidance across different development phases.

## Core Features

- **Project Initialization**
  - Requirements generation and refinement
  - Technology stack selection with BOM
  - Architecture design
  - Project scaffolding

- **Development Support**
  - Feature story creation
  - Code health analysis
  - System visualization
  - Unit test generation

- **Documentation**
  - README generation
  - Code explanation and tutoring

## Using the Prompts

1. Navigate to the relevant prompt in `/prompts` directory
2. Share the raw URL with your AI assistant
3. Begin using the workflow

Each prompt has two components:
- `[prompt-name].md` - AI instructions
- `[prompt-name].meta.md` - Usage documentation

## Project Structure

```plaintext
software-dev-prompt-library/
├── prompts/
│   ├── architecture/
│   ├── documentation/
│   ├── planning/
│   ├── testing/
│   └── visualization/
├── workflows/
│   └── [workflow guides]
└── docs/
    ├── getting-started.md
    └── prompt-guidelines.md
```
## Key Benefits

- Streamlined development workflows from project inception to maintenance
- Intelligent adaptation to different programming languages and frameworks
- Focused, single-purpose prompts that chain together for complex tasks
- Built-in validation and best practices
- Promotes consistent development patterns across teams
- Reduces cognitive load during development tasks
- Enables rapid prototyping and iteration

## Getting Started

1. Review [getting-started.md](docs/getting-started.md) to understand available workflows
2. Choose your starting point:
   - New project? Start with requirements generation
   - Existing project? Begin with code health analysis
3. Follow the workflow guides for your chosen development path
4. Chain prompts together as needed for more complex tasks

## Contributing

1. Review [prompt-guidelines.md](docs/prompt-guidelines.md) for prompt structure and principles
2. Each prompt needs both implementation (.md) and documentation (.meta.md)
3. Test prompts across different AI models and project types
4. Submit additions that focus on specific development tasks
5. Maintain language and framework agnosticism
