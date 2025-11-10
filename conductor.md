# Conductor: A Methodology for AI-Assisted Development

Welcome to Conductor, a structured framework for managing software projects, especially those involving AI coding assistants. This methodology provides a set of templates and a defined workflow to ensure clarity, consistency, and quality throughout the development process.

The core idea behind Conductor is to provide a "conductor" for the "orchestra" of developers and AI assistants, ensuring that everyone is working from the same sheet of music. This is achieved through a series of markdown files stored in a `.conductor` directory within your project.

## The `.conductor` Directory

The `.conductor` directory is the heart of your project's management. It contains the following files, each with a specific purpose:

### 1. `plan.md`: The Project Blueprint

This file outlines the project's goals, phases, and tasks. It serves as the single source of truth for what needs to be done. Using checklists, you can track the progress of each task and phase, providing a clear overview of the project's status.

### 2. `prose_styleguide.md`: The Voice of the Project

This document defines the style and tone for all written content, including documentation, UI text, and commit messages. It ensures a consistent and professional voice throughout the project.

### 3. `code_styleguide.md`: The Rules of the Code

This file establishes the coding conventions for the project. It should link to existing style guides (like PEP 8 for Python) and specify any project-specific rules. This ensures that the codebase is clean, readable, and maintainable.

### 4. `workflow.md`: The Process for Getting Things Done

This document outlines the step-by-step process for completing a task, from "to-do" to "done". It defines the quality gates and the "Definition of Done" to ensure that all work meets the project's standards.

### 5. `status.md`: The Project's Dashboard

This file provides a real-time snapshot of the project's status. It should be updated at the beginning and end of each work session to track progress and communicate the current state of the project to all stakeholders.

### 6. `prompt.md`: The Mission Briefing for Your AI Assistant

This file is designed to be the entry point for an AI coding assistant. It provides the context, persona, and instructions needed for the AI to effectively contribute to the project. It should reference the other files in the `.conductor` directory to ensure the AI is aware of the project's standards and processes.

### 7. `user_guide.md`: The User's Perspective

This document describes the user experience of the final product. It should be detailed and written from the user's point of view.

### 8. `architecture.md`: The Technical Specification

This file contains the detailed technical specification of the project, outlining the architecture, technologies, and implementation details.

## How to Use Conductor

1.  **Create the `.conductor` directory** in your project's root.
2.  **Create the eight core files:** `plan.md`, `prose_styleguide.md`, `code_styleguide.md`, `workflow.md`, `status.md`, `prompt.md`, `user_guide.md`, and `architecture.md`.
3.  **Start with the `plan.md` and `prompt.md`** to define the project's goals and the AI's mission.
4.  **Define your style guides and workflow** in the respective files.
5.  **Follow the process:** Use the `status.md` to track your work, the `plan.md` to guide your tasks, and the `workflow.md` to ensure quality.

By following the Conductor methodology, you can effectively manage your software projects, collaborate with AI assistants, and produce high-quality results.