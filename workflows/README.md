# AI Workflow Chains

This directory contains documented AI-assisted workflow chains that enable systematic, repeatable development processes through carefully sequenced prompts.

## What are Workflow Chains?

Workflow chains are structured sequences of AI prompts where each phase:
- Requires specific inputs
- Produces well-defined outputs
- Feeds those outputs as inputs to subsequent phases
- Maintains clear dependencies between phases
- Includes verification points to ensure chain integrity

This chained approach ensures:
- Consistent, repeatable processes
- Clear dependencies between development phases
- Proper validation at each step
- Traceable development progress
- Maintainable documentation

## Available Workflows

### [Post-Scaffolding Sprint Workflow](post-scaffolding-sprint-workflow-chain.md)
A three-phase workflow for planning and implementing new features:
1. Implementation Analysis - Assesses current feature status
2. Sprint Story Generation - Creates well-formed user stories
3. Story Implementation - Systematically implements stories

Each phase builds on the outputs of previous phases, creating a connected chain of development activities.

## Using Workflow Chains

1. Review the workflow documentation to understand:
   - Required inputs for each phase
   - Expected outputs
   - Verification points
   - Chain dependencies

2. Follow the chain sequence strictly:
   - Verify all required inputs are available
   - Complete each phase fully before proceeding
   - Validate outputs at each step
   - Maintain documentation of progress

3. Use provided commands to:
   - Initiate each phase
   - Check phase status
   - Verify chain integrity

More workflows coming soon!
