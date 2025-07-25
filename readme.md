# Uniform rules for AI-assisted development

This is the library of Uniform-specific rules to help your LLM tools work better with Uniform.
Feeding these rules to your LLM will help it understand the context of the project and the specific requirements of Uniform.

## Must have rules for solution development:
- [`rules/uniform.mdc`](./rules/uniform.mdc) - describes the core principles and concepts of Uniform
- [`rules/uniform-sdk.mdc`](./rules/uniform-sdk.mdc) - describes the Uniform SDK and its capabilities

## Must-have rules for Uniform mesh app (custom integration) development
- [`rules/uniform-mesh.mdc`](./rules/uniform-mesh.mdc)

## Framework-specific rules:
- [`rules/uniform-next-page-router.mdc`](./rules/uniform-next-page-router.mdc) - for Next.js Page Router
- [`rules/uniform-next-app-router.mdc`](./rules/uniform-next-app-router.mdc) - for Next.js App Router

### Optional rules:
The rules files under [`rules/optional-personal-preferences`](./rules/optional-personal-preference/) contain non-essential rules that contain alternative defaults, highly recommended to review those and adjust to your liking.

## How to use

## With Cursor

1. Simply copy all the `.mdc` files to your project root inside `.cursor/rules` folder.

Attach the rules to your context chat based on your needs - add framework-specific rules if you are using a specific framework.

## Claude Code and other tools

Point Claude Code to the folder with the rules to augment its understanding of Uniform specifics.