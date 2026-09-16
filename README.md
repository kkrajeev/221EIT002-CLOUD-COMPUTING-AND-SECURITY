# MTech Cloud Computing: Review Topics and Starter Papers

**Purpose.** Topic bank for an MTech review article based on peer-reviewed original publications (minimum 10). Each topic is chosen so a careful review can later become a major-project prototype.

**How to use this file.** Pick one topic. Collect at least 10 peer-reviewed papers (prefer 2022–2026). Write a taxonomy + comparison table + open problems. Convert one open problem into an implementation.

**Preferred venues for papers.** IEEE Transactions on Cloud Computing, IEEE Access, IEEE TPDS / TNSM, ACM Computing Surveys, ACM SoCC, Elsevier Future Generation Computer Systems / Journal of Systems and Software / Computer Networks / Computer Science Review, Springer Cluster Computing / Journal of Cloud Computing / Computing. Strong conference papers from SoCC, Middleware, ICDCS, CCGrid, IEEE CLOUD, IC2E, EuroSys, and NSDI are also acceptable.

**Search strings.**
- `"cloud computing" AND (survey OR "systematic review" OR taxonomy)` with year filter 2023–2026
- `"serverless" AND (edge OR continuum OR "cold start")`
- `"multi-cloud" AND (interoperability OR sovereignty OR orchestration)`
- `"carbon-aware" OR "green cloud" OR FinOps`
- `"federated learning" AND (cloud OR edge) AND (survey OR review)`

---

## Review-to-project method

1. Frame 3–4 research questions (scope, methods, metrics, gaps).
2. Use a PRISMA-style selection note: databases, keywords, inclusion/exclusion, years.
3. Build one taxonomy. Do not write paper-by-paper summaries only.
4. One comparison table: objective, method, dataset, metrics, cloud vs edge, limitations.
5. End with 3 concrete open problems and a one-page candidate project design.
6. Keep citations from IEEE, ACM, Elsevier, Springer, and top conferences.

---

## Topic 1. AI-driven resource allocation and scheduling in cloud / multi-cloud

**Review angle.** Classify RL, heuristics, and hybrid schedulers. Compare SLA, cost, energy, and fairness.

**Starter papers**
- AI-driven resource allocation in cloud computing: a systematic review revealing critical sustainability and evaluation gaps. *Computing* (Springer), 2026.
- Task Scheduling in Cloud Environment–Techniques, Applications, and Tools: A Systematic Literature Review. *IEEE Access*, 2024.
- Public Datasets for Cloud Computing: A Comprehensive Survey. *ACM Computing Surveys*, 2025.
- Also search IEEE TCC and FGCS for reinforcement-learning cloud scheduling, multi-objective VM placement, and Kubernetes DRL autoscaling.

**Project hook.** Carbon-aware or SLA-aware DRL scheduler versus Kubernetes HPA. Report cost, SLA violations, and energy.

---

## Topic 2. Serverless / FaaS across the cloud–edge continuum

**Review angle.** Cold start, function placement, workflows, and FaaS outside the central cloud.

**Starter papers**
- Beyond Cloud: Serverless Functions in the Compute Continuum. *SN Computer Science* (Springer), 2025.
- Serverless Computing for Next-generation Application Development (special issue overview). *Future Generation Computer Systems* (Elsevier), 2025.
- Computation offloading in the edge-to-cloud compute continuum: a survey of federated architectural solutions. *Cluster Computing* (Springer), 2025.
- Also search ACM SoCC, IEEE CLOUD, IC2E, and Middleware.

**Project hook.** Measure cold start versus provisioned concurrency. Place the same function in cloud and edge. Add a simple arrival predictor.

---

## Topic 3. Edge–cloud collaborative computing and distributed intelligence

**Review angle.** Model split, collaborative inference, orchestration under delay and loss.

**Starter papers**
- Edge-Cloud Collaborative Computing on Distributed Intelligence and Model Optimization: A Survey. arXiv:2505.01821 (cite the peer-reviewed version when available).
- The journey to cloud as a continuum: Opportunities, challenges, and research directions. *ICT Express* (Elsevier), 2025.
- Empowering real-time applications through mobile edge computing: Survey on joint computation offloading and data caching. *Computer Science Review* (Elsevier), 2026.
- A Comprehensive Survey on Fog Computing. *Archives of Computational Methods in Engineering* (Springer), 2026.

**Project hook.** Split inference (edge feature extract + cloud model) under injected delay/loss. Report latency and accuracy.

---

## Topic 4. Green cloud, carbon-aware scheduling, and energy-efficient data centers

**Review angle.** PUE versus location-based carbon intensity. Why few papers actually measure carbon.

**Starter papers**
- The Springer *Computing* 2026 SLR on AI resource allocation (flags the carbon-awareness gap).
- Energy and green datacenter papers in *FGCS*, *IEEE TCC*, and *Sustainable Computing: Informatics and Systems* (Elsevier).
- Workload placement using renewable-aware and carbon-intensity traces.

**Project hook.** Schedule batch jobs with electricity carbon-intensity traces versus a cheapest-region baseline.

---

## Topic 5. Multi-cloud, hybrid cloud, interoperability, and digital sovereignty

