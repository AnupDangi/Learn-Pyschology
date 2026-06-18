# Introduction to Psychology — PSYC 110

**Yale University · Open Yale Courses · Professor Paul Bloom**

Course site: https://oyc.yale.edu/psychology/psyc-110
Youtube Lectures: https://youtu.be/P3FKHH2RzjI?si=heaLVbvege7OyjSR

A comprehensive scientific introduction to the human mind — spanning neuroscience, development, language, memory, emotion, social psychology, mental illness, and happiness.

---

## Quick Start

**Just want to read?** Open the compiled PDF:

```
PSYC110_Complete_Notes.pdf   ← All 20 lectures in one formatted document (1 MB)
```

**Want individual lectures?** Browse the [`notes/`](./notes/) folder — one Markdown file per lecture.

---

## Folder Contents

```
Introduction to Psychology (PSYC 110)/
├── PSYC110_Complete_Notes.pdf    ← Complete notes (all 20 lectures, formatted)
├── PSYC110_Complete_Notes.html   ← Source HTML used to build the PDF
├── notes/                        ← Individual lecture notes (Markdown)
│   ├── lecture-1.md
│   ├── lecture-2.md
│   └── ... (through lecture-20.md)
├── transcripts/                  ← Raw lecture transcripts from oyc.yale.edu
│   ├── lecture-1.md
│   └── ...
├── fetch_transcripts.py          ← Script: download transcripts from Yale
└── build_pdf.py                  ← Script: compile notes into PDF
```

---

## Lecture Index

| # | Title | Topics |
|---|-------|--------|
| 1 | Introduction | Course overview, sub-fields of psychology, preview of key topics |
| 2 | Foundations: This Is Your Brain | Neuroscience, brain structure, neurons, split-brain research |
| 3 | Foundations: Freud | Psychoanalytic theory, unconscious, psychosexual development, defense mechanisms |
| 4 | Foundations: Skinner | Behaviorism, classical conditioning, operant conditioning, reinforcement |
| 5 | What Is It Like to Be a Baby | Cognitive development, Piaget, infant perception, theory of mind |
| 6 | How Do We Communicate? | Language acquisition, grammar, brain areas for language, sign language |
| 7 | Conscious of the Present (I) | Language cont., vision, visual processing, early vs. late selection |
| 8 | Conscious of the Present (II) | Memory systems, encoding, retrieval, eyewitness memory, amnesia |
| 9 | Love *(Guest: Prof. Peter Salovey)* | Evolutionary psychology of love, attachment, emotional intelligence |
| 10 | Evolution and Rationality | Natural selection, adaptive behavior, game theory, rational choice |
| 11 | Emotions, Part I | Basic emotions, facial expressions, emotion theories (James-Lange, Schachter) |
| 12 | Emotions, Part II | Disgust, fear, happiness, cross-cultural emotion, moral emotions |
| 13 | Why Are People Different? | Personality, intelligence, IQ, heritability, nature vs. nurture |
| 14 | What Motivates Us: Sex | Sexual psychology, gender differences, evolutionary explanations, mate preferences |
| 15 | Morality | Moral development, trolley problems, psychopathy, empathy, altruism |
| 16 | Self and Other, Part I | Social psychology, conformity, obedience (Milgram), persuasion |
| 17 | Self and Other, Part II; Sleep & Dreams | Attribution, stereotyping, sleep stages, dreams, laughter |
| 18 | Mental Illness, Part I *(Guest: Prof. Nolen-Hoeksema)* | Depression, anxiety disorders, diagnosis, DSM |
| 19 | Mental Illness, Part II | Schizophrenia, personality disorders, treatment approaches |
| 20 | The Good Life: Happiness | Therapy effectiveness, positive psychology, hedonic adaptation, set point theory |

---

## Scripts

### `fetch_transcripts.py`
Downloads all 20 official lecture transcripts from oyc.yale.edu into `transcripts/`.

```bash
python3 fetch_transcripts.py          # fetch all
python3 fetch_transcripts.py lecture-5  # fetch one
```

Skips lectures already downloaded (checks file size > 1 KB).

### `build_pdf.py`
Compiles all Markdown notes in `notes/` into `PSYC110_Complete_Notes.pdf`.

```bash
/opt/homebrew/bin/python3 build_pdf.py
```

Requires `weasyprint`:
```bash
pip install weasyprint --break-system-packages
```

---

## Note Format

Each file in `notes/` follows this structure:

```
# Lecture Title

## Overview        ← 1-paragraph summary of the full lecture
## Key Concepts    ← Definitions of key terms with exact quotes
## Detailed Notes  ← Section-by-section breakdown with timestamps
## Key Takeaways   ← Core ideas to remember
```

---

## Source

All transcripts are from the official Open Yale Courses website and are used for personal educational purposes.  
Original content © Yale University / Paul Bloom.
