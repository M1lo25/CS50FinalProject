# CS50 Intro to Cybersecurity – Final Project
**Case Study:** XZ Utils Backdoor (CVE-2024-3094)

This repository supports my 7-10 minute presentation on the XZ Utils backdoor, including a recap of the backdoor, the mechanism for the backdoor via release tarballs, and relevant supply-chain mitigations.

## Materials
- **Slides (PDF):** ./slides/Progetto_finale.pdf
- **References:** ./References.md
- **Video (Unlisted):** [youtube-link](https://youtu.be/hZiRb05Liw0)

## Key Takeaways
- **Tarball ≠ Git:** enforce artifact–tag parity in CI; fail on any mismatch.
- **Supply-chain hardening:** attestations (in-toto), SBOMs, SLSA ≥ L3, two-person review.
- **Detect & recover:** monitor sshd anomalous behavior/symbol interposition; retain tested rollback playbooks.

## Incident Snapshot
- **CVE:** CVE-2024-3094  
- **When:** March-April 2024  
- **Impact focus:** risk to SSH auth via indirect dependency chain (ex. sshd → libsystemd → liblzma)

## Acknowledgments
**Andres Freund**, these files acknowledge everyone in the distro for finding and remediating this.

---

**Presenter:** Gianluca Milani,edX: Gianluca25,GitHub: M1lo25  
**Recorded Date:** 16/10/2025
