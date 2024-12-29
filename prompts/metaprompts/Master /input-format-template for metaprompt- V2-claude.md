# Metaprompt Input Format Template

```markdown
# Purpose
[Clear statement of what you want to achieve in a single sentence]

# Instructions
- [Instruction 1 ending with a period.]
- [Instruction 2 ending with a period.]
- [Additional instructions as needed, each ending with a period.]

# Sections
- [section-name-1]
- [section-name-2]
- [additional-sections-as-needed]

# Variables
- [[variable-name-1]]: [brief description]
- [[variable-name-2]]: [brief description]
- [[additional-variables-as-needed]]: [brief description]

# Aider Workflow Configuration
[Include this section only if using aider workflow]

## Commands
- Pattern: S{X}.{Y}
- Format: #command-name

## Document-Requirements
- Content-Match: Story S{X}.{Y}

## Command-Directions
- #command-name-1: [detailed explanation of what the command does]
- #command-name-2: [detailed explanation of what the command does]

## Steps
[Number between 1-8]

## Steps-Description
1. Request chat mode
2. [Description of step 2]
3. [Description of step 3]
...
N. Save and summarize flow

# Examples
[Optional: Include examples of expected input/output]