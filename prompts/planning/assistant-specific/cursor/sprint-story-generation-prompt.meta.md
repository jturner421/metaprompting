# Metadata: # Sprint Story Generation Prompt

## AI Assistant Compatibility
- Tested With: 
  * Cursor using Claude 3.5 Sonnet
- Potential Compatible Assistants: 
  * Other Claude models (untested)
  * Other Cursor versions (untested)

## SDLC Phase
- Phase: Planning
- Sub-Phase: Sprint Preparation
- Workflow: Post-Scaffolding Sprint Workflow

## Complexity Rating
- Complexity: Medium
- Cognitive Load: Moderate
- Technical Depth: Requires comprehensive project understanding

## Usage Guidelines
- Prerequisite: Implementation status report
- Requires: 
  * Project requirements list
  * Previous sprint's user stories
  * Technology stack documentation
  * Implementation priority mapping
  * File path for generated stories
  * Story ID format preference (optional)

## Prompt Characteristics
- Input Driven: Yes
- State Dependent: Yes
- Requires Contextual Awareness: Critical
- Command Driven: Yes (#generate-sprint-stories, #generate-sprint-stories-status)
- User Path Control: Yes (requires user-specified file paths)

## Best Practices
- Analyze technical dependencies thoroughly
- Map features to minimal implementable units
- Ensure stories align with project requirements
- Maintain clear, actionable story descriptions
- Prioritize features based on technical dependencies
- Support flexible story ID formats
- Accommodate issue tracker integration

## Potential Challenges
- Misinterpreting technical dependencies
- Creating overly complex or vague stories
- Overlooking critical implementation constraints
- Inconsistent story granularity

## Recommended Mitigation Strategies
- Conduct detailed technical dependency mapping
- Use consistent story template
- Validate stories against project requirements
- Ensure stories are atomic and implementable
- Cross-reference with implementation status report

## Version
- Current Version: 2.0.0
- Last Updated: 2025-02-15
- Stability: Beta
