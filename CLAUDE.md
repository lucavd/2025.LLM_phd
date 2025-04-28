# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands
- Render Quarto documents: `quarto render filename.qmd`
- Preview Quarto documents: `quarto preview filename.qmd`
- Render all documents: `quarto render`
- Convert to specific format: `quarto render filename.qmd --to html|pdf|docx`

## Code Style Guidelines
- Formatting: Follow Quarto markdown conventions
- YAML headers: Use standardized format for consistent document rendering
- Image paths: Always use relative paths (e.g., `images/filename.png`)
- Code blocks: Use appropriate language tags for syntax highlighting (e.g., ```r, ```python)
- Document structure: Use hierarchical headings (##, ###, ####) for proper document organization
- Speaker notes: Place notes in ::: notes ::: blocks for presentation slides
- CSS styling: Place custom styling in `styles.css` file to maintain consistency

## Slide Creation Style
- Use `##` for slide titles/headers
- Use incremental lists with `incremental: true` in YAML or manually with ::: {.incremental}
- Style text with span syntax: [Text]{style="color:#2E86C1;"}
- Use columns with ::::: columns and ::: {.column width="X%"} syntax
- Add horizontal dividers with `---` or `------------------------------------------------------------------------`
- Include speaker notes in ::: notes ::: blocks at the end of each slide
- Format callouts with ::: callout-note or ::: callout-warning blocks
- Use consistent color scheme for headers (#2E86C1, #117A65, etc.)

## Practical Section Guidelines
- Demonstrate both commercial tools (ChatGPT, Claude) and local deployment options (LM Studio, WebLLM)
- Include hands-on examples with clinical text summarization and analysis
- Emphasize data privacy considerations when handling clinical information
- Structure prompts to demonstrate key LLM parameters (temperature, context window management)
- Include examples of prompt techniques for clinical use cases (chain-of-thought, structured prompting)
- Provide comparison examples between general and medical-specific LLMs when possible