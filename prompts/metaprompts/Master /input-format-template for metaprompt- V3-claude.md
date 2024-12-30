# Metaprompt Input Format Template

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
- [[variable-name]]: [brief description]
- [[provided-requirements]]: Project requirements specification
- [[provided-tech-stack]]: Technology stack details
- [[provided-user-stories]]: User stories list
- [[step-mode]]: Required chat mode for the step
- [[step-action]]: Action for the current step
- [[step-prompt]]: Prompt for the current step

# Aider Workflow Configuration
[Include this section only if use-aider=true]

## Mode Control
- Architect Mode: [yes/no]
- Pre-review Required: [yes/no]

## Commands
- Pattern: S{X}.{Y}
- Format: #command-name
- Available Modes: [ask|architect|code]

## Command-Directions
- #command-name: [detailed explanation]
- #architect-review: [architectural validation details]
- #status: [progress tracking details]

## Validation Rules
- Success Criteria: [criteria for step completion]
- Failure Handling: [error management approach]

## Steps
[Number between 1-8]

## Steps-Description
1. Request chat mode
2. [Component Analysis]
3. [Implementation Details]
4. Save and summarize flow

# Examples
[Include example input/output demonstrating:
- Workflow commands
- Mode transitions
- Status checks
- Architecture reviews]
