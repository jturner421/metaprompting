# Metaprompt Template User Guide

## Introduction
This guide explains how to format your input for the metaprompt template. The template is designed to structure your requirements into a format that Language Models (LLMs) can consistently process.

## Input Format Structure

Your input should follow this structure:

```
Purpose: [Clear statement of what you want to achieve]
Instructions: [List of specific instructions, separated by periods]
Sections: [Required sections in the output]
Variables: [List of variables needed]
Commands: [Specific commands for aider workflow, if needed]
Command-Directions: [Explanations of what commands do in aider workflow]
Steps: [Number of steps in aider workflow (1-8)]
Steps-Description: [Description of what each step will do]
```

## Step-by-Step Guide

### 1. Define Your Purpose
Write a clear, single sentence that describes what you want to achieve.

Example:
```
Purpose: Create the implementation status analyses that guides prioritization of future sprints based on current implementation status and requirements.
```

### 2. List Your Instructions
Write out specific instructions, each ending with a period.

Example:
```
Instructions:
    Based on the provided requirements, technology stack, and current set of user stories, generate an implementation status analysis.
    Include a clear analysis of completed, partially implemented, and not yet implemented features.
    Prioritize features based on technical dependencies and requirements.
    Maintain clear, structured output.
    Include a priority order for next implementation phase.
```

### 3. Specify Required Sections
The Sections field defines the structure of the output you want to receive. Each section should be:
- Written in lowercase
- Use hyphens between words
- Separated by commas

Required sections typically include:
- `overview` - High-level summary of the analysis or output
- `purpose` - The goal or objective being addressed
- `instructions` - Specific steps or guidelines
- `examples` - Sample inputs and outputs (if needed)
- `user-prompt` - Where user input will be processed
- `variables` - List of required inputs
- `workflow` - Steps in the process (if applicable)
- `output-format` - Desired format of the results

Example:
```
Sections: overview, completed-features, partially-implemented-features, not-yet-implemented-features, priority-order-for-next-implementation-phase
```

### 4. Define Variables
Variables are placeholders for information that will be provided either by the user or system. Each variable should be:
- Written in lowercase
- Use hyphens between words
- Listed with their specific purpose

Common variables include:
- `user-input`: The primary text or request from the user
- `provided-requirements`: Specific requirements or specifications
- `provided-tech-stack`: Technology stack information
- `provided-user-stories`: User stories or requirements
- `user-prompt`: The formatted input template
- `use-aider`: Boolean flag for enabling Aider workflow

Example:
```
Variables: user-input, provided-requirements, provided-tech-stack, provided-user-stories, user-prompt, use-aider
```

### 5. Defining Steps for Aider Workflow
When using the aider workflow, you must specify:

1. Number of Steps (1-8):
```
Steps: 4
```

2. Description of each step's action:
```
Steps-Description:
1. Request chat mode
2. Load and validate requirements
3. Generate implementation analysis
4. Save and summarize flow
```

Note: 
- Step 1 must always be "Request chat mode"
- The last step must always be "Save and summarize flow"

### 6. Commands for Aider Workflow
If your prompt uses aider workflow, specify the required commands.

Example:
```
Commands: #analyze-impl, #analyze-impl-status
```

### 7. Explain Aider Workflow Commands
Provide clear directions for what each command does in the aider workflow.

Example:
```
Command-Directions: #analyze-impl: Starts or resumes implementation analysis. #analyze-impl-status: Shows current progress in analysis workflow.
```

## Usage Tips

1. **Keep It Structured**
   - Use the exact section headings shown above
   - Maintain consistent formatting
   - Separate sections with line breaks for readability

2. **Be Specific**
   - Write clear, actionable instructions
   - List all required sections
   - Define all variables that will be used

3. **Common Mistakes to Avoid**
   - Don't skip required sections
   - Don't use different section names than specified
   - Don't forget to separate instructions with periods
   - Don't forget to make first step "Request chat mode"
   - Don't forget to make last step "Save and summarize flow"

## Final Checklist

Before submitting your input, verify:
- [ ] Purpose is clearly stated in one sentence
- [ ] Instructions are complete and end with periods
- [ ] All required sections are listed
- [ ] All necessary variables are defined
- [ ] Commands and their directions are included (if using aider workflow)
- [ ] Steps are between 1 and 8
- [ ] First step is "Request chat mode"
- [ ] Last step is "Save and summarize flow"
- [ ] Format matches the template structure