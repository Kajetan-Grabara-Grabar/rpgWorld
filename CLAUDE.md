# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**rpgWorld** is an Obsidian Vault project for documenting and world-building an RPG (Role-Playing Game) setting. This is a **documentation-focused project**, not a software development project. All content is managed as markdown files within the Obsidian knowledge management system.

### Key Characteristics

- **Type**: Obsidian Vault / Knowledge Management System
- **Primary Language**: Markdown (.md)
- **Configuration**: JSON (Obsidian settings)
- **No build system, tests, or CI/CD**: This is a documentation project that doesn't require compilation or automated testing
- **Development stage**: Active campaign development with foundational world-building documentation

## Directory Structure

```
rpgWorld/
├── .obsidian/              # Obsidian vault configuration and metadata
├── .claude/                # Claude Code settings
├── Świat/                  # World documentation folder
│   ├── OpisŚwiata.md      # Core world description (Region Ur)
│   └── KompleksKur-Nu-Gi-A.md  # Major dungeon complex documentation
├── Frakcje/                # Factions and organizations documentation
│   ├── RycerzeZakonuRóży.md   # Three orders of knights
│   ├── Gildie.md              # Guild organizations (mercantile, exploration, mining)
│   ├── KorsarzePowietrzni.md  # Airship corsairs
│   └── Nefilim.md             # Mysterious giant faction
├── Lokacje/                # Location documentation
│   ├── WielkaBiblioteka.md           # Underground trading hub
│   └── MiasteczkoNadBiblioteką.md    # Surface settlement
├── NPCs/                   # Non-player character documentation
│   └── OliverSchreiber.md  # Sample NPC with game statistics
├── Welcome.md              # Obsidian default welcome note
├── README.md               # Project readme
└── CLAUDE.md               # This file
```

## Content Architecture

### Vault Organization

The project uses an **Obsidian vault** with hierarchical note structure:

#### Świat/ folder: World documentation
- **OpisŚwiata.md**: Documents **Region Ur** - a forested region with multiple independent city-states
- **KompleksKur-Nu-Gi-A.md**: Major dungeon complex with three distinct levels (shallow caves, labyrinth, ancient city)
  - Contains both public information and GM-only secrets
  - Central location for campaign activity

#### Frakcje/ folder: Faction and organization documentation
Documents major organized groups within the world. All factions follow a consistent encyclopedic format with formal tone.

**Current factions**:
- **Rycerze Zakonu Czerwonej Róży** (Red Rose Knights): Wealthy, corrupt military order controlling magical dust trade
- **Rycerze Zakonu Białej Róży** (White Rose Knights): Medical/hospital order, politically neutral
- **Rycerze Zakonu Czarnej Róży** (Black Rose Knights): Destroyed archaeological order, ruins remain
- **Gildie Handlowe** (Mercantile Guilds): Decentralized merchant organizations
- **Gildie Eksploracyjne** (Exploration Guilds): Dungeon exploration franchises
- **Gildie Górnicze** (Mining Guilds): Exploitative mining operations
- **Korsarze Powietrzni** (Air Corsairs): Airship operators with monopoly on dust-powered technology
- **Nefilim**: Mysterious giant faction with non-magical advanced technology, rising threat

Each faction file uses a standardized structure (see Faction Documentation Format below).

#### Lokacje/ folder: Location documentation
Documents specific places within the world. Locations follow encyclopedic format similar to factions.

**Current locations**:
- **Wielka Biblioteka** (Great Library): Underground chamber in Kur-Nu-Gi-A complex, now a trading hub
- **Miasteczko Nad Biblioteką** (Town Above the Library): Surface settlement serving explorers

#### NPCs/ folder: Non-player character documentation
Character sheets for important NPCs, including game statistics and GM notes.

**Current NPCs**:
- **Oliver Schreiber**: Merchant cartographer, potential quest giver and recurring character

### Faction Documentation Format

Faction documents follow a consistent structure for easy navigation and comparison:

1. **Title (H1)**: Faction/Organization name
2. **Opis section (H2)**: Overview of the organization, membership structure, and core characteristics
3. **Economic/Resource section (H2)**: Economic model, primary income sources, dependencies
   - Named variably: "Struktura ekonomiczna", "Model ekonomiczny", "Struktura organizacyjna"
4. **Social/Political section (H2)**: Position in society, diplomatic relationships, influence
   - Named variably: "Wpływ polityczny i potencjał", "Pozycja społeczna i wpływ", "Współpraca i relacje zewnętrzne"
5. **Additional specialized sections (H2)**: As appropriate for faction type
   - Examples: "Technologia pyłowa", "Potencjał militarny", "Wyposażenie indywidualne"
6. **Notes section**: Key observations prefaced with **"Notatka – [Topic]"** in bold

