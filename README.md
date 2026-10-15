# Block Based Learning MVP

A dependency-free local implementation of the Block Based Design Wireflow in Figma:
https://www.figma.com/design/wjmpRHIVoQJ8meJTM8oKyy/Block-Based-Design-Wireflow

## Run

Requires Node.js 18 or newer. No package installation is needed.

```sh
npm start
```

Open http://localhost:5173 and select **Explore the demo**.

## Included

- Landing page and demo student profile onboarding.
- Home, course catalog, assessments, and sections placeholder.
- SSD, sequence, UML, domain model, and free practice workspaces.
- Three independent sample questions per course.
- Add, drag, keyboard-move, edit, delete, and undo diagram components.
- Connect components with request and return relations.
- Local autosave, structural feedback, submission snapshots/history, and JSON export.
- Locally downloaded Figma assets, gray panel tokens, and blue active states.

Use the relation button, then select a source and target. Double-click a component or select it and choose **Edit selected**. Entities accept one attribute per line. Arrow keys move a focused component; Enter edits it.

## MVP boundaries

All profile data, work, and submissions remain in this browser's local storage. This is a single-user demo, not secure authentication. No passwords are requested. Institutional SSO, instructor sections, backend persistence, grading, semantic validation, collaboration, and production account management are not implemented. Sample scenarios replace the outline's placeholder assignment text. Structural feedback only checks for components, a relation, and reasoning; it does not establish answer correctness.

## Validation

`npm run check` checks JavaScript syntax. Browser verification covered demo entry, course navigation, connection creation, submission, switching questions, and answer persistence after reload.
