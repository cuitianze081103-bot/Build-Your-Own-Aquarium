# Repository instructions

## Branch workflow required by the project owner

- Before editing project files, create or switch to a dedicated `codex/<task>` branch.
- Commit and push all agent changes to that branch, never directly to `main` or `master`.
- Use `codex/setup-aquarium` for the initial source import.
- Open a pull request against `main` with a concise description and relevant validation.
- Do not merge pull requests or change the default branch without the owner's explicit request.
- Do not force-push, delete branches, or change repository visibility without explicit authorization.
- If the default branch or remote changes, inspect the actual repository state before proceeding.

## Aquarium requirements

- Keep all visible webpage text in English.
- Preserve the current first-version side-view aquarium and six-step interaction flow unless the owner requests a change.
- Keep the sand tool background transparent; drawing its icon over the tank must not clear the tank canvas.
- Keep pointer, touch, keyboard, responsive layout, and reduced-motion behavior usable.
- Keep authentication credentials, personal files, reference videos, generated variants, and scratch files out of the repository.

## Validation and delivery

- Run `npm run check` for JavaScript syntax changes and `npm test` for interaction/state changes.
- Check the page visually when layout or rendering changes.
- Report the working branch, pull request, and relevant checks to the owner.
- Deployment and public access are separate actions. Do not change hosting permissions merely to deploy a branch.
