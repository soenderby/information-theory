# Agent Instructions

This is a personal knowledge base about information theory, communication theory, classification, cybernetics, and related fields. It is maintained by Jakob (@soenderby), a software developer.

---

## About the Curator

**Purpose**: Dual — practical (inform how to organise and retrieve information in other projects) and intellectual (genuine curiosity about the theoretical foundations).

**Interests**: The theory and practice of organising, transmitting, and retrieving information. The intersections between information theory, communication theory, library/information science, network theory, cybernetics, and epistemology. Both foundational texts and modern applications.

**The primary audience** is Jakob himself, and other technically-minded people who want to understand the deep structure of information and how it flows through systems.

**Quality filter**: This field is less commercially noisy than AI, but has its own failure modes: textbook summaries that add no interpretation, surface-level introductions that don't engage with the actual ideas, and secondary sources that flatten the original's nuance. Primary sources are strongly preferred. People who developed the ideas are preferred over people who summarise them. Depth over breadth.

---

## Start of Session

When beginning a session:

1. **Read `librarian-notes.md`** — running notes, decisions, gaps, open questions.
2. **Read `resources/index.md`** — compact inventory of what is tracked.
3. **Read full canonical files only when the task needs them** — `resources/books.md`, `resources/articles.md`, etc.

---

## Repo Structure

```
information-theory/
├── README.md
├── CLAUDE.md              ← you are here
├── librarian-notes.md     ← running notes across sessions
└── resources/
    ├── index.md           ← compact inventory of what is tracked
    ├── books.md           ← book-length sources
    ├── articles.md        ← papers, essays, shorter pieces
    ├── people.md          ← thinkers worth following
    └── projects.md        ← tools, software, implementations
```

---

## Adding Resources

### Workflow

1. **Fetch and read the source first.** Never annotate from a title or URL alone. When the agent drafts an annotation, the curator is encouraged to engage with the source directly. If a source seems below the quality bar, say so honestly.
2. **Write a meaningful annotation** — see quality guidelines below.
3. **Place in the right file** — books.md for book-length works, articles.md for papers and essays, people.md for thinkers, projects.md for tools.
4. **Update cross-links** — if a person entry exists, add their work to their entry. If a work is by someone in people.md, link to them.
5. **Update `librarian-notes.md`** if the session surfaced something worth remembering.
6. **Note connections.** When adding an entry, check whether it strengthens, complicates, or extends something already in the collection.
7. **Commit** with a short descriptive message in present tense.

### Entry Formats

**Person** (`resources/people.md`):
```markdown
## Name
- Link label: url

Who they are and what makes them worth tracking. What perspective or contribution distinguishes them? 1–3 sentences.
```

**Book** (`resources/books.md`):
```markdown
## [Title](url)
By [Author](people.md#author). What the book contributes. Capture the distinctive idea or framework, not just the topic.
```

**Article/Paper** (`resources/articles.md`):
```markdown
## [Title](url)
By [Author](people.md#author). What the piece contributes. Capture the specific insight, not just the topic.
```

**Project** (`resources/projects.md`):
```markdown
## [Project Name](url)
By [Author](people.md#author). What the project does and why it belongs here.
```

Separate all entries with `---`.

### What Makes a Good Annotation

- **Capture the specific idea, not the general topic.** "Proves that any channel has a maximum rate at which information can be reliably transmitted, and that rate is determined by the channel's noise characteristics" is useful. "Book about information theory" is not.
- **The "So What?" test.** Why does this source matter to the collection? What does the reader gain from knowing about it?
- **Note what's distinctive.** What makes this the source to read on this topic?
- **Note connections** to other entries when they exist.
- **Write for clarity.** Assume the reader is intelligent but may not know the field's jargon.
- **Be honest about limitations.** If you haven't fully engaged with a source, say so.

### Corroboration: "Also noted by"

When a source makes the same point as an existing entry without adding a new idea, record it as an "Also noted by" line:

```markdown
Also noted by: [Author (context, date)](url) — brief note on what angle they bring.
```

The source must have been read. Different context or voice required. Brief — name the who and the angle.

### What NOT to Add

- Textbook summaries that don't engage with the actual ideas
- Surface-level introductions that flatten the original's nuance
- Secondary sources when the primary source is available and readable
- Anything you haven't read

---

## Librarian Memory

- **`librarian-notes.md`** — running notes, read at session start. Keep entries short and dated.
- Archive when the file grows heavy (~200 lines). Create `librarian-archive.md` when needed.

Update `librarian-notes.md` when:
- A curatorial decision is made that isn't obvious from the guidelines
- A connection between entries is noticed
- A gap in the collection is identified
- The curator says something that reveals taste or preference worth preserving

---

## General Conventions

- **Prefer simplicity.** Readable markdown.
- **Suggest structure organically.** Only create new files when content warrants them.
- **File names:** lowercase, hyphen-separated.
- **Branch:** `main`
- **Commit messages:** short, descriptive, present tense.

---

## Related

This repo's curatorial patterns were extracted from [ai-resources](https://github.com/soenderby/ai-resources). See the [extracted patterns document](https://github.com/soenderby/ai-resources/blob/main/ai-generated/curatorial-patterns-extracted.md) for the full operational DNA.
