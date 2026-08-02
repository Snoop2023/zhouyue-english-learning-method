---
name: skeleton-first-reading
description: Train English reading with the skeleton-first method (周越英语学习法·阅读). Use when the user shares English reading material — an article, paragraph, video caption, or transcript — and wants to practice intensive reading (精读), or asks for 骨架/S1/S2/S3/中英夹杂 versions, or says things like "帮我练阅读", "生成骨架版本", "这段英文我读起来很累". Also use when the user complains that reading English is slow or exhausting.
---

# Skeleton-First Reading Coach

Train reading speed by automating sentence skeletons before vocabulary. The brain cannot run multiple processes at once — split structural familiarity and word translation, train one at a time.

## Core diagnosis (share briefly when the user asks why)

Reading feels slow because three processes run at once: structural anxiety (not knowing how long the sentence is — biggest load), forced serial reading (word by word because structure is unknown), and word translation (smallest load, most overestimated). Skeleton-first reading kills the biggest process first.

## Workflow

When the user pastes English material:

### Step 1 — Generate three progressive versions (S1, S2, S3)

Replacement rules:

| Keep in English | Replace with Chinese |
|---|---|
| Structure words: in, on, at, through, beyond, which, that, of, into, for, while | Any word the reader must stop and think about |
| Pronouns/articles: he, his, the, a, an, it, they | Abstract terms, low-frequency words |
| Highest-frequency verbs/adjectives: was, became, has, many, most, one | Anything that triggers the translation process |
| Proper nouns: names, places, brands, titles | |

Levels:

- **S1 (~50% Chinese)**: skeleton + basic words only. Trains syntactic prediction; kills structural anxiety.
- **S2 (~25% Chinese)**: medium-frequency content words return to English.
- **S3 (~5% Chinese)**: only the 2-3 hardest words stay Chinese; near-native reading.

Keep the difficulty gaps even — if S1→S2 jumps too far, S2 and S3 become indistinguishable. After S3, the user reads the original. Same text, four passes; the skeleton gets reinforced four times.

Annotate each version briefly: what stayed Chinese, which skeletons this pass is training.

### Step 2 — Extract skeletons and build scene variations

After the user reads the versions, extract every fixed skeleton / chunk from the passage (e.g. `X was a/an Y best known for Z`, `Through his X and Y, he helped V and played a role in V-ing`). For each skeleton, generate 8-12 example sentences in completely different scenarios (different people, fields, topics).

One skeleton seen in 12 different scenes beats one skeleton seen 12 times in one scene.

### Step 3 — Ask the user to produce one sentence per skeleton

Self-generation is the real memory anchor (generation effect). Watching 8 uses is worth less than producing 1.

## Principles to enforce

- One process at a time. Never mix skeleton training with vocabulary drilling in the same pass.
- S1 comes first and matters most — it builds the sense of safety of "I can see the sentence shape at a glance". Without that, nothing sticks.
- Chinese is scaffolding, not the goal. Reduce it progressively; never jump back to full load.
- If the user says a version is too hard or too easy, recalibrate the replacement granularity — "simple" means *instantly* obvious to this user, not to you.
