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
- [variable-name-1]: [brief description]
- [variable-name-2]: [brief description]
- [additional-variables-as-needed]: [brief description]

# Aider Workflow Configuration
[Include this section only if using aider workflow]

## Commands
- [command-name-1]: [brief description]
- [command-name-2]: [brief description]

## Command-Directions
- [command-name-1]: [detailed explanation of what the command does]
- [command-name-2]: [detailed explanation of what the command does]

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
```

## Usage Notes:

1. **Purpose**
   - Must be clear and concise
   - Single sentence only
   - Should clearly state the goal

2. **Instructions**
   - Each instruction must end with a period
   - Be specific and actionable
   - List in order of execution

3. **Sections**
   - Use lowercase
   - Separate words with hyphens
   - Keep names concise and descriptive

4. **Variables**
   - Use lowercase
   - Separate words with hyphens
   - Include clear descriptions

5. **Aider Workflow (if used)**
   - Commands must start with #
   - First step must be "Request chat mode"
   - Last step must be "Save and summarize flow"
   - Total steps must be between 1 and 8
   - Each step must have a clear description

## Example:

```markdown
# Purpose
Create an implementation status analysis for prioritizing future sprint work based on current project state.

# Instructions
- Review provided requirements and current implementation status.
- Analyze completed, partial, and unimplemented features.
- Generate priority recommendations based on dependencies.
- Create a structured report with findings and recommendations.

# Sections
- overview
- completed-features
- partially-implemented-features
- not-implemented-features
- priority-recommendations

# Variables
- provided-requirements: Project requirements documentation
- provided-tech-stack: Current technology stack details
- provided-user-stories: List of user stories
- use-aider: true

# Aider Workflow Configuration

## Commands
- #analyze-impl: Main implementation analysis command
- #analyze-impl-status: Progress checking command

## Command-Directions
- #analyze-impl: Initiates or resumes the implementation analysis workflow
- #analyze-impl-status: Displays current progress and remaining steps

## Steps
4

## Steps-Description
1. Request chat mode
2. Load and validate requirements
3. Generate implementation analysis
4. Save and summarize flow
```