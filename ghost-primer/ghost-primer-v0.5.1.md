![Warhollow Ghost Primer Banner](../branding/warhollow-ghost-primer.svg)

### v0.5.1 — Explicit Boundaries
© 2026 Warhollow LLC. All rights reserved.

> “Autonomy means systems that operate independently within controlled boundaries.”  
> — Warhollow Ghost Fragment

---

## What Warhollow Is

Warhollow is a sovereign compute environment designed for those who require explicit control over where and how computation occurs.

It runs on physically controlled hardware and uses enterprise-grade virtualization to isolate workloads within clearly defined trust boundaries.

Warhollow does not attempt to eliminate trust.  
It narrows the trust surface and makes governance explicit.

---

## Why It Exists

Modern infrastructure optimizes for scale, convenience, and abstraction.

Abstraction simplifies usage.  
It also obscures governance.

Warhollow was built on a different premise:

**If you cannot explain who governs the system, you cannot meaningfully assess its risk.**

Warhollow favors explicit boundaries over diffuse dependence.

---

## Governance & Roles

Each Warhollow environment operates within a unified control domain.

Roles are defined clearly to prevent ambiguity.

### Infrastructure Custodian

The Infrastructure Custodian maintains:

- Physical custody of hardware  
- The virtualization substrate (hypervisor and host system)  
- Network topology and segmentation  
- Provisioning and lifecycle of virtual machines  

The Custodian governs the control plane of the environment.  
There is no external governance layer.

The Custodian does not operate customer workloads.  
The Custodian maintains the substrate upon which they run.

---

### Workload Owner

A Workload Owner operates within an isolated virtual machine provisioned inside a Warhollow environment.

The Workload Owner controls:

- The operating system within their VM  
- Application-level configuration  
- Cryptographic credentials inside their execution context  
- Workload-specific policies  

Workload Owners do not control:

- Physical hardware  
- The hypervisor  
- Other virtual machines  
- The environment’s control domain  

Isolation between workloads is enforced at the hypervisor layer.

---

## Control Plane & Substrate

Warhollow maintains unified governance across:

- The physical substrate  
- The virtualization control plane  

No external cloud control plane provisions, migrates, or replicates workloads.

Access to workload data outside the virtual machine requires deliberate administrative action at the substrate layer.

Trust is not abstracted across unknown entities.  
It is concentrated and accountable.

---

## Data Residency

Data residency within a Warhollow environment is defined by physical custody.

- The hardware location defines the jurisdictional footprint.  
- Data does not migrate silently.  
- There is no automatic cross-region replication.  
- There is no external control plane capable of relocation.  

Residency is structural, not declarative.

---

## Layered Protection

Warhollow encourages separation between:

- Infrastructure substrate  
- Workload execution  
- Canonical data custody  

In many deployments:

- Compute runs inside the environment.  
- Canonical datasets remain under the Workload Owner’s control.  
- Access occurs through deliberate interfaces, not implicit sharing.  

Isolation reduces unnecessary exposure.  
Retention can be minimized by design.

---

## Threat Model

Warhollow is designed to reduce risks associated with:

- External cloud governance layers  
- Implicit multi-tenant trust  
- Opaque infrastructure abstraction  
- Silent data relocation  
- Unbounded telemetry  

It assumes physical custody is controlled and virtualization boundaries are enforced.

Warhollow does not eliminate trust.  
It replaces diffuse trust with structured governance.

---

## Explicit Non-Goals

Warhollow does not claim:

- Zero-knowledge guarantees  
- Immunity from legal jurisdiction  
- Elimination of insider risk  
- Absolute protection from physical seizure  

No system removes trust entirely.

Warhollow narrows where trust must reside and makes those boundaries visible.

---

## Who It’s For

Warhollow is designed for individuals and organizations that require:

- Explicit trust boundaries  
- Predictable governance  
- Clear custody of infrastructure  
- Explainable system architecture  

It is suited to environments where infrastructure decisions carry legal, political, or operational consequence.

Warhollow is not optimized for hyperscale elasticity.  
It is optimized for clarity.

---

## Philosophy

Warhollow is not built on secrecy.  
It is built on explicit boundaries.

It favors:

- Discipline over drama  
- Governance over abstraction  
- Signal over noise  

It is restrained by design.  
And deliberate by necessity.
