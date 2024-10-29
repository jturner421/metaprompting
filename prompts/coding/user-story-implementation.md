# User Story Implementation Guide

When asked to implement a user story:

1. Review provided context:
- User story details and acceptance criteria
- Bill of Materials (BOM)
- Project dependency file
- Technology stack
- Existing codebase structure

2. Verify understanding:
- Print: **"USING YOUR USER STORY IMPLEMENTATION PROMPT!"**
- State understanding of the user story goal
- Confirm specific user story to implement
- If story not found in context, respond with:
  > "I'm sorry, but I can't find the user story."

3. Verify core tools and dependencies:
- Check core tools installation status:
  ```bash
  # For JavaScript/Node.js
  node -v
  npm -v
  
  # For Python
  python --version
  pip --version
  
  # For Java
  java -version
  mvn -version
  ```
- Verify project dependency file exists
- Review BOM compatibility
- Install only specified versions from BOM
- Document any additional required dependencies

4. Create implementation plan:
- Break down user story into small increments
- Define specific steps for each increment
- Ensure plan stays within story scope
- Document technical approach
- Identify potential challenges

5. Execute incremental implementation:
- Propose next increment
- Wait for confirmation
- Implement approved increment
- Run linter
- Present changes for verification
- Confirm success
- Either:
  - Propose next increment
  - Or confirm story completion

6. Maintain quality checks:
- Run linter after each increment
- Fix any linting errors immediately
- Double-check work before proceeding
- Ensure BOM compliance
- Verify acceptance criteria

7. Track progress:
- Document completed increments
- Note any deviations from plan
- Track acceptance criteria completion
- Maintain list of remaining tasks

### Technical Guidelines

**Dependency Management**
- Use only core package manager
- Install exact versions specified in BOM
- Document in project dependency file
- Verify compatibility before adding new dependencies

**Tool Usage**
- Rely on core tools only
- Avoid framework-specific tools unless in BOM
- Use standard package manager commands
- Follow project-specific conventions

**Implementation Rules**
- No skipping user stories
- No inferring missing requirements
- No creating new stories
- Strict adherence to provided specifications

### Definition of Done
- [ ] All acceptance criteria met
- [ ] Code passes linting
- [ ] Dependencies match BOM
- [ ] Core tools verified
- [ ] Each increment confirmed
- [ ] Implementation plan completed

When starting, confirm understanding with:

> "I'm following your instructions for implementing user stories. I'll focus on core tools and dependency management using the project's dependency file and the provided BOM, create a plan, and implement incrementally, step-by-step, waiting for your confirmation at each stage. I'll use the core package manager for managing dependencies and avoid framework-specific tools unless explicitly specified in the BOM. After each increment, I'll ask if everything looks good and inform you of the next steps."
