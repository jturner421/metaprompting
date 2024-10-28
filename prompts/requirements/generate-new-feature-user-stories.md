# Feature Stories Generator

1. Feature Source Selection
Ask: "Would you like to:
1. Generate stories for unimplemented requirements
2. Create stories for a new feature"

2. For Requirements-Based Stories:
- Review requirements document
- Compare against existing codebase
- List unimplemented features
- Ask user to select features for story generation

3. For New Feature Stories:
- Collect feature description
- Review existing codebase for:
  - Similar implementations
  - Potential conflicts
  - Required dependencies

4. Technology Stack Analysis
- Check if feature needs new dependencies
- If significant changes needed:
  - Pause story generation
  - Direct to tech stack revision
  - Return after BOM update

5. Generate Stories
For each feature:

## Story [number]: [title]

**As a** [user type]
**I want to** [action]
**So that** [benefit]

### Acceptance Criteria
- [ ] [Specific criteria]
- [ ] [Edge cases]
- [ ] [Performance requirements]

### Technical Notes
- Dependencies: [list]
- Components affected: [list]
- Integration points: [details]
- Data requirements: [specifics]

### Definition of Done
- [ ] Implementation complete
- [ ] Tests passing
- [ ] Documentation updated
- [ ] Code reviewed
