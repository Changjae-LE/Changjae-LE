# Hi, I'm Changjae Lee

Building Reliable and Secure Cloud Systems

I'm pursuing an M.S. in Computer Science at the University of Southern California,
with an expected graduation in May 2027.

I'm interested in technologies that keep cloud systems reliable and secure.
I enjoy automating repetitive tasks and building tools that automatically
identify and resolve problems.

## Featured Projects

| Project | Engineering focus | Implementation |
|---|---|---|
| [PipelineFixRL](https://github.com/Changjae-LE/pipelinefixrl) | Kubernetes troubleshooting and automated remediation | Collects runtime evidence, derives deterministic patches, and validates repairs through Docker builds and deployments in kind |
| [CJGate](https://github.com/Changjae-LE/cjgate) | DevSecOps and CI security enforcement | Integrates Gitleaks and Semgrep with a local GitHub Actions policy gate and a separate Midnight live proof path |
| [ProofOps](https://github.com/Changjae-LE/proofops) | Incident verification and service operations | Analyzes evidence locally, generates demo receipts, and exposes health endpoints, metrics, structured logs, and a recovery runbook |

### PipelineFixRL — Diagnose and recover

Python · Kubernetes · Docker · Helm · kind · FastAPI · GitHub Actions

- Iterative repair: derive a patch, build, deploy, validate, and use new evidence to refine it.
- Repair provenance distinguishes derived results from fallback and unsuccessful attempts.
- Archived v2 evaluation: 5/8 held-out scenarios repaired, with golden fallback disabled.
- The frozen agent's three novel relationship cases remained unsolved; the benchmark
  documents those boundaries alongside the successful repairs.

[Architecture](https://github.com/Changjae-LE/pipelinefixrl/blob/master/docs/ARCHITECTURE.md)
· [Evaluation methodology](https://github.com/Changjae-LE/pipelinefixrl/blob/master/docs/GENERALIZATION.md)

### CJGate — Enforce security before deployment

TypeScript · GitHub Actions · Gitleaks · Semgrep · Docker · Midnight Compact

- Blocks CI when scanner signals violate the secret/SAST policy.
- Tests both PASS and BLOCK outcomes using explicit fixtures.
- Uses read-only GitHub Actions permissions and keeps scanner details out of public gate output.
- Separates local policy evaluation from the live zero-knowledge proof and transaction path.

[Security workflow](https://github.com/Changjae-LE/cjgate/blob/main/.github/workflows/cjgate-security-gate.yml)

### ProofOps — Verify evidence and expose operational signals

TypeScript · Node.js · Express · Docker · Vitest · GitHub Actions

- Browser-local incident analysis, evidence commitments, and containment-time policy evaluation.
- Liveness, readiness reporting, Prometheus-compatible metrics, and structured JSON logs.
- Graceful shutdown and a multi-stage non-root container with a health check.
- The default receipt is a local demo; live on-chain submission is not implemented.

[Runbook](https://github.com/Changjae-LE/proofops/blob/main/docs/RUNBOOK.md)
· [Integration status](https://github.com/Changjae-LE/proofops/blob/main/docs/MIDNIGHT_STATUS.md)

## Technologies Used in These Projects

- Infrastructure: Kubernetes, Docker, Helm, kind
- Automation: GitHub Actions, Python, TypeScript
- Security: Gitleaks, Semgrep, policy enforcement, evidence privacy
- Reliability: deployment validation, health checks, metrics, repair provenance, runbooks

## Azure Learning Direction

I'm extending this foundation toward Microsoft Azure infrastructure and cloud security.
My learning priorities include Infrastructure as Code, identity and access control,
network security, AKS, and observability. The projects above demonstrate my current
Kubernetes, CI/CD, security automation, and service operations work.

## Opportunities

I'm interested in Cloud Infrastructure, Cloud Security, SRE, and DevOps
opportunities where I can build reliable platforms and automate security controls.

