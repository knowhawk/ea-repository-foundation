# Changelog

All notable changes to the EA Repository Foundation are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project uses [Semantic Versioning](https://semver.org/). The Foundation and the Landscape are released under the same version number.

## [2.0] - Unreleased

First release as an Archi model (Archi 5.10, coArchi), migrated from the Sparx Enterprise Architect template v1.x.

### Added
- Architecture Metamodel: one generic element per ArchiMate 3.2 element type (60), each with its definition, and about 140 relationships compliant with ArchiMate 3.2, organized in folders by layer and type.
- Metamodel views per ADM phase: 00 Overview (Layered viewpoint), 01 Preliminary, 02 Phase A to 10 Phase H (Phase C split into Data and Application), 11 Requirements Management, 99 Complete Metamodel.
- Reference Library – TOGAF Artifact Guides (74): one guide view per TOGAF artifact, organized by phase and named `<phase>-<type><number>`, describing purpose, viewpoint or production method, elements and relationships, stakeholders and storage location in the Landscape.
- Guide properties: TOGAF Artifact, ADM Phase, Artifact Type, ArchiMate Viewpoint, Reference.
- Reference Library – Stakeholder Catalogue: generic stakeholders and their concerns (Stakeholder associated with Driver), to be adapted per project.
- Standards Library: empty folders for external standards and reference architectures.
- Read Me view, Purpose and generic model properties (Organization, Project Name, Name, Template Version).
- Lifecycle Status property for elements and relationships (Planned, In Implementation, Active, Phasing Out, Retired), documented in the Read Me view (Properties section).
- Change Reference property for planned and retiring content.
- Pull request template (`.github/pull_request_template.md`).
- Distribution as an Archi model template (`.architemplate`).

### Changed
- Relationships not compliant with ArchiMate 3.2 removed.
- Path modeled as an element.
- Relationships added: Deliverable realizes Requirement; Assessment associated with Deliverable; Business Service realizes Requirement; Application Service realizes Requirement.
- Concern modeled as a Driver associated with a Stakeholder; findings on the situation modeled as Assessments associated with the Driver.
- Documentation reviewed and corrected for every element and folder.

### Removed
- Glossary and acronyms: moved out of the model to a separate JSON glossary.
- Example content: moved to a separate example model.

## [1.x] - Legacy

Sparx Enterprise Architect template (EARepositoryTemplate_20260216). No longer maintained; superseded by version 2.0.
