# Getting Started with Software Development Prompts

This library provides two complementary approaches to AI-assisted development:
1. Individual prompts for specific tasks
2. Workflow chains that connect multiple prompts in a systematic process

## Using Individual Prompts

1. Navigate to the relevant prompt category in `/prompts`:
   - architecture/ - System design and tech stack
   - coding/ - Implementation and development
   - documentation/ - Docs and diagrams
   - requirements/ - Project planning
   - testing/ - Test generation and validation

2. Each prompt has two files:
   - `[prompt-name].md` - AI instructions
   - `[prompt-name].meta.md` - Usage documentation

3. Share the prompt URL with your AI assistant and begin working

## Using Workflow Chains

1. Review available workflows in `/workflows`
2. Choose a workflow that matches your development phase
3. Follow the chain sequence:
   - Verify required inputs
   - Execute each phase
   - Validate outputs
   - Track progress with status commands

## Available Features

### Project Initialization
- Requirements generation and revision
- Technology stack selection with BOM
- Architecture design
- Project scaffolding

### Development
- Feature story generation
- Code health analysis
- System visualization with PlantUML
- Comprehensive unit testing

### Documentation
- README generation
- Code explanation and tutoring

## Getting Started

1. For a new project:
   - Start with requirements generation
   - Move to tech stack selection
   - Follow the scaffolding workflow

2. For an existing project:
   - Begin with code health analysis
   - Use the post-scaffolding workflow
   - Add features incrementally

3. For any project:
   - Review workflow documentation
   - Verify chain dependencies
   - Track progress systematically
