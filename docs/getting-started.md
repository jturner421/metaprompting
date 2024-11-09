# Getting Started with AI-Assisted Development Prompts

This library provides a comprehensive, systematic approach to AI-assisted software development through:
1. Modular, task-specific prompts
2. Interconnected workflow chains that guide the development process

## Project Structure

```
project-root/
├── docs/                   # Project documentation
├── prompts/                # AI prompt library
│   ├── architecture/       # System design prompts
│   ├── code-analysis/      # Code health and review prompts
│   ├── coding/             # Implementation prompts
│   ├── documentation/      # Documentation generation prompts
│   ├── learning/           # Project understanding prompts
│   ├── maintenance/        # Project maintenance prompts
│   ├── planning/           # Project planning prompts
│   ├── requirements/       # Requirements analysis prompts
│   └── testing/            # Testing and validation prompts
└── workflows/              # Workflow chain definitions
    ├── general/            # Generic workflow templates
    └── assistant-specific/ # AI assistant-specific workflows
        └── aider/          # Workflows for specific AI assistants
```

## Prompt Types

Each prompt category contains two key files:
- `[prompt-name].md`: Detailed AI instruction set
- `[prompt-name].meta.md`: Metadata with usage guidelines, complexity, and compatibility information

## Workflow Chains

Our workflow chains provide a structured, step-by-step approach to development:

### Post-Scaffolding Sprint Workflow
1. **Implementation Status Analysis**
   - Assess current project state
   - Identify implemented and pending features

2. **Sprint Story Generation**
   - Create focused user stories
   - Prioritize based on technical dependencies

3. **Story Analysis**
   - Break down user stories into atomic steps
   - Define clear implementation criteria

4. **Story Implementation**
   - Carefully implement each story step
   - Ensure all requirements are met

## Development Approaches

### New Project Initialization
- Generate initial requirements
- Select technology stack
- Create project scaffolding
- Follow initial sprint workflow

### Existing Project Enhancement
- Analyze current implementation status
- Generate stories for next sprint
- Implement features incrementally
- Maintain comprehensive documentation

## Best Practices

- Use status commands to track workflow progress
- Verify inputs and outputs at each workflow stage
- Maintain clear, atomic implementation steps
- Document all decisions and changes
- Leverage AI assistants with workflow-specific prompts

## Getting Started

1. Review the project structure
2. Explore available prompts and workflows
3. Choose the appropriate workflow for your development phase
4. Follow the systematic, step-by-step process
5. Continuously validate and document progress
