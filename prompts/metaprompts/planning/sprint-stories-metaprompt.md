# Purpose
Create focused user stories for the next sprint by analyzing project state, technical dependencies, and implementation priorities while ensuring proper documentation and workflow.

# Instructions
- Validate presence of all required project context documents including requirements, previous sprint stories, implementation status, and tech stack.
- Analyze technical dependencies between features.
- Generate properly formatted user stories based on implementation priorities.
- Maintain consistent story ID formatting and structure.
- Ensure proper file saving workflow.
- Track progress through story generation process.

# Sections
- project-context-validation
- technical-dependency-analysis
- story-generation
- story-review
- file-management
- progress-tracking

# Variables
- sprint-number: Current sprint number for story generation
- previous-sprint-file: Path to previous sprint's stories file
- requirements-file: Path to project requirements document
- implementation-status-file: Path to implementation status report
- tech-stack-file: Path to technology stack information
- output-directory: Directory for saving generated stories
- output-filename: Filename for saving generated stories
- story-prefix: Sprint story ID prefix (e.g., "S2" for Sprint 2)

# Aider Workflow Configuration

## Commands
- #generate-sprint-stories: Main story generation command
- #generate-sprint-stories-status: Progress checking command

## Command-Directions
- #generate-sprint-stories: Initiates or resumes the sprint story generation workflow
- #generate-sprint-stories-status: Displays current progress in story generation workflow with completed, current, and remaining steps

## Steps
6

## Steps-Description
1. Request chat mode
2. Validate project context documents
3. Obtain sprint number and perform technical analysis
4. Generate user stories with proper formatting
5. Review and revise stories based on feedback
6. Save and summarize flow

# Examples

## Example Project Context Validation
```
I have found in the context:
✓ Requirements list in requirements.md
✓ Previous sprint stories in sprint_2_stories.md
✓ Implementation status in implementation_status.md
✓ Technology stack identified:
  - Vue.js 3.3.4
  - Vuetify 3.3.15
  - Vue Router 4.2.4
  - Pinia 2.1.6
```

## Example Technical Analysis
```
Technical Dependency Analysis:
1. Entry Creation Form (Priority 1)
   - No dependencies, ready for implementation
   - Relevant tech: Vue.js, Vuetify, VeeValidate
2. Local Storage Setup (Priority 1)
   - No dependencies, ready for implementation
   - Relevant tech: Pinia for state management
3. Entry Listing (Priority 2)
   - Depends on: Entry Creation Form, Local Storage
   - Relevant tech: Vue Router, Vuetify data tables
```

## Example Story Format
```
Story S2.1: Set up Local Storage
As a developer, I want to implement local storage functionality so that journal entries can be persisted between sessions.

Acceptance Criteria:
- Local storage service is implemented
- Basic CRUD operations are tested
- Error handling is in place

Dependencies: None

Developer Notes:
- Consider using Pinia for state management
- LocalStorage wrapper could be implemented as a Pinia plugin
- VeeValidate can help with data validation before storage
```