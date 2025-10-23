<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="media/P4Cyber_W.png">
    <source media="(prefers-color-scheme: light)" srcset="media/P4Cyber.png">
   <img src="media/P4Cyber.png" alt="P4Cyber Logo" width="600"/>
  </picture>
</p>

# **P4Cyber** - **Peers for Cyber**

**Unstoppable · Decentralized · Neutral** 

*CYBER INTELLIGENCE*

A decentralized, verifiable, and unstoppable layer for Internet-wide cyber intelligence 

**built on [Pears](https://docs.pears.com/) by [Holepunch](https://holepunch.to/)**.

---

## **Why This Matters**

The Internet’s public surface is the world’s largest shared digital infrastructure — yet today, visibility into it is mediated by a few centralized entities. These systems, while powerful, introduce single points of failure, policy bias, and fragility. **P4Cyber changes that.**

* **World-first decentralized cyber intelligence:** no central index, no choke points, no gatekeepers.
* **Neutral and ownerless:** no company or nation decides what gets scanned, stored, or queried.
* **Verifiable by design:** append-only logs, signed feeds, reproducible scans.
* **Fresher coverage at global scale:** a swarm of peers outpaces any single data center — more ports, more IPs, more often.

---

## **The Idea in 90 Seconds**

Today’s exposure search engines — like Shodan, Shadowserver, and Censys — are centralized: one operator scans, stores, and serves. That brings power, but also fragility: single policy surface, cost ceilings, limited reach, uneven freshness, and stoppability.

**P4Cyber flips the model.** Anyone can run a node. Nodes collaborate to schedule work, perform scans, sign results, and replicate data across a peer-to-peer fabric. Think *“BitTorrent for cyber exposure”* with built-in guarantees on integrity, provenance, and safety.

**Vision:** a neutral, censorship-resistant, ownerless cyber intelligence layer for the public Internet — *port-wide by default*, with broader IP coverage and higher refresh cadence than any solitary system can sustain.

---

## **Core Principles**

* **Decentralization:** scanning, indexing, and serving via a mesh of peers — no central servers.
* **Neutrality:** an ownerless protocol and signed feeds ensure no single entity controls inclusion or access.
* **Unstoppable:** discovery and replication happen over the swarm; data lives everywhere and nowhere.
* **Verifiability:** append-only logs, cryptographic signatures, and reproducible parameters guarantee trust in proofs, not authorities.

---

## **Philosophy**

Centralized security intelligence is powerful but fragile. P4Cyber rethinks how truth about the Internet is measured and shared. Only a decentralized and verifiable architecture can guarantee reliability and neutrality.

In cybersecurity, truth must not depend on a single operator’s database or a single jurisdiction’s policy. P4Cyber treats Internet measurement as shared infrastructure — governed by protocols and proofs, not by corporate policies or government directives.

* **Decentralized by design →** no single company or state can become a gatekeeper or point of failure for who sees what, or when.
* **Cryptographically verifiable →** results are reproducible and tamper-evident; trust is placed in math and code, not institutions.
* **Neutral and ownerless →** inclusion and behavior are determined by transparent rules that no party can unilaterally bend.

This philosophy ensures that access, distribution, and policy cannot be captured by any one actor. Decisions about how data is shared are transparent and collectively defined, while the protocol guarantees that no single authority can deny, distort, or selectively grant access to a fundamental resource: security.

---

## **Challenges**

P4Cyber is intentionally ambitious: a fully decentralized, neutral, and unstoppable network that continuously maps the Internet’s attack surface and, over time, expands into a broader Cyber Intelligence commons. That scope — global coverage, constant freshness, and trust-by-design without a central operator — poses several challenges:

1. **Internet-scale coverage:** approaching *“all ports over all IPv4”* with meaningful recency (and preparing for IPv6’s vastness), while managing duplication, bias, and ethical rate limits.
2. **Heterogeneous node environments:** running the P4Cyber node reliably across diverse OSes and form factors (server, desktop, mobile) and network conditions, while preserving consistent measurement semantics and reproducibility — without central orchestration. This demands scalable coordination, adaptive load balancing, and resilience across devices.
3. **Incentivizing participation:** designing fair, manipulation-resistant rewards so nodes contribute bandwidth, compute, and storage sustainably, while resisting Sybil attacks and low-quality data.
4. **Jurisdictional resilience:** operating reliably across countries with varying laws and censorship, embedding practical tools that help node operators handle blocks, throttling, and legal constraints — while preserving simplicity and neutrality.

---

## **Future Development**

P4Cyber is currently in an **alpha phase** focused on validating the core idea and stress-testing Internet-scale execution. We are experimenting with **[Pears](https://docs.pears.com/)** as the decentralization layer, evaluating distributed scanning algorithms, and optimizing data structures for peer-driven repositories.

This phase informs the **beta stage**, where the project will operate in production-like conditions with defined objectives — coverage targets, freshness SLAs, proof-of-measurement guarantees, and improved node onboarding UX.

As development progresses, P4Cyber will introduce **operator incentives**, potentially through a **token model** tied to verifiable contributions (bandwidth, compute, storage). These incentives will follow transparent, manipulation-resistant rules that reward active, high-quality participation.

Looking ahead, P4Cyber will integrate **decentralized AI agents** to autonomously perform advanced Cyber Intelligence tasks — such as correlating exposed services, anomaly detection, and trend analysis across peer-generated data. These agents will operate transparently using local compute and federated coordination to preserve privacy, neutrality, and resilience while enhancing collective situational awareness.

In parallel, the platform will evolve beyond surface scanning toward a complete Cyber Intelligence ecosystem — a community-driven resource for neutral-by-design cybersecurity. 

Optionally, as part of this roadmap, we may provide **decentralized VPN tooling** to bolster jurisdictional resilience — a capability relevant not only to P4Cyber’s operations but also to broader efforts that safeguard neutrality and freedom of expression online.

---

## **P4Cyber Alpha**

This section describes the current alpha test for P4Cyber. Note that **the alpha is experimental** and is intended to validate algorithms, peer coordination via Pears, and the use of Hypercore/Hyperbee data structures for decentralized storage and search. The alpha does not include open-source scanning code — it provides instructions for testers to install Pears, run the P4Cyber application, and participate in a controlled test network.

**1) What it is**

P4Cyber Alpha is an early, limited test of the peer-driven scanning and data-replication model. It is not intended to produce a complete Internet-wide index. Instead, it validates core ideas:

Running a P4Cyber node (client or server) that connects to the P2P fabric provided by Pears by Holepunch.

Using Hypercore / Hyperbee for append-only feeds and decentralized searchable repositories across peers.

Exercising distributed scan scheduling, result replication, and decentralized search — all without a central database.

Key constraints of the alpha:

No open-source scanning backend shipped in this repo; the alpha delivers a packaged client for testing.

Limited port scope: the alpha scans ~5,000 common ports (the primary ports) — not full 0-65535 coverage.

Limited distribution of nodes: since the network size is small, coverage is intentionally partial and results are for testing only.

**2) What you can test**

