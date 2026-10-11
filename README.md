# PROJECT VAJRA V4 — Engineering Workbench

V4 is a standalone browser simulator for engineering learning and early process-model prototyping.

## Modules
- Three.js orbit/zoom machine concept view.
- Injection process recipe with screw-area, estimated stroke, volumetric flow and cycle-time calculations.
- Hydraulic power, equivalent cylinder force and efficiency estimates.
- Preliminary clamp-force check from cavity pressure × projected area × margin.
- Five barrel-zone setpoints with discrete-time PID calculation and illustrative thermal dynamics.
- Simplified PP cooling energy balance and cooling-water capacity estimate.
- Editable PLC-style sequence timing, I/O monitor, start/stop/reset, simulated fault injection, and event log.

## Run
Open `index.html` in a modern browser with internet access. Three.js is loaded from jsDelivr, so an offline copy needs the library bundled locally.

## GitHub Pages
Upload `index.html`, `style.css`, `app.js`, and this README to a repository root. Enable GitHub Pages from Settings → Pages.

## Model scope and safety
All machine motion and control logic are simulated. Values and equations are simplified assumptions rather than a validated model of a particular Woojin 2500T press. The clamp tonnage check and cooling estimate are screening calculations only. Validate calculations with actual machine manuals, cylinder/linkage data, resin datasheets, mold geometry, mold-flow/thermal analysis, and qualified engineers before using them in production. This website must never be used as a real-machine safety controller.


## VAJRA AI Assistant
Added an on-page local engineering Q&A helper with suggested questions for recipe, hydraulics, PID and alarms. It uses current simulator inputs with rule-based response templates. A cloud LLM is not connected yet; user questions stay in the browser. It must not control or be connected to a real molding machine.
