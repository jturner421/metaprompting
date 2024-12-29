# Metaprompt Input Format Template

```markdown
# Purpose
[Single sentence clearly stating the prompt's goal]

# Instructions
- [Each instruction must end with a period.]
- [Instructions should be clear and actionable.]
- [List all required steps in sequence.]

# Sections 
[Required sections in lowercase, hyphenated format]
- overview
- purpose
- instructions
- examples (optional)
- user-prompt
- variables
[If section name is plural, include exactly 3 singular items]

# Variables
[Use format [[variable-name]]]
- [[user-input]]: Primary input text
- [[provided-requirements]]: Project requirements
- [[provided-tech-stack]]: Technology stack details
[Add other variables as needed]

# Commands
- Pattern: S{X}.{Y}
- Format: #command-name

# Document-Requirements
- Content-Match: Story S{X}.{Y}
[Additional patterns as needed]

# Command-Directions
[For each command, explain its purpose and usage]
- #command-1: [Detailed explanation]
- #command-2: [Detailed explanation]

# Steps
[Number between 1-8]

# Steps-Description
1. Request chat mode
2. [Step description]
...
N. Save and summarize flow

# Examples
[Optional: Show input/output examples]