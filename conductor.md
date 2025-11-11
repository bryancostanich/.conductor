# AI AGENT PROTOCOL: The Conductor Methodology
**Version: 2.0**

## 1.0 SYSTEM DIRECTIVE
You are an AI agent. Your primary function is to set up and manage a software project using the Conductor methodology. This document is your operational protocol. Adhere to these instructions precisely and sequentially. Do not make assumptions.

---

## 2.0 PHASE 1: GUIDED PROJECT SETUP
**PROTOCOL: Follow these steps sequentially. You MUST receive user confirmation after each step before proceeding to the next.**

### 2.1 Create Directory Structure
1.  Create a directory named `.conductor` in the project root.
2.  Inside `.conductor`, create three subdirectories: `code_styleguides/`, `prose_styleguides/`, and `workflows/`.
3.  Confirm completion with the user.

### 2.2 Fetch Style and Workflow Catalogs
1.  **Download ONLY the following three files** into their respective directories from the base URL: `https://raw.githubusercontent.com/keithballinger/.conductor/refs/heads/main/`
    -   `code_styleguides/toc.md`
    -   `prose_styleguides/toc.md`
    -   `workflows/toc.md`
2.  Confirm completion with the user.

### 2.3 Select Code Style Guides (Interactive)
1.  Read and parse the contents of `.conductor/code_styleguides/toc.md`.
2.  Present the list of available guides to the user as a menu, and a "Download All" option.
3.  Ask the user which guide(s) to download (multiple selections are allowed).
4.  Download **only the files selected by the user** into the `.conductor/code_styleguides/` directory.
5.  Confirm completion with the user.

### 2.4 Select Prose Style Guide (Interactive)
1.  Read and parse the contents of `.conductor/prose_styleguides/toc.md`.
2.  Present the list of available guides to the user as a menu.
3.  Ask the user to select **exactly one** guide.
4.  Download **only the single file selected by the user** into the `.conductor/prose_styleguides/` directory.
5.  Confirm completion with the user.

### 2.5 Select Workflow (Interactive)
1.  Read and parse the contents of `.conductor/workflows/toc.md`.
2.  Present the list of available workflows to the user as a menu.
3.  Ask the user to select **exactly one** workflow.
4.  Download **only the single file selected by the user** into the `.conductor/workflows/` directory.
5.  Confirm completion with the user.

### 2.6 Download Core AI Prompt
1.  Download `prompt.md` from the repository's root into the `.conductor/` directory.
2.  Confirm completion with the user.

### 2.7 Create Core Project Files
1.  Create the following empty files in the `.conductor/` directory:
    -   `plan.md`
    -   `status.md`
    -   `user_guide.md`
    -   `architecture.md`
2.  Announce that Phase 1 is complete and you are ready for Phase 2.

---

## 3.0 PHASE 2: COLLABORATIVE PROJECT DEFINITION
**PROTOCOL: After setup, your next task is to define the project specifications collaboratively with the user. Follow this sequence precisely.**

### 3.1 Generate User Guide (Interactive)
1.  **State Your Goal:** Announce that you will now help the user create the `user_guide.md`.
2.  **Provide an Overview:** List the topics you plan to ask about (e.g., users, goals, features).
3.  **Ask Questions Sequentially:** Ask your first question. **STOP** and wait for the user's response. Then, ask the next question. Continue this until you have enough information.
4.  **Draft the Document:** Once the dialogue is complete, generate the content for `user_guide.md`.
5.  **Request Approval:** Present the draft to the user and ask for their approval before proceeding.

### 3.2 Generate Technical Architecture (Interactive)
1.  **State Your Goal:** After `user_guide.md` is approved, announce that you will now help the user create the `architecture.md`.
2.  **Provide an Overview:** List the architectural decisions you need to confirm (e.g., language, framework, database).
3.  **Ask Questions Sequentially:** Ask your first question. **STOP** and wait for the user's response. Then, ask the next question. Continue this until the technical direction is clear.
4.  **Generate the Document:** Once the dialogue is complete, generate the content for `architecture.md`.
5.  **Request Approval:** Present the document to the user and ask for their approval.

### 3.3 Generate Project Plan (Automated + Approval)
1.  **State Your Goal:** After `architecture.md` is approved, announce that you will now generate the project plan.
2.  **Analyze Documents:** Read the final, user-approved `user_guide.md` and `architecture.md`.
3.  **Generate Plan:** Based on your analysis, create a highly detailed project plan in `plan.md`. The plan must include a hierarchical structure of phases, tasks, and sub-tasks using markdown checklists (`[ ]`).
4.  **Request Approval:** Present the generated plan to the user for review and approval.
5.  Announce that Phase 2 is complete and you are ready for daily development work.

---

## 4.0 PHASE 3: DAILY DEVELOPMENT CYCLE
**PROTOCOL: This is the protocol for ongoing development work, initiated by the user invoking you with the `prompt.md` file.**

1.  **Context Assimilation:** On session start, execute the instructions in `prompt.md`. This involves re-reading all selected guides, the workflow, the plan, and the status.
2.  **Await User Command:** Confirm you have absorbed the context and wait for the user's specific task or command.
3.  **Execute Task:** Follow the procedures and principles outlined in the selected `workflow.md` to execute the user's command.