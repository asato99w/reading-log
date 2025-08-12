# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this scientific reading log repository.

## Repository Overview
This is a systematic reading log repository for scientific books, organized by authors and supporting bilingual content (English/Japanese). The repository follows an author-based classification system with comprehensive book analysis and summaries.

## Directory Structure
```
reading_log/
├── BIOLOGY/                    # Life sciences subject area
│   ├── [Author_Name]/         # Author-based organization
│   │   ├── AUTHOR.md          # Comprehensive author profile
│   │   └── [Book_Title]/      # Individual book directory
│   │       ├── CLAUDE.md      # Book-specific instructions
│   │       ├── README.md      # Book overview
│   │       ├── en/           # English content
│   │       │   ├── Author_[Name].md  # Book-context author info
│   │       │   ├── Overall_Structure.md
│   │       │   ├── Reading_Notes.md
│   │       │   └── structure/ # Chapter summaries
│   │       └── jp/           # Japanese content
│   │           ├── 全体構成.md
│   │           ├── 読書メモ.md
│   │           ├── 著者_[Name].md
│   │           └── 構成/      # Chapter details
└── ECONOMY/                   # Economics subject area
    └── [Same structure as BIOLOGY]
```

## Author Organization System
- **AUTHOR.md**: Central profile containing comprehensive information about the author (biography, academic career, major contributions, awards, legacy)
- **Book-specific author files**: Context-specific information about the author during the time of writing each book, including:
  - Pre-publication context and motivation
  - Academic/personal circumstances during writing
  - Immediate reception and impact
  - Long-term influence of that specific work

## File Naming Conventions
- Author directories: `FirstName_LastName/` (underscore for spaces)
- Book directories: `English_Title--Japanese_Title/`
- English author files: `Author_FirstName_LastName.md`
- Japanese author files: `著者_[Name].md`
- Chapter files: `Chapter[N]_Title.md` / `第[N]章_タイトル.md`

## Content Structure Standards
Each chapter file contains:
- **Chapter Overview**: Brief 1-2 sentence summary
- **Main Content**: 2-3 key topics with detailed bullet points
- **Key Points**: 3 important takeaways

## Git Repository Management
- Repository is connected to GitHub: https://github.com/asato99w/reading-log.git
- Use conventional commit messages with descriptive content
- Always include the standard footer in commit messages:
  ```
  🤖 Generated with [Claude Code](https://claude.ai/code)
  
  Co-Authored-By: Claude <noreply@anthropic.com>
  ```

## Working Instructions
1. Maintain bilingual consistency between English and Japanese versions
2. Update README.md when adding new books or authors
3. Follow established patterns for content organization
4. Ensure CLAUDE.md files contain book-specific guidance
5. When reorganizing, maintain existing content integrity
6. Always commit and push changes to GitHub after major modifications

## CRITICAL: Required Files for Each Book
Each book MUST have these files in the exact structure:
```
[Book_English_Title--Japanese_Title]/
├── CLAUDE.md           # Book-specific instructions
├── README.md           # Book overview (bilingual)
├── en/                 # English content
│   ├── AI_Reading_Notes.md     # AI-generated notes
│   ├── Author_[Name].md        # Author context for this book
│   ├── Overall_Structure.md    # Book structure overview
│   └── structure/              # Chapter files
│       └── Chapter[N]_[Title].md
└── jp/                 # Japanese content
    ├── AI読書メモ.md
    ├── 著者_[Name].md
    ├── 全体構成.md
    └── 構成/
        └── 第[N]章_[タイトル].md
```

## File Creation Order
When creating a new book entry:
1. Create directory with format: `English_Title--Japanese_Title/`
2. Create CLAUDE.md with book-specific guidance
3. Create README.md with bilingual book overview
4. Create English version files first:
   - Overall_Structure.md
   - Author_[Name].md
   - AI_Reading_Notes.md (if applicable)
   - structure/ directory with chapter files
5. Then create Japanese version with same content structure

## Current Authors and Books
### BIOLOGY
- Richard Dawkins: The Selfish Gene, The Blind Watchmaker
- John Maynard Smith: Evolution and the Theory of Games  
- Daniel Davis: The Beautiful Cure
- Siddhartha Mukherjee: The Song of the Cell

### ECONOMY
- Alvin Roth: Who Gets What — and Why
- Ariel Rubinstein: Economic Fables
- von Neumann & Morgenstern: Theory of Games and Economic Behavior