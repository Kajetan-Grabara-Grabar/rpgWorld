# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**rpgWorld** is an Obsidian Vault project for documenting and world-building an RPG (Role-Playing Game) setting. This is a **documentation-focused project**, not a software development project. All content is managed as markdown files within the Obsidian knowledge management system.

### Key Characteristics

- **Type**: Obsidian Vault / Knowledge Management System
- **Primary Language**: Markdown (.md)
- **Configuration**: JSON (Obsidian settings)
- **No build system, tests, or CI/CD**: This is a documentation project that doesn't require compilation or automated testing
- **Early stage**: Currently contains foundational world-building documentation

## Directory Structure

```
rpgWorld/
├── .obsidian/              # Obsidian vault configuration and metadata
├── .claude/                # Claude Code settings
├── Świat/                  # Main world documentation folder
│   └── OpisŚwiata.md      # Core world description (Region Ur documentation)
├── Frakcje/                # Factions and organizations documentation
│   └── RycerzeZakonuRóży.md  # Orders of Knights documentation
├── Welcome.md              # Obsidian default welcome note
├── README.md               # Project readme (currently empty)
└── CLAUDE.md               # This file
```

## Content Architecture

### Vault Organization

The project uses an **Obsidian vault** with hierarchical note structure:

- **Świat/** folder: Contains all world-building documentation
  - Currently documents **Region Ur** - a forested region with multiple independent city-states
  - Expected to expand with documentation of:
    - Characters and NPCs
    - Magic systems and lore
    - Geography and locations
    - Historical events and timelines

- **Frakcje/** folder: Contains faction and organization documentation
  - Documents major organized groups within the world
  - Current factions: Rycerze Zakonu Czerwonej Róży, Rycerze Zakonu Białej Róży
  - Each faction file uses a standardized structure (see Faction Documentation Format below)

### Faction Documentation Format

Faction documents follow a consistent structure for easy navigation and comparison:

1. **Title (H1)**: Faction/Organization name
2. **Opis section (H2)**: Overview of the organization, membership structure, and core characteristics
3. **Economic/Resource section (H2)**: Economic model, primary income sources, dependencies (named variably based on faction type: "Struktura ekonomiczna", "Model ekonomiczny", etc.)
4. **Social/Political section (H2)**: Position in society, diplomatic relationships, influence (named variably based on context: "Wpływ polityczny i potencjał", "Pozycja społeczna i wpływ", etc.)
5. **Notes section (H3)**: Key observations prefaced with **"Notatka – [Topic]"** in bold

This format enables consistent organization comparison and supports potential future visualization of faction dynamics.

### Knowledge Graph Structure

The project leverages Obsidian's features:

- **Wikilinks**: Cross-references between notes using `[[link syntax]]`
  - Wikilink conventions: `[[Region Ur]]` for world regions, `[[Rycerze Zakonu Czerwonej Róży]]` for factions
  - Enables automatic backlink tracking across the knowledge base
- **Backlinks**: Automatic tracking of relationships between documents
  - Essential for finding all references to a given faction, location, or character
- **Tags**: Categorization of content (e.g., `#region`, `#faction`, `#character`, `#neutral`)
  - Use tags to mark faction alignment (e.g., `#corrupt`, `#charitable`, `#militant`)
- **Properties/Metadata**: YAML frontmatter for structured data about world elements
  - Consider adding properties for faction type, size, influence level in future expansions
- **Graph View**: Visual exploration of how notes connect to each other
  - Particularly useful for understanding faction relationships and dependencies

## Obsidian Configuration

**Enabled Core Plugins** (in `.obsidian/core-plugins.json`):
- File Explorer, Global Search, Quick Switcher
- Graph and Outline views (important for visualizing world structure)
- Backlink and Outgoing Link panels
- Canvas (for mind-mapping world elements)
- Tag Pane, Properties, Page Preview
- Sync, Daily Notes, Templates, Note Composer

**Key Settings**:
- Workspace configuration stored in `.obsidian/workspace.json`
- Claude Code integration settings in `.claude/settings.local.json`

## Working with the Project

### Editing World Documentation

1. **Adding new world elements**: Create markdown files in the appropriate subfolder under `Świat/`
2. **Linking between notes**: Use Obsidian wikilink syntax: `[[Note Name]]`
3. **Organizing structure**: Use heading hierarchy (H1-H6) to structure content within documents
4. **Tagging content**: Add tags at the bottom of documents: `#region #geography #completed`
5. **Using properties**: Add metadata blocks at the top of files for structured information

### Markdown Best Practices

- Use meaningful heading structures (H1 for titles, H2 for major sections)
- Link related notes using wikilinks to create a navigable knowledge graph
- Use consistent naming conventions (snake_case or PascalCase) for note titles
- Include tags and properties for categorization and filtering
- Keep notes focused on single topics (one character, one location, etc.)

### Obsidian Vault Best Practices

- Use the Outline view to navigate within large documents
- Use the Graph view to visualize relationships between world elements
- Use the Tag Pane to browse and organize content by category
- Use Daily Notes for session notes or campaign journals
- Use Templates for consistent formatting of similar content types

## Git Workflow

This project uses standard Git version control:

```bash
git status           # Check current changes
git add .            # Stage changes
git commit -m "msg"  # Commit with message
git push             # Push to remote (github.com/Kajetan-Grabara-Grabar/rpgWorld)
```

**Branch**: Main branch is used for all commits.

## Common Tasks

### Expand World Documentation

1. Create new markdown files in `Świat/` for new regions, characters, or factions
2. Add wikilinks to connect to existing documentation
3. Use properties for structured metadata (e.g., population, ruler, climate)
4. Tag content appropriately for easy discovery

### Review Relationships

1. Open the Graph view in Obsidian to visualize connections
2. Use the Backlinks panel to see what references a note
3. Use the Outgoing Links panel to see what a note links to

### Navigate the Knowledge Base

1. Use Global Search (Ctrl/Cmd + Shift + F) to find content
2. Use Quick Switcher (Ctrl/Cmd + K) to jump between notes
3. Use the File Explorer to browse the directory structure
4. Use the Outline view to navigate within large documents

## Important Notes

- This is a **documentation project**, not a code project
- There are no build steps, tests, or linting to configure
- Obsidian uses wikilinks and a knowledge graph model - familiarize yourself with this paradigm
- The `.obsidian/` folder contains metadata that Obsidian reads; respect this structure
- The project is in early stages - content is foundational and expected to grow significantly
