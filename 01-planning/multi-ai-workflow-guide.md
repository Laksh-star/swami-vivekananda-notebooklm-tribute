# Multi-AI Workflow Guide

> A decision framework for choosing the right AI tool for each task—
> learned through trial, error, and a few happy accidents.

---

## The Core Insight

No single AI does everything well. Each has character—distinct strengths, 
blind spots, and sweet spots. The magic happens when you orchestrate them 
like instruments in an ensemble, not soloists competing for the spotlight.

This guide captures what I learned building the Vivekananda NotebookLM notebook.

---

## The Decision Tree
```
START: What do I need to create?
│
├─► DEEP RESEARCH (facts, quotes, timelines, citations)
│   │
│   └─► Use: Perplexity AI
│       Why: Web synthesis, automatic citations, structured reports
│       Prompt tip: Ask for "comprehensive source document" with clear sections
│
├─► COMPARATIVE ANALYSIS (philosophy matrices, concept mapping)
│   │
│   └─► Use: Perplexity AI
│       Why: Can pull from multiple sources, good at structured comparisons
│       Prompt tip: Specify exact column structure you want
│
├─► CREATIVE WRITING WITH VOICE (essays, narratives, personal tone)
│   │
│   └─► Use: Claude (Sonnet or Opus with extended thinking)
│       Why: Nuanced voice, can mimic different writing styles authentically
│       Prompt tip: Specify tone AND who the "author" is (e.g., "high school student")
│
├─► STRUCTURED FRAMEWORKS (action plans, templates, checklists)
│   │
│   └─► Use: ChatGPT (with extended thinking)
│       Why: Excellent at systematic organization, consistent formatting
│       Prompt tip: Provide exact table structure you want
│
├─► FACTUAL Q&A / EXAM CONTENT (flashcards, quiz banks)
│   │
│   ├─► Option A: Gemini Pro
│   │   Why: Comprehensive coverage, good at factual density
│   │
│   └─► Option B: Claude Opus (with extended thinking)
│       Why: Better reasoning on conceptual questions
│       
│   Pro tip: Generate with BOTH, compare, keep the best of each
│
└─► FINAL ASSEMBLY & INTERACTION
    │
    └─► Use: Google NotebookLM
        Why: Source-grounded responses, built-in audio/flashcards/mind maps
        Prompt tip: Quality of output depends entirely on quality of sources
```

---

## Tool Profiles

### Perplexity AI
**Superpower:** Research synthesis with citations  
**Best for:** Gathering facts, quotes, timelines, comparative matrices  
**Watch out for:** Can be surface-level on philosophical nuance  
**Prompt pattern:** "Create a comprehensive source document for [topic]. Include: [specific sections]. Format as structured report with clear headings."

### Claude (Sonnet 4.5 / Opus 4.5)
**Superpower:** Voice and nuance  
**Best for:** Essays, reflection content, anything requiring authentic human tone  
**Watch out for:** Can be verbose; may need "be concise" guidance  
**Prompt pattern:** "Write [content type] in the voice of [specific persona]. Tone: [adjectives]. Constraint: [word count, style notes]."

### ChatGPT (5.2 Extended Thinking)
**Superpower:** Systematic organization  
**Best for:** Action plans, frameworks, templates, structured content  
**Watch out for:** Can feel formulaic; less natural voice  
**Prompt pattern:** "Create [X] different [templates/plans] for [topic]. Format as table with columns: [specify exact structure]."

### Gemini 3 Pro
**Superpower:** Factual comprehensiveness  
**Best for:** Exam Q&A, factual content at scale  
**Watch out for:** Less personality in writing  
**Prompt pattern:** "Generate [number] Q&A facts about [topic]. Mix: [X]% factual, [Y]% conceptual. Format: Q: [text] A: [text]."

### Google NotebookLM
**Superpower:** Source-grounded AI with built-in tools  
**Best for:** Final assembly, interactive layer, audio/visual outputs  
**Watch out for:** Only as good as your uploaded sources  
**Prompt pattern:** Custom instructions shape persona; chat prompts drive specific outputs

---

## Workflow Patterns That Worked

### Pattern 1: Research → Refine → Assemble
```
Perplexity (gather) → Claude (refine voice) → NotebookLM (assemble)
```
Used for: Quote collections, biographical content

### Pattern 2: Parallel Generation → Compare → Select
```
Gemini (version A) ─┬─► Compare ─► Keep best
Claude (version B) ─┘
```
Used for: Exam Q&A where I wanted both breadth and depth

### Pattern 3: Structure → Voice → Polish
```
ChatGPT (framework) → Claude (add voice) → NotebookLM (test with chat)
```
Used for: Action plans that needed both structure AND warmth

---

## Common Pitfalls (And How I Avoided Them)

| Pitfall | What Happened | The Fix |
|---------|---------------|---------|
| Using one tool for everything | Generic, uneven quality | Match tool to task type |
| Skipping the research phase | NotebookLM outputs were shallow | Invest in source quality first |
| Over-prompting | Outputs became bloated | Simpler prompts, then iterate |
| Not specifying format | Had to reformat everything manually | Include exact structure in prompt |
| Forgetting persona context | Essays sounded like AI, not students | Always specify "who" is writing |

---

## The Meta-Lesson

AI collaboration isn't about finding the "best" model. It's about understanding 
each tool's character and knowing when to call on each one.

Think of it like assembling a team:
- **Perplexity** is your researcher—thorough, cited, comprehensive
- **Claude** is your writer—nuanced, voice-flexible, thoughtful
- **ChatGPT** is your organizer—systematic, structured, reliable
- **Gemini** is your fact-checker—dense, comprehensive, precise
- **NotebookLM** is your conductor—bringing it all together into something interactive

The orchestra sounds better than any soloist.

---

*Last updated: January 2026*
