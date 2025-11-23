# .conductor: An AI-Driven Project Management Framework

Welcome to Conductor, a structured system for managing software projects with an AI agent like the Gemini CLI.

The core philosophy is to provide the AI with a clear, unambiguous **protocol** to follow, turning it from a simple coding assistant into a proactive project manager. This system ensures a consistent, high-quality development process from initial setup to daily work.

Conductor works by working with you to create a set of Markdown files that describe, and become, the authoritative plan of record, conceptually similar to a specification, and these files become the guardrails that guide your AI agents (used by Conductor) to build and maintain your project or solution.

## How It Works

The Conductor methodology is divided into two main phases:

1.  **Phase 1: Guided Setup:** A one-time, interactive process where the AI acts as a setup wizard. It scaffolds the project structure, helps you select the appropriate style guides and workflows, and creates the core project management files.
2.  **Phase 2: Daily Development:** For all subsequent interactions, the AI uses the `.conductor/prompt.md` file to re-assimilate the project's context and rules, ensuring it always adheres to the established workflow for every task.

---

## Getting Started

Conductor can be launched and used one of two ways, the recommended way is to install it as a registered extension within the Gemini CLI. It can also be called from Gemini manually, via prompting.

### Installing and Registering the Extension

#### Prerequisites

1. To install as a Gemini extension, first make sure you have the [Gemini CLI](https://geminicli.com/) installed.
2. Because there is not a published executable, you will also need to clone this Conductor repo locally.

#### Registering

Once the Gemini CLI is installed and the Conductor repo has been cloned, you can register Conductor as an extension via the following termina command:

```bash
gemini extensions link [path to conductor_repo]/extensions/conductor
```

### Launching Conductor

Conductor can be launched within Gemini using one of two commands:

* `/conductor:init` - Used the first time to initialize your project.
* `/conductor:resume` - Used to open an existing conductor project.

#### Initializing a Project 

To create a new Conductor project, navigate to the root directory of where you want to create your project, if you're using Git, this would typically be your repo directory.

1. Launch Gemini:
    ```bash
    gemini
    ```

2. Lauch the Conductor project initialization by executing the following command in the Gemini CLI window:
    ```bash
    /conductor:init
    ```






**Launch the Gemini CLI with the following command:**

Alternatively, you can manually prompt gemini:

```bash
gemini -i "I want to set up this project using the Conductor methodology. Your instructions are in the file located at https://raw.githubusercontent.com/keithballinger/.conductor/refs/heads/main/conductor.md. Download that file with curl, then read it. Then begin the setup process as outlined in that file." --yolo --model "gemini-2.5-pro"
```

### Daily Development Workflow

After the initial setup is complete, use this prompt **every time** you start a new work session. It directs the AI to read the local `prompt.md` file, understand the project's context, and prepare for the day's tasks.

**Using the Extension**

Launch Gemini
```bash
gemini
```

In the gemini chat window type:
```bash
/conductor:resume
```

**Launch the Gemini CLI with the following command:**

```bash
gemini -i "Start my development session by following the instructions in .conductor/prompt.md." --yolo
```

---

## Core Files

-   **`conductor.md`**: The master protocol file used only for the initial project setup.
-   **`prompt.md`**: The entry point for all daily development sessions.
-   **`plan.md`**: The AI-generated, human-approved project plan with phases and tasks.
-   **`code_styleguides/`**: Contains the selected code style guides for the project.
-   **`prose_styleguides/`**: Contains the selected prose style guide for all written content.
-   **`workflows/`**: Contains the selected workflow protocol that the AI must follow for all tasks.
