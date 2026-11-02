# EA Repository Foundation

Archi template for the **Architecture Foundation** of an Architecture Repository based on the **TOGAF® Standard, 10th Edition**, modeled in **ArchiMate® 3.2**.

It provides the reusable, project-independent part of the repository: a reference metamodel, views organized along the TOGAF ADM, and guides for every TOGAF artifact (catalogs, matrices, tables and diagrams). It is designed to be used together with the companion **EA Repository Landscape** template, which holds the architecture of the enterprise itself.

> **Version:** 2.0 &nbsp;·&nbsp; **Tool:** [Archi](https://www.archimatetool.com) 5.x &nbsp;·&nbsp; **Collaboration:** coArchi plugin

---

## What's inside

### Architecture Metamodel
- One sample element for each ArchiMate 3.2 element type (60 elements), each with its definition.
- 139 typical relationships between them, all compliant with the ArchiMate 3.2 relationship rules (Archi Validator: no warnings).
- Element folders organized by layer and by element type, ordered *active structure / behavior / passive structure*.

### Metamodel views, ordered along the TOGAF ADM

| View | Content |
|---|---|
| 00 Overview | Layered view of the key element types and essential relationships |
| 01 Preliminary | Stakeholders, drivers, principles, goals |
| 02 – 10 | One view per ADM phase, from Phase A (Architecture Vision) to Phase H (Architecture Change Management); Phase C is split into Data and Application Architecture |
| 11 Requirements Management | Requirements realization and meanings |
| 99 Complete Metamodel | Complete reference view, organized by layer |

Layout convention: within each layer, active structure on the left, behavior in the center, passive structure on the right; Motivation on the right; Physical Extension below Technology.

### Reference Library – TOGAF Artifact Guides
74 guide views, one per TOGAF artifact, grouped by ADM phase and named `<phase>-<type><number>`:

- **Phase:** `P` Preliminary, `A`, `B`, `CD` (Phase C Data), `CA` (Phase C Application), `D`, `E`, `F`, `R` (Requirements Management)
- **Type:** `C` Catalog, `M` Matrix, `T` Table, `D` Diagram

Each guide describes the purpose of the artifact, the ArchiMate viewpoint to use (or how to produce it from the model), the main elements and relationships, the typical stakeholders and where to store the result in the Landscape model. It carries the properties `TOGAF Artifact`, `ADM Phase`, `Artifact Type`, `ArchiMate Viewpoint` and `Reference` (link to the relevant section of the TOGAF Standard online).

### Standards Library
Empty folders, ready for external standards and reference architectures.

---

## Getting started

### Use it as a template
1. Download the `.architemplate` file from the latest [Release](../../releases).
2. In Archi: **File › New › New Model from Template…** and select the downloaded file.
3. Rename the model (`<Organization> - <Project name> - Foundation`) and replace the placeholders in the model *Purpose* and properties (`Organization`, `Project`, `Model Owner`).
4. Read the **Read Me** view in the model.

### Work on the template itself
1. Install the **coArchi** (Collaboration) plugin in Archi.
2. **Collaboration › Import Remote Model to Workspace…** with the URL of this repository.
3. Use a GitHub Personal Access Token as password.

---

## Conventions

- All names, documentation and notes are written in English.
- Element names: singular, Title Case. Relationship names are left empty unless they add meaning.
- Every element and every folder carries a documentation text.
- Only ArchiMate 3.2 compliant relationships; run the Archi Validator before each release.

## Versioning

The Foundation and Landscape templates are released together and share the same version number. See [CHANGELOG](CHANGELOG.md) for the history of changes.

---

## License

This work is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You may share and adapt it, including for commercial purposes, provided you give appropriate credit.

**Third-party content.** The definitions of the ArchiMate elements and some folder descriptions are taken from the *ArchiMate® 3.2 Specification* and the *TOGAF® Standard, 10th Edition*, © The Open Group. They are reproduced for reference with their source and are **not** covered by the CC BY 4.0 license. The TOGAF artifact guides link to the TOGAF Standard published by The Open Group at [pubs.opengroup.org](https://pubs.opengroup.org/togaf-standard/).

ArchiMate® and TOGAF® are registered trademarks of The Open Group. This project is not affiliated with or endorsed by The Open Group.

## Author

Olivier Sabbe – Enterprise Architect
