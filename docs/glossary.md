# Glossary

A shared vocabulary for Vínculo. Terms are listed alphabetically and grouped by what they describe.

---

## Network terms

### Node
An entity in the network. Can be a Profile, Project, or Organization. Profiles never connect directly, every connection routes through a Project or Organization node.

### Edge
A connection between two nodes, defined by participation. Three types exist: `created` (Profile → Project), `part_of` (Profile → Organization), `belongs_to` (Project → Organization).

### Trace
The path between two people through shared projects and organizations. The trace is computed at query time and shown with an editorial explanation of how the connection formed.

### Bridge node
A Project or Organization that connects otherwise separate clusters of people. Used in the analytics layer as a proxy for structural importance, replacing the role that follower counts play in conventional platforms.

---

## People & participation

### Profile
A person's node in the network. A Profile is included because the person participated in something — not because they performed or posted.

### Role
The function a person had within a project or organization (lead, contributor, collaborator, member, editor). Roles are stored on the edge, not the node, because the same person can hold different roles in different contexts.

### Participation
The act that creates an edge. Someone is in the network because they took part in a project or belonged to an organization. Participation, not declaration, is what makes a connection real in Vínculo.

### Co-author
Anyone who shaped a piece of work, regardless of whether their name appears on the final output. Vínculo treats co-authorship as a structural fact (you were part of the project) rather than a credit hierarchy.

### Credit
The visible record of who contributed to a project. In conventional platforms, credit is uneven, one name surfaces and others disappear. Vínculo represents credit as a graph: every named participant is a visible node.

---

## Project lifecycle

### Project
A bounded instance of work with defined participants. Has a start date, sometimes an end date, and at least one Profile linked to it through the `created` edge.

### Organization
An ongoing entity that contains members and may produce projects. Has members (linked through `part_of`) and optionally projects (linked through `belongs_to`).

### Shared work
A Project or Organization that connects multiple Profiles through participation. The atomic unit of connection in Vínculo.

---

## System terms

### Ghost node
A Profile that has been added to the network by a collaborator (named in a project) but has not yet claimed their node. The ghost still appears in traces — they participated, even if they have not yet shown up to confirm.

### Claiming
The process of confirming identity and activating a Ghost node. Once claimed, the Profile owner can edit their information, add new projects, and name further collaborators.

### Invite
The link sent to a Ghost node owner. Opening the invite shows them their position in the network — already there, already connected — before they have done anything.