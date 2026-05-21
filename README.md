# Threat Modeling Studio

Threat Modeling Studio is a single-file, browser-based threat modeling tool for drawing diagrams, capturing threats, generating reports, and exporting diagrams for review.

## Features

- Drag-and-drop diagramming for common threat model elements: processes, data stores, external entities, actors, trust boundaries, and notes.
- Data flow editing with selectable ports, curved connections, and edge controls.
- Threat tracking with STRIDE classification, DREAD scoring, and risk levels.
- Report view with filtering, sorting, and export options.
- JSON import/export for diagram state.
- PNG export for sharing diagrams outside the app.
- Multiple model tabs in one workspace.
- Dark and light themes, plus a toggle for the background grid.
- Optional AI analysis panel for generating threat suggestions and remediation guidance.

## Getting Started

1. Open [tmapp.html](/workspaces/tmapp/tmapp.html) in a modern browser.
2. Create a model or use the default example diagram.
3. Drag items from the toolbox onto the canvas.
4. Connect nodes by enabling edge mode and selecting ports.
5. Add threats, review the report, or export the model when you're done.

## Common Actions

- Add a node by dragging from the toolbox.
- Move nodes by dragging them on the canvas.
- Resize trust boundaries and note cards with the on-canvas handles.
- Switch between Diagram, Threats, Report, and AI Analysis using the top bar.
- Use Import and Export to move model data between machines or sessions.
- Use PNG Export to create a static diagram image.

## AI Analysis

The AI Analysis panel can inspect the current diagram and suggest threats, controls, and remediation priorities. If you use it, provide an API key in the UI and choose the provider/model you want to use.

## Project Structure

- [tmapp.html](/workspaces/tmapp/tmapp.html) - the full application, including markup, styling, and client-side logic.
- [README.md](/workspaces/tmapp/README.md) - project overview and usage notes.

## Notes

- The app runs entirely in the browser; no build step or backend is required.
- Saved model state lives in browser storage unless you export it manually.
- The app uses remote Google Fonts, so an internet connection is needed for the intended typography.