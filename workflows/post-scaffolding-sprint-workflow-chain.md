# Post-Scaffolding Sprint Workflow Chain: AI-Assisted Planning and Implementation

## Overview

This workflow represents a chained sequence of AI-assisted processes for planning and implementing new features. Each phase produces specific outputs that become required inputs for subsequent phases, creating a connected chain of development activities.

The workflow operates through three sequential phases:
```
Phase 1: Implementation Analysis
↓ [Outputs feed Phase 2]
Phase 2: Sprint Story Generation
↓ [Outputs feed Phase 3]
Phase 3: Story Implementation
```

## Input/Output Chain

### Phase 1: Implementation Status Analysis (#analyze-impl)
**Initial Inputs Required:**
- Project requirements list
- Current user stories
- Core technology stack information

**Key Outputs → [Feed into Phase 2]:**
- Implementation status report documenting:
  - Completed features with supporting evidence
  - Partially implemented features with progress details
  - Not yet implemented features
- Prioritized feature list ordered by dependencies
- Technical dependency mapping

### Phase 2: Sprint Story Generation (#generate-sprint-stories)
**Required Inputs (including Phase 1 outputs):**
- Implementation status report (from Phase 1)
- Prioritized feature list (from Phase 1)
- Technical dependency mapping (from Phase 1)
- Previous sprint stories
- Sprint number
- Technology stack details

**Key Outputs → [Feed into Phase 3]:**
- Technical dependency analysis
- Set of well-formed user stories, each with:
  - Story identifier (S<X.Y>)
  - Acceptance criteria
  - Technical dependencies
  - Developer notes
  - Implementation considerations

### Phase 3: Story Implementation (#implement-story)
**Required Inputs (including Phase 2 outputs):**
- User stories with identifiers (from Phase 2)
- Technical dependency analysis (from Phase 2)
- Implementation considerations (from Phase 2)
- Project technical requirements
- Current dependencies list

**Key Outputs:**
- Implemented features meeting acceptance criteria
- Updated dependency list
- Verified working increments

## Workflow Chain Execution

### Starting the Chain

1. **Initiate Analysis:**
   ```
   #analyze-impl
   ```
   - Ensure all Phase 1 inputs are available
   - Wait for complete analysis before proceeding

2. **Generate Stories:**
   ```
   #generate-sprint-stories
   ```
   - Must have all Phase 1 outputs available
   - Proceeds only when analysis outputs are complete

3. **Implement Stories:**
   ```
   #implement-story S<X.Y>
   ```
   - Requires complete story generation outputs
   - Execute for each story in sequence

### Progress Tracking
Monitor chain progress using status commands:
```
#analyze-impl-status
#generate-sprint-stories-status
#implement-story-status
```

### Chain Dependencies

```
Implementation Analysis
└── Outputs required for Story Generation:
    ├── Implementation status report
    ├── Feature priorities
    └── Technical dependencies
    └── Story Generation
        └── Outputs required for Story Implementation:
            ├── User stories
            ├── Technical analysis
            └── Implementation considerations
```

## Maintaining Chain Integrity

### Verification Points
Each phase has specific verification points where the chain integrity must be confirmed:

1. **Analysis → Story Generation**
   - Verify implementation status report is complete
   - Confirm all features are properly prioritized
   - Validate technical dependency mapping

2. **Story Generation → Implementation**
   - Verify all stories have required components
   - Confirm technical dependencies are properly mapped
   - Validate acceptance criteria are testable

### Chain Break Prevention

To maintain workflow integrity:
1. Never skip phases or assume outputs
2. Verify all outputs before proceeding to next phase
3. Keep all documentation updated as you progress
4. Use status commands to confirm current state
5. Don't proceed if required inputs are missing

## Best Practices for Chain Execution

1. **Document Management**
   - Keep all phase outputs in accessible locations
   - Document any modifications to outputs
   - Version control all artifacts

2. **Phase Transitions**
   - Explicitly verify all required outputs exist
   - Validate output quality before proceeding
   - Document any assumptions or decisions

3. **Dependency Handling**
   - Track both technical and workflow dependencies
   - Verify dependency satisfaction at each step
   - Document any dependency changes

## Using the Workflow Chain

1. **Preparation**
   - Gather all initial inputs
   - Verify input completeness
   - Set up documentation structure

2. **Execution**
   - Follow the chain sequence strictly
   - Verify outputs at each step
   - Maintain documentation of progress

3. **Verification**
   - Use status commands frequently
   - Verify chain integrity at each phase
   - Document completion of each phase

## AI Integration Notes

This workflow chain has been tested with:
- AI Assistant: aider
- LLM: Claude 3.5 Sonnet (October 22, 2024 release)

The chain assumes:
- AI can handle file operations
- Developer verifies all outputs
- Each phase completes fully before chain proceeds

## Chain Verification

Before starting each phase, verify:
1. All required inputs are available
2. Previous phase outputs are complete
3. All dependencies are satisfied
4. Documentation is current

Remember: The strength of this workflow lies in its chained nature. Each phase builds upon the outputs of the previous phase, creating a comprehensive and connected development process.
