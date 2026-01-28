# Human Scale Data

- Use bullet points or lists only when absolutely necessary.
- Avoid idioms. Write plainly and concisely.
- Do not abstract anything into a function unless it is used more than twice within the same document.
- Ask if you do not understand.

Always read the introdution (en/intro.qmd) in order to understand the philosophical outlook of this project.

Per the intro:

This book does not assume advanced Python or GIS knowledge. It aims to be an intensive course, not exhaustive, and provides resources for further exploration when possible. The goal of this work is not on mastering GIS programming but on providing replicable workflows that users can readily understand and apply in their own contexts to drive tangible municipal action.

## Output Style

- Do not narrate your thought process or describe what you're about to do.
- Do not announce each edit or tool use before executing it.
- Work quietly and report results when complete.
- Only output substantive information: completed work, findings, questions, or summaries.

## Agent Mode

When instructed to work "as" one of the following agents, read and follow the corresponding prompt from `.agents/`:

| Invocation | File |
|------------|------|
| "as translator" or "as Spanish to English translator" | `.agents/es-to-eng-translator.md` |
| "as instructor" or "as Python GIS instructor" | `.agents/pygis-instructor.md` |
| "as editor" or "as English editor" | `.agents/eng-copyeditor.md` |
| "as open data reviewer" or "as open data specialist" | `.agents/open-data-reviewer.md` |
| "as content reviewer" or "high-level content reviewer" | `.agents/content-reviewer.md` |
| "as climate risk expert" | | `.agents/climate-risk-expert.md` |
| as Robust Decision-Making Reviewer" | `.agents/rdm-expert.md` |

Read the agent file before responding. Follow its instructions for tone, output format, and review approach.

## Content Formatting

### Citations and References

Datasets must be cited the first time they appear in a .qmd file. All citations should be stored in references.bib.

### Terminology

Key terms should be bolded and defined inline the first time they appear in a .qmd file. When a term appears in multiple chapters, subsequent chapters should link back to where the term is first defined if necessary.

Tangential but important terms (such as "cloud," "categorical," or "continuous") should be defined in sidebars with the term in bold.

### Callouts

Use callouts to organize different types of information:

- **Tips**: Useful but not central information that arises in the workflow, such as troubleshooting CRS issues or types of helpful Python libraries
- **Important**: Critical information that readers must understand, such as guidance on working with local datasets
- **Sidebars**: Definitions of tangential but important terms

### Code Blocks

Analysis code should appear in non-folding code blocks. Visualization code should appear in folded code blocks unless the visualization code itself is essential to what we want to illustrate (it rarely is).

## Releases

When creating a new release:
1. Update CHANGELOG.md moving items from [Unreleased] to the new version section
2. Add the release date to the version section
3. Create a git tag with the version number (format: v*.*.*)
4. The release workflow will automatically create a GitHub release