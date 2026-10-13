# Aegis-RCA: Week 6 Progress Update

**Project Title:** Aegis-RCA: A Clock-Immune Spatial-Temporal Graph Architecture for Real-Time Microservice Root-Cause Analysis  
**Reporting Period:** Weeks 1 – 6 (Academic Schedule)  
**Project Manager:** Abdul Wahab  
**Team:** Abdul Wahab (Project Manager / AI Lead), [Partner Name] (DevOps / Backend Lead)  
**Date:** October 13, 2026  

---

## 1. Executive Progress Summary

During Weeks 1 through 6, the Aegis-RCA team completed all initial project initiation, proposal defense, literature review, and testbed provisioning milestones. 

**Milestone MS-1 (Proposal Defense & Requirements Finalization)** was formally achieved at Week 4 with the approval of our IEEE-compliant Final Year Project Proposal. As of Week 6, **Activity A2 (Testbed Setup, Virtual User Simulation & Dataset Creation)** is actively underway, with the target Kubernetes microservice benchmark environment deployed, initial Locust load generator scripts configured, and preliminary Chaos Mesh fault injection scenarios verified.

---

## 2. Completed Activities & Milestone Status

| Activity ID | Task Description | Timeline | Status | Key Deliverables |
| :--- | :--- | :--- | :--- | :--- |
| **A1** | Literature Review & Requirement Specification | Weeks 1–4 | **100% Complete** | Approved FYP Proposal & Technical Specification Document (**Milestone MS-1 Achieved**) |
| **A2** | Testbed Setup, Virtual User Simulation & Dataset Creation | Weeks 5–8 | **50% In Progress** | Kubernetes / AWS EKS cluster, Sock Shop deployment, Locust user scripts, Chaos Mesh fault CRDs |
| **A3** | Data Ingestion Pipeline & Redis Streaming Buffer | Weeks 9–12 | Pending | Scheduled for Weeks 9–12 |

---

## 3. Key Accomplishments (Weeks 1–6)

### Activity A1: Literature Review & Requirement Specification (Weeks 1–4) — [Completed]
* Conducted a literature review of AIOps root-cause analysis frameworks (MicroRCA, CauseRCA, Graph-based RCA) and identified core gaps regarding inter-node clock skew and unmonitored dependency blindness.
* Formulated the mathematical and architectural specification for the two-tier Aegis-RCA framework (Tier 1 ST-GCN anomaly gatekeeper paired with Tier 2 Personalized PageRank trace traversal).
* Finalized and defended the formal FYP Proposal document.

### Activity A2: Testbed Setup, Virtual User Simulation & Dataset Creation (Weeks 5–8) — [In Progress]
* Provisioned the Kubernetes cluster environment on AWS EKS.
* Deployed the **Sock Shop** benchmark microservice application, verifying inter-service communication and OpenTelemetry trace span generation.
* Configured **Locust** load generators to simulate continuous virtual user traffic across dynamic browsing, cart management, and checkout flows.
* Integrated **Chaos Mesh** into the Kubernetes cluster and executed test fault injections (CPU throttling and synthetic network packet loss).

---

## 4. Team Contributions & Task Distribution

### Abdul Wahab (Project Manager / AI & Algorithmic Lead)
* Authored and structured the complete technical FYP proposal, methodology specifications, and project plan WBS.
* Defined the mathematical formulations for the ST-GCN adjacency/feature matrices and parent-child trace span PageRank graph walk.
* Set up the PyTorch Geometric development environment and prepared baseline graph data preprocessors.

### [Partner Name] (DevOps, Backend & Frontend Lead)
* Configured the Kubernetes cluster infrastructure and AWS EKS deployment manifests.
* Deployed Sock Shop benchmark microservices and configured OpenTelemetry sidecar collectors.
* Developed Locust Python user simulation scripts and validated Chaos Mesh fault injection CRDs on the cluster.

---

## 5. Immediate Next Steps (Weeks 7–8)

1. **Complete Baseline & Abnormal Telemetry Dataset Generation:** Run extended multi-hour Locust traffic sessions under pristine conditions (normal baseline) and inject structured Chaos Mesh faults (CPU throttling, memory leaks, packet loss, and clock skew) to export labeled ground-truth datasets.
2. **Initiate Activity A3 (Data Ingestion Pipeline):** Begin development of the OpenTelemetry-to-Redis streaming worker to buffer high-throughput trace span batches into RAM for fast inference.
3. **Prepare for Milestone MS-2:** Ensure telemetry pipeline, dataset, and testbed verification deliverables remain on track for Week 12 evaluation.
