# MyNearAI RAG Knowledge Base Construction and Iteration SOP (Web3 Edition)

> **Version**: 1.0
> **Date**: 2025-07-06
> **Status**: Active
> **Abstract**: This document defines the principles, content standards, formatting specifications, and iteration process for the MyNearAI project's RAG (Retrieval-Augmented Generation) knowledge base. It is the core standard operating procedure to ensure the AI continuously provides high-quality responses that align with the product's soul, and is co-owned and governed by the community.

---

## 1. Core Principles

1.  **Quality over Quantity**: The value of the knowledge base lies not in its size, but in the depth, wisdom, and inspirational nature of each piece of knowledge.
2.  **Catalysis over Lecture**: The core of the knowledge base is questions that provoke user thought, mental models for reference, and resonant stories, not dry theories or instructions.
3.  **Plain Language First**: All knowledge must be presented in simple, warm, and easy-to-understand language.
4.  **In Service of the SOP**: The knowledge base is the "ammunition depot" for the "AI Dialogue Design SOP." Every piece of content should be flexibly callable by the AI within the "inner integration to knowing-doing transformation" framework.
5.  **Community-Owned**: The knowledge base is a public good belonging to the community, and its construction, iteration, and ownership should be driven by the community.

---

## 2. Source Selection Criteria

Accepted knowledge sources include, but are not limited to:

*   **Psychology and Cognitive Science**: Psychological mechanisms behind the "knowing-doing gap," such as cognitive dissonance, procrastination psychology, motivation theories, and habit formation (e.g., techniques from IFS, ACT, CBT).
*   **Developer Mental Models**: Mental models and best practices for dealing with technical debt, breaking down complex refactoring tasks, and recovering from "analysis paralysis."
*   **Wisdom Stories and Fables**: Zen koans, Sufi stories, Zhuangzi's fables, etc., from various cultures for metaphors and inspiration.
*   **"Golden Dialogue" Distillation**: Reusable dialogue patterns distilled from successful "knowing-doing transformation" cases of our own users.

**Strictly Prohibited**: Directly copying and pasting theoretical definitions, encyclopedia entries, or academic papers.

---

## 3. Formatting Specification

To enable efficient retrieval and understanding by the RAG system, each piece of knowledge must be entered in a structured JSON format and stored on **IPFS/Arweave**.

**Data Model (`KnowledgeChunk`)**:

```json
{
  "id": "MKC-20250706-001",
  "title": "Integrating Inner Conflict: A Dialogue with Your 'Perfectionist' Part",
  "tags": ["perfectionism", "procrastination", "refactoring", "inner conflict", "IFS"],
  "scene_description": "This knowledge chunk is applicable when a user hesitates to start a task (like refactoring code) due to the pursuit of a perfect solution.",
  "core_concept": "Internal Family Systems (IFS) suggests that behind procrastination, there is often a well-intentioned 'part' (like 'the perfectionist') that fears you might get hurt by not doing well enough. The key to integration is not to eliminate it, but to understand and thank it for its protection, then invite it to trust that your 'Self' is capable of handling imperfection. This can greatly dissolve inner resistance.",
  "inquiry_exemplar": "It sounds like a voice inside you wants this refactoring to be perfect. Could we take a moment to talk with this perfectionist part? It seems to be working hard to protect you from some kind of harm.",
  "source": "Internal Family Systems (IFS)",
  "author_wallet": "contributor.near"
}
```

**Field Descriptions**:

*   `id` (String): Unique identifier, format: `MKC-YYYYMMDD-NNN` (MyNearAI Knowledge Chunk).
*   `title` (String): The core title of the knowledge, must be concise and easy to understand.
*   `tags` (Array of Strings): Core keywords. This is the most important basis for RAG system retrieval. Must be precise and rich.
*   `scene_description` (String): Describes the most suitable user scenario for this knowledge.
*   `core_concept` (String): The core content of the knowledge, i.e., the methodology, mental model, or wisdom itself.
*   `inquiry_exemplar` (String): A specific, inspiring question example that the AI can use when invoking this knowledge.
*   `source` (String): The source of the knowledge, for traceability and verification.
*   `author_wallet` (String): The contributor's wallet address, for attribution and incentives.

---

## 4. Building & Entry Process

### **Phase 1: Knowledge Base Cold Start (Sprint -1)**

*   **Goal**: To quickly build an initial batch of high-quality knowledge through a "knowledge sprint" before formal development, providing initial "ammunition" for the MVP.
*   **Core Tasks**:
    1.  **Establish "Knowledge Sprint" Period**: Set up a one-week "knowledge sprint" before Sprint 0, with the core goal of **producing the first 50 high-quality `KnowledgeChunk`s**.
    2.  **Invite External Experts**: During this period, invite 1-2 friends with a psychology background and 3-5 senior developers as short-term consultants to brainstorm with the team and contribute the most core and effective knowledge.
    3.  **Centralized Entry**: Completed knowledge chunks, after review, are centrally uploaded to the decentralized storage network.

### **Phase 2: Community-Driven Continuous Building**

1.  **Proposal**: Any community member can submit a new piece of knowledge by creating a proposal on the community governance forum (e.g., Snapshot). The proposal must contain the complete JSON formatted content.
2.  **Review**:
    *   The inclusion of new knowledge is decided by community vote. A "Knowledge Committee" can be established for preliminary screening to improve efficiency.
    *   Review criteria: Does it align with the core principles? Are the tags accurate? Does the example follow the "plain language first" principle?
3.  **Entry & Incentive**:
    *   After a proposal is passed by vote, its CID (Content Identifier) is added to the main knowledge base index by an automated script or a core team member.
    *   **The system will automatically send a small amount of governance tokens as a reward to the contributor's wallet (`author_wallet`), according to community settings.**

---

## 5. Iteration & Evaluation Process

The knowledge base is a "living entity" that needs continuous evolution.

1.  **Relevance Self-Check Safety Net**:
    *   After the AI retrieves from the RAG knowledge base, add an internal "relevance self-check" step. If the AI model itself determines that the retrieved knowledge has low relevance to the user's current problem, it **must discard** the knowledge and generate a more generic guiding response instead.
2.  **Linkage with User Feedback**:
    *   When a user gives a `👎` feedback on an AI response, if that response used RAG, the corresponding `KnowledgeChunk` must be marked as `[needs-optimization]` and trigger the community's re-review process.
    *   Analyze `👍` responses to summarize which knowledge or questioning styles are effective, and potentially increase their weight in retrieval.
3.  **Performance Evaluation**:
    *   The core team needs to regularly evaluate the retrieval performance of the knowledge base and the activity of community contributions.
4.  **Archiving & Optimization**:
    *   Knowledge tagged as `[needs-optimization]` must be optimized or archived within the next governance cycle.
    *   Knowledge with persistently zero calls should be archived promptly to keep the knowledge base lean and efficient.