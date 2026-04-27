# Vínculo

> **Note:** This repository is part of the SE_07 Technical Documentation module at Code University Berlin.  
> The project was initially developed around a different system (VITRO) and later pivoted to Vínculo to better align with my personal work.  
> Earlier drafts are preserved as part of the documentation process.


### A network where connection requires a shared thing

Vínculo is an invite-only network that maps how people are connected through the projects and organizations they have actually contributed to.

You cannot connect to a person in Vínculo.

Every connection must pass through something tangible, a project, a publication, an event, or an organization. No shared thing, no edge.

---

## Core idea

Most platforms define connection as proximity, following, endorsing, or linking.

Vínculo defines connection as participation.

If two people did not take part in the same thing, they are not connected.

---

## The model

Vínculo is a graph with three node types:

- **Person** — someone who contributed  
- **Project** — a bounded thing that was made  
- **Organization** — an ongoing entity with members  

Connections are defined by roles:

- Person → Project (`writer`, `editor`, `participant`)
- Person → Organization (`member`, `contributor`)
- Project → Organization (`belongs_to`)

There are **no direct person-to-person edges**.

---

## Key feature

Vínculo can trace the path between two people through shared projects and organizations, and explain that connection in human language.

---

## What makes it different

- No profiles to build  
- No followers or endorsements  
- No scraping or auto-generated data  
- Every node is named through real participation  
- Credit is distributed across everyone involved  

---

## Status

This repository contains the technical documentation for the system and its concept prototype.

---

## Prototype

The interactive prototype can be accessed by opening:

- [index.html](index.html)

To view it:
- download or clone the repository  
- open `index.html` in any web browser  

The prototype demonstrates how users explore connections through shared projects and organizations.
The prototype is a conceptual artifact used to explore and validate the system design described in this documentation.

---

## Documentation

- **Docs folder**: [`/docs`](docs/)
- [Proto Persona](docs/personas.md) who this is for  
- [User Story](docs/user-story.md) what they are trying to do  
- [Procedural Guide](docs/procedural-guide.md) how to enter and use Vínculo  
- [Conceptual Overview](docs/conceptual-overview.md) what Vínculo is and why it exists  
- [Glossary](docs/glossary.md) key terms  
- [Contributing](docs/contributing.md) how to propose edits  

---

*SE_07 Technical Documentation — Code University Berlin*
*Project by Mercedes Torrendell*