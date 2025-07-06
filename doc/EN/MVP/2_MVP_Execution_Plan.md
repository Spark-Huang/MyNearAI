# MyNearAI MVP Execution Plan (Web3 Edition)

> **Version**: 1.0
> **Date**: 2025-07-06
> **Status**: Active
> **Related Documents**: `MyNearAI_Product/EN/MVP/0_MVP_Strategy_and_Goals.md`, `MyNearAI_Product/EN/MVP/1_MVP_Product_Requirements_Document.md`
> **Abstract**: This document serves as the action manual for the MyNearAI MVP phase, detailing the technology stack, development schedule, user recruitment, and feedback collection process, aiming to ensure the project efficiently and orderly achieves its Web3 strategic goals.

---

## 1. Project Roles & Responsibilities

| Role | Core Responsibilities |
| :--- | :--- |
| **Product Owner** | Responsible for the final success of the MVP; defines and manages the product backlog; ensures development work aligns with strategic goals. |
| **Tech Lead** | Responsible for overall technical architecture design; ensures code quality and project technical feasibility; solves key technical challenges. |
| **Smart Contract Dev** | Responsible for the development, testing, and deployment of the SBT contract; ensures the security and efficiency of on-chain logic. |
| **Frontend/DApp Dev** | Responsible for the DApp's UI implementation, interaction logic with wallets and smart contracts, and user experience. |
| **Backend/Integration Dev** | Responsible for integration with AI models and decentralized storage; provides necessary API services for the DApp. |
| **UX/UI Designer** | Responsible for providing simple, efficient interface designs and smooth interaction prototypes that appeal to Web3 users. |
| **Community/Eco Ops** | Responsible for recruiting and managing the developer angel user community; organizing user interviews and feedback collection; liaising with NEAR ecosystem resources. |

---

## 2. Technology Stack

| Domain | Technology/Service | Rationale |
| :--- | :--- | :--- |
| **Client Framework** | **React / Vue / Svelte** | Mainstream front-end frameworks with mature Web3 library support, facilitating rapid DApp construction. |
| **Blockchain Platform** | **NEAR Protocol** | Low cost, high speed, developer-friendly, its sharding technology and WebAssembly support are well-suited for complex AI applications. |
| **Smart Contract Language** | **Rust** | The preferred language for NEAR smart contracts, known for its safety, performance, and reliability. |
| **Decentralized Storage** | **IPFS / Arweave** | Used for storing SBT metadata and visual assets, ensuring the permanence and immutability of the assets. |
| **AI Model Service** | **[TBD] (e.g., OpenAI API, Gemini API)** | In the MVP phase, prioritize using mature third-party APIs to quickly validate the core dialogue flow. The long-term goal is to integrate with decentralized AI compute networks. |
| **AI Implementation** | **Composable Agents + RAG** | Adopt an open-source, composable agent architecture. The RAG knowledge base can be stored on IPFS and co-maintained by the community to improve the quality and transparency of AI dialogues. |
| **Deployment** | **Vercel / Fleek / Spheron** | Provide simple and fast decentralized front-end deployment and hosting services. |
| **Team Collaboration** | **GitHub, Notion, Discord** | Used for code management, document collaboration, and instant communication. |

---

## 3. Development Schedule

We will adopt a **seven-week** agile development cycle.

### **Sprint 0: Core Experience Validation (0.5 weeks)**
*   **Goal**: To validate the effectiveness of the "inner integration to knowing-doing transformation" dialogue flow at the lowest cost before committing engineering resources.
*   **Core Tasks**:
    *   Conduct "Wizard of Oz" testing with 5-10 target developer users, where a human simulates the AI in the background.
    *   Validate and iterate on the "AI Dialogue Design SOP," collecting initial "golden dialogue data."
*   **Core Output**: A "Wizard of Oz Test Insights Report" to inform prompt design and AI model selection.