The P4Cyber GUI is required for participating in the alpha. Through the interface you can:

**Set bandwidth allowance** for the node (to avoid saturating local network).

**Start / Stop scanning** sessions manually.

**Search gathered results** via a textual search bar (IP address only).

**Browse results** in a Shodan-like view showing: discovered ports, protocols, banners, and certificates.

**View scanning metrics**: how many blocks the node scanned. In this alpha a block corresponds to scanning a single port across ~600,000 IPs. Metrics are available per-session and historically (since the app was first run on that node).

**Inspect last-block details**: view the data captured for the most recent block scanned by the node.

Limitations and scope:

Results are incomplete by design and only representative of the current alpha network.

Scans are constrained to ~5,000 prioritized ports.

Reproducibility and proofs are being evaluated; some fields or features may be placeholders during alpha.

**3) Install & Run**

Supported OS: Linux 64-bit and Windows 64-bit. No specific distribution or version is required beyond these architectures.

Prerequisites: a machine (server or desktop) with a GUI environment and sufficient network/bandwidth. Mobile clients are not part of this alpha.

**1) Install Pears**
Follow official Pears installation instructions: https://docs.pears.com/

**2) Start (obtain & run)**
The alpha uses Pears’ runtime to obtain and run the application in a single step. Open a terminal and run:

