# Conceptual Overview

## Purpose

This document explains how Vínculo is structured as a system.

Vínculo is a network that represents how people are connected through shared work.  
This overview focuses on how those connections are formed, how the network is modeled, and how its components relate to each other.

---

## The core rule

All connections in Vínculo follow a single constraint:

**People do not connect directly.  
They connect through shared participation in a project or organization.**

This rule defines the structure of the network.

---

## Node types

Vínculo operates with three node types:

- **Person** — an individual participant  
- **Project** — a bounded instance of work  
- **Organization** — an ongoing structure  

Projects may include types (e.g. interview, event, publication, series), but these do not introduce additional node types.

A series is treated as a project that can contain other projects.

---

## Relationships

Connections are defined through participation:

- A person contributes to a project  
- A person is part of an organization  
- A project may exist within an organization  

These relationships form the edges of the network.

Each edge includes a **role**, which describes how the connection exists (e.g. editor, member, contributor).


## Diagram — Network Structure

Person  
   │ (role: editor, participant, etc.)  
   ▼  
Project  
   │ (belongs to)  
   ▼  
Organization  

Multiple people connect through the same project:

Person ──(role)──> Project <──(role)── Person

   
---

## Network structure

The network is a graph composed of:

- nodes (people, projects, organizations)  
- edges (relationships defined by roles)  

There are no direct edges between people.

All paths between individuals pass through one or more intermediate nodes.

---

## Traces

A connection between two people can be understood by tracing a path through the network.

A trace consists of:
- a sequence of nodes  
- the roles that define each step  

This allows the system to explain how two individuals are connected through shared participation.

---

## Growth of the network

The network grows through user contribution:

- users add projects or organizations  
- participants are named and assigned roles  
- new nodes are created when needed  

Unclaimed participants appear as ghost nodes and can later be claimed.

## Diagram — User Flow

Invite → Peek → Claim → Expand → Contribute

[Invite]
   ↓
User receives email and opens map

[Peek]
   ↓
User sees themselves already connected to a project
Limited exploration

[Claim]
   ↓
User verifies identity and confirms role

[Expand]
   ↓
Full network becomes visible

[Contribute]
   ↓
User adds a project and names collaborators

---

## Summary

Vínculo is structured as a graph where:

- connections are indirect  
- relationships are defined by roles  
- participation is the basis of all links  

The system represents collaboration as a structured network rather than a set of direct relationships.