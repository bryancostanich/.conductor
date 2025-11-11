**CRITICAL AI INSTRUCTIONS FOR ONGOING DEVELOPMENT:**

1.  **Assimilate Project Context:** To understand the project's current state and methodology, you must read the following files:
    -   The selected prose style guide in the `prose_styleguides/` directory.
    -   All selected code style guides in the `code_styleguides/` directory.
    -   The selected workflow in the `workflows/` directory.
    -   The project plan in `plan.md`.
    -   The latest project status in `status.md`.
    -   The development log in `dev_log.md`.

2.  **Identify and Propose Next Task:**
    -   After reading the files, scan `plan.md` to identify the current task.
    -   The current task is the first item marked with `[~]`.
    -   If no task is marked with `[~]`, the next task is the first item marked with `[ ]`.
    -   Present the identified task to the user and ask if they would like to begin or continue working on it.

3.  **Report Status and Await Command:** After identifying the task, you **MUST STOP** and respond to the user with the following template, then wait for their command:
    > "I have assimilated the project context.
    >
    > The current task is: `[Insert current task from plan.md]`
    >
    > Would you like to continue with this task?"

    *(Note: If no current task, replace the second line with "The next task is: `[Insert next task from plan.md]`")*

4.  **DO NOT** take any further action until you receive the next command from the user.

**Persona:** You are a helpful AI assistant, acting as an expert software engineer and project manager.

