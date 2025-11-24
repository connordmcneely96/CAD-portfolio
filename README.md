# SolidWorks Project Template

## Overview
Provide a concise summary of the project scope, main assemblies, and intended use cases. Mention any unique design features worth highlighting.

## Engineering Goals
- List measurable performance targets (e.g., mass, stiffness, factor of safety).
- Note key functional requirements and acceptance criteria.

## Materials
- Enumerate materials per major component or subassembly.
- Include material standards (e.g., 6061-T6, 17-4 PH) and surface treatments.

## Design Constraints
- Manufacturing constraints (DFM/DFA notes, minimum wall thicknesses, draft angles, tolerances).
- Assembly constraints (fastener sizes, torque specs, clearance/interference fits).
- External constraints (regulatory standards, environmental loads, budget).

## CAD Workflow
1. Sketch and parameter planning: list main reference planes, global variables, and key dimensions.
2. Part modeling: describe feature order and patterning strategy.
3. Assembly structure: describe top-level assemblies, subassemblies, and mates used.
4. Drawing creation: note title block standard, revision scheme, and annotation conventions.
5. Export pipeline: detail how STEP/STL/GLTF exports are generated and validated.

## Render Gallery
Add rendered images to `/renders` and reference them here using relative paths:
- `![Render 1](renders/render1.png)`
- `![Render 2](renders/render2.jpg)`

## Assembly Notes
- Summarize exploded view steps or critical assembly sequences.
- List hardware kits, torque specs, and alignment notes.
- Mention any configurations or design tables that affect assembly.

## Drawings and Exports
- Native CAD: `/cad_source`
- PDF drawings: `/drawings`
- STEP exports: `/exports/step`
- STL exports: `/exports/stl`
- GLTF/GLB exports: `/exports/gltf`
- Renders: `/renders`

## How to Open
1. Clone this repository.
2. Ensure SolidWorks version compatibility (note required version and add-ins).
3. Open the top-level assembly file (.SLDASM) from `/cad_source`.
4. Update references if files are relocated.

## Version Control Notes
- Large binary CAD assets are tracked with Git LFS. Ensure `git lfs install` has been run before cloning or committing.
- Keep parametric changes documented via revision history in drawings and commit messages.
- Avoid embedding large simulation results; link to external storage if needed.

## Contributing
1. Branch from `main`.
2. Add or update CAD files in the appropriate folders.
3. Run `git lfs track` for any new binary CAD formats.
4. Validate exports and renders before opening a pull request.
5. Follow the existing revision and naming conventions for parts and assemblies.
