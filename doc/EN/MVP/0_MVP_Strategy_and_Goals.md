# MyNearAI MVP Core Strategy and Goals (Web3 Edition)

> **Version**: 1.0
> **Date**: 2025-07-06
> **Status**: Active
> **Abstract**: This document is the supreme guideline for the MVP phase of the MyNearAI product line. It defines the MVP's guiding principles, core objectives, scope boundaries, and success criteria, aiming to validate the business viability of its core value proposition—solving "knowing but not doing"—combined with the Web3 feature of "user-owned AI."

---

## 1. Core MVP Principles

Our primary task at present is **not** to build a full-featured "decentralized consciousness evolution platform," but to focus on **creating a user-owned "practice dojo" that solves the "knowing-doing gap" for developers.**

To this end, we establish three core principles:

1.  **Validation over Building**: The sole purpose of the MVP is to gain real insights into the effectiveness of the "inner integration to knowing-doing transformation" model and the user's willingness to pay for "AI ownership," with minimal investment.
2.  **Depth over Breadth**: We will forgo a vast feature set to focus on polishing a "minimal but complete" core experience loop: "perceiving the block -> integrating the conflict -> taking micro-action -> on-chain proof."
3.  **Precision over Generality**: We will shift from serving broad "growth anxiety" sufferers to a highly focused group of "developers troubled by the knowing-doing gap." We will co-create with our beachhead users, letting them define the future of the product.

---

## 2. Strategic Goals of MVP

### 2.1. Primary Goal

**To validate, at minimum cost, whether the "inner integration to knowing-doing transformation" model is effective in helping developers solve the practical problem of "knowing but not doing," and to test whether users recognize the value of "owning their own AI."**

Specifically, we need to answer:

> **Can we, through an efficient "inner integration" dialogue, effectively help developers transform their inner conflict into a "first step action," and make them believe that this "self-owned" AI tool is worth having?**

### 2.2. Core Hypotheses to Validate

*   **Hypothesis 1 (The Hook)**: The core selling point, "Know you should, but can't? MyNearAI walks the first step with you," can effectively attract the attention of developers stalled by inner conflict.
*   **Hypothesis 2 (The Awareness)**: Users are willing to follow the AI's guidance to identify and acknowledge the real "blocks" hindering their action through dialogue.
*   **Hypothesis 3 (The Transformation)**: After perceiving the block, users are willing to accept the AI's "integration" and "empowerment" prompts and find them helpful for taking the first step.
*   **Hypothesis 4 (The Web3 Value)**: Users can understand and appreciate the value of "owning their own AI agent" and "putting growth experiences on-chain," and believe this constitutes a core advantage over Web2 products.

---

## 3. Target Audience for MVP

We will focus 100% on our "beachhead" users.

| User Persona | Description | Core Pain Points |
| :--- | :--- | :--- |
| **Developers troubled by the knowing-doing gap** | 1. Frequently get stuck in a "know I should, but don't want to start" dilemma with technical debt, complex refactoring, etc.<br>2. Are interested in tools that solve fundamental psychological obstacles and in the data sovereignty brought by Web3.<br>3. Are active in development environments like VS Code and have a basic understanding of crypto wallets. | 1. **Action Paralysis**: An important task is indefinitely postponed due to inner conflict.<br>2. **Mental Friction**: The constant struggle between "reason" and "emotion" consumes significant mental energy.<br>3. **Confidence Erosion**: Repeated failures to act erode self-efficacy, leading to self-doubt. |

---

## 4. MVP Scope Definition

### 4.1. Core Experience Loop: From "Knowing-Doing Gap" to "On-Chain Medal"

```mermaid
graph TD
    A[Knowing-Doing Gap<br>(e.g., want to refactor but can't start)] --> B(Start MyNearAI Session);
    B --> C{AI Guides Awareness of "Block"};
    C --> D[【Key Turning Point】<br>AI Guides Integration of Inner Conflict];
    D --> E(User Takes "Micro-Action"<br>e.g., writes the first comment);
    E --> F(User Returns to Work<br>and Completes Task);
    F --> G(Post-Session Review<br>"Let's talk about that breakthrough");
    G --> H(Mint "Growth Medal"<br>Turn experience into an on-chain SBT);
```

### 4.2. In-Scope Features

| Module | Feature | Notes |
| :--- | :--- | :--- |
| **Core Dialogue** | AI dialogue flow following the "Knowing-Doing Transformation SOP" | Strictly follows the "Awareness -> Integration -> Micro-Action -> Review" four-stage protocol. |
| **Web3 Wallet Integration** | NEAR Wallet Login | Users interact with the app via their own wallet, which serves as their decentralized identity. |
| **AI Agent** | Basic AI Agent | Upon login, the system deploys a basic, user-owned AI agent for the user. |
| **Growth Medal (SBT)** | Minting successful "knowing-doing transformation" experiences as Soul-Bound Tokens | Users can name their breakthroughs and record them as non-transferable on-chain credentials in their wallets. |

### 4.3. Out-of-Scope Features

*   Complex AI agent marketplace or customization features.
*   Complex tokenomics beyond SBTs.
*   All features outside the core loop: no community, no complex gamification, no growth reports, etc.

---

## 5. MVP Success Metrics

| Category | Core Metric | Target/Measurement |
| :--- | :--- | :--- |
| **Learning & Validation (Primary)** | **"Knowing-to-Doing Conversion Rate"** | **Core North Star Metric**. Measures the percentage of users who move from "starting a session" to "successfully taking a micro-action." |
| | **Qualitative Feedback** | Conduct in-depth interviews with at least 20 developer users to validate the model's effectiveness and the appeal of Web3 features. |
| **Web3 Value Validation** | **SBT Minting Rate** | The percentage of users willing to mint their successful transformation as a "Growth Medal" > 30%. |
| | **Repeat Usage Intention** | After a successful conversion, a survey asks about their willingness to use the tool again for similar issues, aiming for a score > 4.0/5.0. |
| **Basic Retention** | **D7 Retention** | 7-day retention rate for developer users > 10%. |

---

## 6. MVP Go-to-Market Strategy

| Strategy | Action |
| :--- | :--- |
| **User Acquisition** | **Precision Channels**: Targeted placement and content marketing in developer communities like VS Code Marketplace, GitHub, and Web3 developer communities (e.g., NEAR community). |
| **Core Narrative Strategy** | **Unified Hook**: All external communication will use "**Know you should, but can't? MyNearAI walks the first step with you.**" as the core selling point.<br>**Value Proposition**: Explain the core value as "helping you integrate inner conflicts and forge your growth into an on-chain medal." |

---

## 7. MVP Business Model

**Core features are free, with minor gas fees for advanced features (like minting SBTs).**

The sole goal of the MVP phase is to validate the core value, not to generate profit. Business model exploration will be deferred to later versions.