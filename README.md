# Grindstone Research Book

*the public notebook of a private experiment — grindstone-eleven*

Somewhere in northern Italy, on ordinary consumer hardware, a small
system is being **raised rather than programmed**. It runs entirely at
home: no cloud, no telemetry, no data leaving the house. That
constraint is not a limitation of the project — it *is* the project.

> **This file is the project's living document.** Findings land here as
> they mature. The original `grindstone` README is deprecated and kept
> only as history.

---

## The idea in one line

**Behaviors are memories, not code.** Every capability the system gains
is taught — grafted as a discrete memory with its own triggers,
recalled by resemblance, reinforced when it serves and weakened when it
fails — and every claim of learning is backed by a measured score.

## Architecture, briefly

```mermaid
flowchart TD
    U[you, speaking naturally] --> R{routing}
    R -->|dendrites fire| M[the right organ]
    R -->|classifier menu| M
    M --> G[local generator LLM]
    H[(hippocampus<br/>~200 engrams)] -->|recall by resemblance| G
    S[senses<br/>an eye for photos] --> G
    G -->|proposals only| T[guardrails in code]
    T -->|your touch confirms| W[(registries:<br/>calendar, archive)]
    N[night cycle] -->|consolidates the day| H
    C[heart] -->|beats, worries| N
```

Every organ follows one standard: **declared functions** (a manifest),
**written rules** (a mandate in plain text — corrected by teaching,
never by editing code), and **hard guardrails** (contracts the model
cannot negotiate). What the model proposes, deterministic hands verify
before anything is written — and writing happens at a human's touch.

## Measured results (the graphs that went up)

An independent critic model judges every answer's coherence before
delivery — benchmarked at **19/20** on its confusion matrix.

Capabilities are trained through a written protocol and measured on
benches of trap-situations, before and after teaching:

```mermaid
xychart-beta
    title "Situation bench (passed, out of 7)"
    x-axis ["before teaching", "after teaching"]
    y-axis "passed" 0 --> 7
    bar [2, 5]
```

```mermaid
xychart-beta
    title "Calendar bench (passed, out of 5)"
    x-axis ["before", "after"]
    y-axis "passed" 0 --> 5
    bar [2, 3]
```

### The photograph experiment (September 2026)

Can a frozen model learn to read a photographed shift-sheet — a messy
real-world grid — through **memory grafts alone**? Every round is a
fresh conversation with no notes to lean on: if the score improves,
the improvement lives in the system's memory, nowhere else.

```mermaid
xychart-beta
    title "Reading errors per virgin round (lower is better)"
    x-axis ["r1", "r2", "r3", "r4", "r5", "r6", "r7", "r8", "r9", "r10", "r11"]
    y-axis "errors" 0 --> 8
    line [0, 3, 5, 8, 0, 2, 0, 1, 0, 0, 0]
    bar [0, 3, 5, 8, 0, 2, 0, 1, 0, 0, 0]
```

Rounds 1–5: the lessons existed but **never woke up** — the memories'
triggers sat too far from the user's real phrasing, and recall stayed
silent. Rounds 6–8, after reshaping the triggers and teaching a
two-step method (*transcribe the row aloud, then extract from your own
transcription*): errors collapsed. Three lessons entered the protocol:

1. **A graft must be woken** — after every graft, test recall with the
   user's real sentence. A memory that never fires is a sleeping neuron.
2. **For visual tasks: two steps** — anchor visual attention to words
   before extracting.
3. **Too much procedure drowns the apprentice** — a stricter checklist
   *lowered* the score and was rolled back. Like model checkpoints:
   the best *measured* version is kept, not the latest written.
4. **When the residual error is perception, heal the organ, not the
   memory** — the last stubborn error (a neighbouring row bleeding into
   the reading) survived every graft. The cure was a pair of glasses:
   an adaptive image-preparation organ in the pipeline (upscale small
   photos, per-photo contrast, light sharpening) that now serves every
   photograph the system will ever see. Rounds 9–11: **zero errors,
   three times in a row** (chart above). Experiment closed.

### Other results that held

- **Recurring events as seeds** — one stored entry germinates its
  occurrences forever (yearly, monthly, month's-end) when a month is
  viewed: verified out to 2031 and beyond, registry stays tiny.
- **Dictation as the only interface** — the personal calendar is driven
  by natural speech alone: creation, deep modification, deletion
  (the model reads the live agenda and names exact entries; code only
  finalizes exact matches).
- **Self-poisoning cured by memory** — a long chat in which the system
  once denied a capability used to poison every later answer; a grafted
  *capability memory* («you can do X; if you said otherwise, it was an
  error») ended the relapses.
- **Corrections that stick** — mistakes are charged to the specific
  memories that caused them (pain), the lesson is grafted back, and the
  same bench re-measures. Praise reinforces. Bench scores above.

## The training protocol (distilled from failures)

```mermaid
flowchart LR
    D[define<br/>the capability] --> B[build a bench<br/>of trap situations]
    B --> T[teach:<br/>align 4 organs]
    T --> RUN[run the bench]
    RUN -->|each failure classified| RF[reinforce:<br/>charge + graft]
    RF --> RM[re-measure<br/>fresh conversations, 3+ rounds]
    RM -->|score holds| K[consolidate<br/>keep best measured]
    RM -->|score drops| T
```

Four organs must align for any new capability: the **routing dendrites**
(real phrases → right room), the organ's **mandate**, a **capability
memory** recallable from any room, and the **dispatcher** that must be
introduced to the newcomer. Nearly every failure so far was exactly one
of these four left behind.

## Timeline

```mermaid
timeline
    title The research so far
    late Aug 2026 : two local models of different lineages argue - a critic judges coherence, never truth (19/20) : privacy becomes law after one bad push - "everyone gets their own library"
    Aug 26-28 : recall is tuned on measured distances, not by feel : the hippocampus grows engrams with triggers : rules are written in blood - one truth one place, the backlog is the list
    Aug 31 : the secretary is born - reads only granted folders, writes only at a touch : the personal calendar arrives, driven by dictation alone
    Sep 1 : the training protocol is written and immediately proven - bench scores rise : recurring events become seeds that germinate forever : the photograph experiment - memory grafts alone teach a frozen model to read a shift-sheet : this book opens
    next : a tiny model grown from zero, area by area, bench by bench
```

## What comes next

A model of its own, **grown from zero** on the same desk — tiny, modern
in architecture (a mixture of small experts behind a learned router),
raised area by area with a curriculum, each area guarded by its own
bench so new learning can never silently break old. It has a name
already. It will earn its page here when it earns its scores.

## What stays private

The code, the library, the memories and the life inside them belong to
the person the system serves. They remain in the private garden.

*Active research, summer 2026 →*