**Review angle.** Portability, failover, data residency, and consumer-side risk management.

**Starter papers**
- Cloud Outsourcing Risk Management for Cloud Consumers: A Systematic Literature Review. *ACM Computing Surveys*, 2026.
- IEEE TCC papers on interoperability, multi-cloud orchestration, and compliance.
- Surveys on Kubernetes multi-cluster (Cluster API, Anthos/Arc-style) and sovereign cloud.

**Project hook.** Deploy one app on two public clouds plus one on-prem/sovereign cluster. Measure failover time, cost, and residency constraints.

---

## Topic 6. Cloud-native security: Zero Trust, confidential computing, container and Kubernetes security

**Review angle.** Compare TEE, encryption, service mesh, and runtime detection.

**Starter papers**
- A survey on privacy and security in distributed cloud computing: exploring federated learning and beyond. *IEEE Open Journal of the Communications Society*, 2025.
- ACM CSUR / IEEE surveys on container security, live migration security, and secure search over outsourced data.
- *Computers & Security* (Elsevier) and IEEE S&P / CCS / ACSAC papers on confidential VMs (SGX/TDX/SEV) and eBPF/Kubernetes security.

**Project hook.** Threat model plus a hardened cluster path (mTLS + runtime detection + one confidential-compute option).

---

## Topic 7. Federated learning and privacy-preserving ML on cloud / edge-cloud

**Review angle.** Privacy versus accuracy versus communication cost under non-IID and delayed clients.

**Starter papers**
- Federated continual learning: a comprehensive survey. *Neurocomputing* (Elsevier), 2026.
- IEEE OJ-COMS 2025 privacy and security survey (FL, MPC, DP, TEE).
- IEEE TKDE / TMC surveys on federated continual learning and Edge-AI FL.

**Project hook.** Flower or FedML clients on simulated edge nodes with a cloud aggregator. Add dropout and delayed updates.

---

## Topic 8. Cloud–edge offloading, caching, and real-time applications

**Review angle.** Joint offloading and caching for IoT, vehicular, and AR/VR latency targets.

**Starter papers**
- Joint offloading and caching survey. *Computer Science Review* (Elsevier), 2026.
- Federated offloading architectures survey. *Cluster Computing* (Springer), 2025.
- Fog/edge task-scheduling surveys in *Cluster Computing* and *Journal of Cloud Computing*.

**Project hook.** iFogSim2 or EdgeCloudSim scenario. Compare greedy versus DRL offloading.

---

## Topic 9. Quantum-inspired optimization and post-quantum readiness for cloud/fog

**Review angle.** Distinguish quantum-inspired classical algorithms from actual quantum hardware. Cover PQC migration for cloud APIs.

**Starter papers**
- Quantum-inspired algorithms in fog computing: A Systematic Literature Review. *Computers and Electrical Engineering* (Elsevier), 2026.
- Integrative AI + edge + quantum + green-cloud framework papers (IEEE conference 2025 onward).
- Post-quantum TLS / hybrid KEM papers for cloud APIs (NIST PQC context).

**Project hook.** Implement one QEA/QPSO scheduler versus GA/PSO on CloudSim. Discuss PQC migration. Do not claim hardware quantum speedup.

---

## Topic 10. FinOps, AI cost governance, and cloud performance engineering

**Review angle.** Connect token/API cost, autoscaling, spot instances, and SLOs. Academic coverage is thinner than industry coverage, so a careful review has value.

**Starter papers / anchors**
- Public Datasets for Cloud Computing. *ACM Computing Surveys*, 2025 (needed for reproducible cost studies).
- *JSS*, *FGCS*, IEEE CLOUD / ICPE / SoCC papers on cloud cost optimization, spot scheduling, and LLM inference cost.
- Use industry trend reports only as context, then cite peer-reviewed measurements.

**Project hook.** Instrument a microservice plus one LLM API. Compare on-demand, spot, reserved, and serverless cost under the same SLO.

---

## Suggested review-to-project pairing

| Topic | Review focus | Follow-on project |
|---|---|---|
| 1 Scheduling / AI allocation | RL vs heuristics | Custom scheduler or Kubernetes operator |
| 2 Serverless continuum | Cold start + placement | OpenFaaS / Knative experiment |
| 3 Edge–cloud intelligence | Model split + orchestration | Delayed/lossy offloading demo |
| 4 Green cloud | Carbon-metric gap | Carbon-intensity job placer |
| 6 Security | Zero Trust + TEE | Hardened Kubernetes + threat analysis |
| 7 Federated learning | Privacy vs accuracy vs comms | FL under packet loss |

---

## Minimum paper-collection checklist

- [ ] At least 10 peer-reviewed original papers (surveys may be used for mapping, but the review must rest on primary studies)
- [ ] Majority from 2022–2026
- [ ] Mix of IEEE / ACM / Elsevier / Springer
- [ ] At least one comparison table with common metrics
- [ ] Explicit limitations of the existing literature
- [ ] One implementable gap for the major project

---

## Notes for students

Starter citations above are entry points, not a complete bibliography. Always open the publisher page, confirm year/venue/DOI, and add related work from the paper’s reference list and “cited by” list. Prefer primary experiments over blogs. If a source is only on arXiv, look for the journal or conference version before citing it as final.
