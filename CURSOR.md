# Cursor Setup

## Installation

Copy the rules file to your project:

```bash
cp .cursor/rules/product-manager-guidelines.mdc your-project/.cursor/rules/
```

The rules apply automatically when you open the project in Cursor (`alwaysApply: true`).

## Manual Setup

1. Open Cursor Settings
2. Navigate to **Rules**
3. Add a new rule file or paste the contents of `.cursor/rules/product-manager-guidelines.mdc`

## Usage

The guidelines activate automatically in every Cursor session within the project. They guide the AI assistant to:

- Start with the user problem before proposing solutions
- Write specs that engineers and designers can act on immediately
- Require success metrics before generating implementation artifacts
- Default to minimum viable scope
- Distinguish evidence from assumption
- Format stakeholder communications for the appropriate audience

## Customization

Edit the `.mdc` file to adjust the guidelines for your team's specific conventions, frameworks, or artifact templates.
