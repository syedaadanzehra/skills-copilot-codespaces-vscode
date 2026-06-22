# Setup

## What this repo is

This is a **GitHub Skills** interactive exercise — *"Code with GitHub Copilot."* It teaches you to use GitHub Copilot's AI code suggestions inside VS Code and Codespaces. There is no application to build; progress is driven by GitHub Actions workflows in `.github/workflows/`, with step content in `.github/steps/`. As you complete each step, an action advances the README to the next one.

## Getting the dev environment running

You work through this exercise in a **Codespace** (a cloud VS Code) — no local toolchain required.

1. Create the dev container so Copilot loads automatically. Add `.devcontainer/devcontainer.json`:
   ```json
   {
       "name": "Codespace for Skills!",
       "customizations": {
           "vscode": {
               "extensions": ["GitHub.copilot"]
           }
       }
   }
   ```
2. Commit it to `main`.
3. Click **Code → Codespaces → Create codespace on main** and wait ~2 minutes for it to spin up.
4. Confirm the `GitHub.copilot` extension appears in the VS Code Extensions sidebar.

> Requires an active GitHub Copilot subscription on your account.

## Working through the exercise

- Follow the instructions in the repo's **README**, which updates itself as you complete each step.
- Several steps ask you to `git pull` in the Codespace terminal before continuing — do this so the workflows can grade your progress.
- Step files live in `.github/steps/`; the grading logic lives in `.github/workflows/`.