**Writing style**: Formal, encyclopedic tone. Avoid colloquialisms. Use precise terminology.

This format enables consistent organization comparison and supports potential future visualization of faction dynamics.

### Location Documentation Format

Location documents follow a similar encyclopedic structure:

1. **Title (H1)**: Location name
2. **Opis section (H2)**: General overview and significance
3. **Specialized sections (H2)**: As appropriate for location type
   - Examples: "Historia odkrycia", "Układ przestrzenny", "Dostęp i transport", "Infrastruktura komercyjna"
4. **Notes section**: Key observations prefaced with **"Notatka – [Topic]"** in bold

**Writing style**: Formal, encyclopedic tone matching faction documentation.

### NPC Documentation Format

NPC documents combine game statistics with narrative information:

1. **Title (H1)**: NPC name
2. **Informacje podstawowe (H2)**: Table with identity, motivation, origin, level, type
3. **Statystyki (H2)**: Table with attribute dice (DEX, INS, MIG, WLP)
4. **Punkty (H2)**: Table with HP, WP, Initiative
5. **Odporności elementarne (H2)**: Table with elemental resistances
6. **Uzbrojenie (H2)**: Tables for melee and ranged attacks
7. **Notatki dla Mistrza Gry (H2)**: GM notes with subsections:
   - Wygląd i osobowość
   - Profesja i umiejętności
   - Aktualna sytuacja
   - Cele i motywacje
   - Haki fabularne
   - Sugerowane wykorzystanie

**Writing style**: Game statistics use tables for clarity. GM notes use formal but practical tone.

### Knowledge Graph Structure

The project leverages Obsidian's features:

- **Wikilinks**: Cross-references between notes using `[[link syntax]]`
  - Wikilink conventions: `[[Region Ur]]` for world regions, `[[Rycerze Zakonu Czerwonej Róży]]` for factions, `[[Wielka Biblioteka]]` for locations
  - Enables automatic backlink tracking across the knowledge base
- **Backlinks**: Automatic tracking of relationships between documents
  - Essential for finding all references to a given faction, location, or character
- **Tags**: Categorization of content (e.g., `#region`, `#faction`, `#character`, `#location`)
  - Use tags to mark faction alignment (e.g., `#corrupt`, `#charitable`, `#militant`, `#neutral`)
- **Properties/Metadata**: YAML frontmatter for structured data about world elements
  - Consider adding properties for faction type, size, influence level, location type
- **Graph View**: Visual exploration of how notes connect to each other
  - Particularly useful for understanding faction relationships and dependencies

## World-Building Principles

### Writing Style Guidelines

All documentation follows a **formal, encyclopedic style**:

- Avoid colloquialisms and informal language
- Use precise, technical terminology
- Present information objectively (even for morally questionable factions)
- Maintain consistent tense (usually present tense for current state, past tense for history)
- Use passive voice where appropriate for formal tone

### Content Organization

- **Separation of player and GM knowledge**: Documents like KompleksKur-Nu-Gi-A.md clearly mark GM-only sections
- **Interconnected factions**: Faction documents reference each other (e.g., Korsarze depend on Zakon Czerwonej Róży for magical dust)
- **Locations tied to factions**: Guild control of locations is documented (e.g., mining guild controls Wielka Biblioteka infrastructure)

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

1. **Adding new factions**: Create markdown files in `Frakcje/` following the faction format
2. **Adding new locations**: Create markdown files in `Lokacje/` following the location format
3. **Adding new NPCs**: Create markdown files in `NPCs/` following the NPC format
4. **Linking between notes**: Use Obsidian wikilink syntax: `[[Note Name]]`
5. **Organizing structure**: Use heading hierarchy (H1-H6) to structure content within documents
6. **Tagging content**: Add tags at the bottom of documents for categorization
7. **Using properties**: Add metadata blocks at the top of files for structured information

### Markdown Best Practices

- Use meaningful heading structures (H1 for titles, H2 for major sections)
- Link related notes using wikilinks to create a navigable knowledge graph
- Use consistent naming conventions (PascalCase for note titles)
- Include tags and properties for categorization and filtering
- Keep notes focused on single topics (one character, one location, one faction)
- Use tables for structured data (especially in NPC stat blocks)
- Use **bold** for emphasis in section headers like "Notatka – [Topic]"

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

1. Create new markdown files in appropriate folder (`Świat/`, `Frakcje/`, `Lokacje/`, `NPCs/`)
2. Follow the relevant documentation format (faction, location, or NPC)
3. Add wikilinks to connect to existing documentation
4. Use properties for structured metadata
5. Tag content appropriately for easy discovery
6. Maintain formal, encyclopedic writing style

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
- All documentation follows a **formal, encyclopedic writing style** - avoid informal language
- **GM-only content** should be clearly marked in documents
- The project is actively developed - content continues to expand with campaign development
