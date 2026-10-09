# System Design & Architecture

## Overview

This directory contains preliminary system design artifacts for our Final Year Project, including system architecture diagrams, workflow diagrams, component descriptions, and technology considerations.

These artifacts communicate our current understanding of the proposed system and will be updated as research progresses and design decisions are validated.

## Current Design Objectives

Our initial design investigation focuses on:

- Understanding the major components of a microservices monitoring platform.
- Exploring how telemetry can be collected and processed.
- Investigating service dependency graphs and their role in root-cause analysis.
- Evaluating potential machine-learning and graph-based approaches.
- Identifying how detected anomalies and root-cause candidates could be presented through a dashboard.

## Design Artifacts

Design documents and diagrams will be added here as they are developed.

| Artifact | Description | Status |
|---|---|---|
| `system-architecture.md` | Preliminary architecture, component descriptions, and design considerations | To be developed |
| `system-flow.md` | Proposed end-to-end flow of telemetry processing and root-cause analysis | To be developed |
| `diagrams/` | Editable diagram sources and exported visual diagrams | To be developed |

## Technologies Under Investigation

Potential technologies and approaches include:

- **Observability:** OpenTelemetry
- **Machine learning:** Candidate anomaly-detection approaches
- **Graph analysis:** Service dependency graphs and candidate graph algorithms
- **Backend:** NestJS and microservices
- **Dashboard:** Next.js
- **Deployment:** Docker and Kubernetes

ST-GCN, Personalized PageRank, Backcrawl, and other specific approaches remain candidates for investigation rather than finalized requirements.

## Design Principles

- Diagrams should reflect the current proposed system, not unverified assumptions.
- Technology choices should be supported by research and feasibility analysis.
- Significant revisions should be recorded through Git history.
- Each design artifact should clearly identify its purpose and current status.
- Open questions and unresolved decisions should be documented.

## Status

**Current stage:** Preliminary design and proposal preparation.

The architecture and workflow are expected to evolve as we review related work, evaluate feasibility, and incorporate supervisor feedback.