### **Sprint 1: Foundation and Safety Baseline (1.5 weeks)**
*   **Goal**: Complete the core architecture, smart contract development, and **ensure the project meets basic ethical and on-chain security baselines**.
*   **Smart Contract Tasks (High Priority)**:
    *   Complete the writing and unit testing of the "Integration Crystal" SBT contract.
    *   Deploy the contract to the testnet and conduct interaction tests.
*   **Backend Tasks (High Priority)**:
    *   Implement the minimum viable crisis intervention logic.
    *   Complete the integration with the AI model API.
*   **Frontend Tasks (High Priority)**:
    *   Develop the crisis intervention UI page.
    *   Set up the DApp project framework and connect to the NEAR wallet.
    *   Complete the static UI layout of the core dialogue interface.

### **Sprint 2: Core Loop (1.5 weeks)**
*   **Goal**: Integrate the front-end, back-end, and smart contract to achieve a complete "knowing-doing gap to on-chain proof" core experience loop.
*   **Tasks**:
    *   Implement real-time dialogue functionality.
    *   Implement the full interaction logic of "perceiving the block -> integrating the conflict -> taking micro-action."
    *   Implement the "Integration Crystal" SBT minting process (calling the contract, user signing, UI updates).
    *   Develop a user profile page to display their owned SBTs.

### **Sprint 3: Optimization and Audit (3.5 weeks)**
*   **Goal**: Optimize the experience, fix bugs, complete the contract audit, and prepare for internal release.
*   **Tasks**:
    *   Joint debugging of front-end and back-end to optimize performance and AI response speed.
    *   **Submit the smart contract to a third party for a security audit**.
    *   Conduct comprehensive internal testing and fix all critical bugs found.
    *   Build the first DApp version for internal use.

---

## 4. Angel User Recruitment & Ops Plan

*   **Core Goal**: To identify and establish deep, cooperative relationships with 10-20 "core contributors" who align with the Web3 philosophy.
*   **Communication Stance**: Adopt the stance of an "open-source project" rather than a "commercial product," maintaining humility, sincerity, and openness.
*   **Recruitment Steps**:
    1.  **Prepare Materials (Sprint 2)**: Write sincere recruitment copy aimed at co-builders, with the core hook: "Know you should, but can't? Come mint your first growth medal."
    2.  **Channel Distribution (Sprint 3)**: Publish recruitment information in developer communities on GitHub, Twitter, and NEAR-related platforms (like DevForum, Discord).
    3.  **User Screening & Communication (Pre-launch)**: Create an angel user communication group (e.g., a Discord channel) and identify potential core contributors from it.

---

## 5. Testing & Feedback Collection Process

*   **Goal**: To systematically collect user feedback to provide data support for validating core hypotheses.
*   **Steps**:
    1.  **Launch**: Release the DApp link to the entire angel user group.
    2.  **Data Analysis**: Analyze core metrics such as "Knowing-to-Doing Conversion Rate," SBT Minting Rate, and D7 Retention.
    3.  **Surveys**: After one week of user experience, distribute surveys to quantitatively assess the tool's value and the appeal of its Web3 features.
    4.  **In-depth Interviews**: Select 5-10 active and churned users each for 30-minute one-on-one in-depth interviews.
    5.  **Feedback Synthesis & Analysis**: Consolidate all data to form an "MVP Test & Learnings Report," clarifying whether core hypotheses have been validated and providing a basis for the next iteration.

---

## 6. Appendix: Long-Term Technical Roadmap Considerations

*   **Decentralized AI Network**: In the long term, the project should gradually transition from relying on centralized AI APIs to integrating with decentralized AI compute networks (like Bittensor, Ritual) to achieve true end-to-end decentralization.
*   **Community-Owned Model**: With the high-quality anonymous feedback data collected, the community could co-fund the training of a proprietary, open-source "knowing-doing unity" model on a decentralized AI training platform (like Gensyn), with ownership belonging to a community DAO.