pear run <P4CYBER_KEY>

Replace <P4CYBER_KEY> with the application key distributed to alpha testers.

pear run will download the latest release associated with that key and execute it — there is no separate manual download step.

The command launches the Pears runtime and starts the P4Cyber GUI. The GUI must be running to participate in scanning and to control node settings.

**3) Configure bandwidth and run scans**

In the GUI, set a conservative bandwidth limit before starting. We recommend beginning with a low value and increasing gradually while observing local network impact.

Use the GUI buttons to Start and Stop scans.

**4) Data and storage**

The application stores its local append-only logs and Hypercore/Hyperbee feeds on the node. Data is replicated across peers per Pears’ protocol.

There is no central database: all data is distributed and accessible by peers according to the protocol and feed metadata.

**5) Updates**

This alpha is experimental: updates may be frequent and not always announced. On restart the client will attempt to run the latest published version available to alpha participants.

---

## **4) FAQ**

**Q: Is the alpha performing port scanning?**
A: The alpha performs systematic, non-targeted scans over randomized IP blocks and prioritized port lists for testing algorithmic behavior — not focused attacks against single targets. The operation is similar in nature to what organizations like Shadowserver and Shodan do at scale, but limited in scope for this alpha.

**Q: Is this legal to run?**
A: Laws and ISP terms vary by jurisdiction. Running distributed scanning may be restricted by some ISPs, cloud providers, or national laws. P4Cyber provides this alpha for research and testing; testers are responsible for ensuring compliance with local laws and provider terms. We recommend verifying terms with your ISP or provider and using a VPN or other mitigations if you deem it necessary.

**Q: Can the scans overload my network?**
A: Yes — if bandwidth is set too high. The GUI provides a bandwidth control: start low and increase gradually. Do not set values that saturate your uplink. If you notice network issues, stop the scan immediately.

**Q: Will my node reveal my identity or correlate scans to my organization?**
A: The alpha is designed to operate on randomized IP blocks rather than targeting specific organizations. However, network-level identifiers (source IP) are present in traffic and may be visible to network operators. Use your discretion and consult legal/IT counsel if required.

**Q: Where are the data stored and who controls them?**
A: Data is stored in decentralized feeds (Hypercore/Hyperbee) across participating peers via Pears. There is no central authority holding all data. Access to feeds is governed by the protocol and feed metadata.

**Q: Why no open-source code in this alpha?**
A: The alpha is distributed as a packaged client to simplify onboarding and protect early-stage internals during testing. Project goals remain aligned with openness — we will evaluate what will be published after the alpha depending on security, safety, and operational considerations.

**Q: Is a GUI mandatory?**
A: Yes for alpha participation. The GUI exposes the controls and metrics required for safe testing (bandwidth limit, scanning control, search, and metrics).

**Q: Are there safety or ethical controls built-in?**
A: The alpha includes rate-limiting, randomized block assignments, and protocols to avoid repeated concentrated scans against a single network. These mechanisms are under active testing and refinement.

**Q: What should I do if I encounter problems?**
A: Report issues in the repository’s Issues or Discussions (if enabled), and include:

- OS and environment

- Pears version

- Steps to reproduce

Important legal notice: This FAQ is informational and not legal advice. Testers must ensure they comply with local laws and their service providers’ terms of service.

---

### License & Reverse-Engineering Notice (Alpha)

The P4Cyber alpha client is provided for testing purposes only and is considered **proprietary software** for the duration of the alpha. The definitive licensing model (including any open-source components) will be announced when we enter the beta release.

By participating in this alpha test, you are requested to refrain from:
- reverse engineering, decompiling, disassembling, or attempting to recover source code;
- copying, modifying, redistributing, or creating derivative works from the alpha binaries or packages;
- using the software in ways that violate applicable laws or your provider’s terms of service.

If you have questions or need explicit permission (for example for integration/testing purposes), please contact us.

