# Prompt Guidelines

## Core Principles

1. Direct AI Instructions
- Write prompts as clear directives to the AI
- Focus on process steps and expected outputs
- Exclude metadata and human-focused documentation

2. Separation of Concerns
- Keep prompt instructions in `.md` files
- Store usage documentation in `.meta.md` files
- Maintain clean separation between AI and human documentation

3. Prompt Structure
- Start with clear workflow name
- List steps in logical order
- Define output formats
- Include validation rules

4. Output Formats
- Use consistent markdown structures
- Include file paths in code blocks
- Separate command-line instructions
- Maintain clear formatting

5. Workflow Integration
- Design prompts to work together
- Allow for iteration and revision
- Support different development stages
- Enable flexible application types

## Best Practices

1. Keep prompts focused
- One primary task per prompt
- Clear scope boundaries
- Minimal complexity

2. Enable interaction
- Break complex decisions into steps
- Allow for user input and revision
- Provide clear options

3. Maintain context
- Reference existing project files
- Consider current development stage
- Check for conflicts and dependencies

4. Support validation
- Include quality checks
- Verify compatibility
- Confirm requirements alignment

## Testing Prompts

1. Verify prompt works across different AI models
2. Test with various project types and sizes
3. Confirm output consistency
4. Validate workflow integration
