# Almeidafly

**Defense-oriented software engineering for the systems that have to keep working.**

Almeidafly is a sole-proprietor engineering shop founded by [Joshua Almeida](https://github.com/fitzyracing1) in New Bedford, MA. We build open tooling that makes software supply chains verifiable, CI pipelines honest, and telemetry and autonomous systems easier to trust.

## Mission

Make mission software provably buildable and tamper-evident, from the dependency tree to the test run, and publish the work in the open so anyone can check it.

## Capability areas

- **Software supply-chain assurance**: dependency risk tracking, controlled patched-dependency delivery, and detection of silently changing defaults.
- **CI hardening**: least-privilege GitHub Actions, security scanning, merge-result testing, and detection of faked or weakened tests.
- **Space and telemetry tooling**: reproducible pipelines for public mission data, thermal modeling, and load-aware compute throttling.
- **Autonomous systems**: approval-gated robot control loops with allowlists and kill switches, plus mobile sensor logging.

## Selected public work

Upstream contributions (open-source pull requests; status shown as of November 2026, not endorsements by the projects' owners):

| Project | Contribution | Status |
|---|---|---|
| NASA | [nasa/api-docs#267](https://github.com/nasa/api-docs/pull/267): fix release tracker on multi-line commit messages | Open |
| NASA | [nasa/vira#7](https://github.com/nasa/vira/pull/7): fix stb FetchContent with a pinned commit | Open |
| NASA | [nasa/meza#77](https://github.com/nasa/meza/pull/77): fix SBOM workflow schedule and script path | Open |
| NASA | [nasa/hermes#317](https://github.com/nasa/hermes/pull/317) / [#318](https://github.com/nasa/hermes/pull/318): F Prime cache image and string-length-prefix fixes | Open |
| NASA | Security hardening of GitHub Actions: [bplib#268](https://github.com/nasa/bplib/pull/268), [ncompare#377](https://github.com/nasa/ncompare/pull/377), [vira#8](https://github.com/nasa/vira/pull/8), [api-docs#268](https://github.com/nasa/api-docs/pull/268), [meza#78](https://github.com/nasa/meza/pull/78) | Open |
| NSA | [NationalSecurityAgency/seabee#64](https://github.com/NationalSecurityAgency/seabee/pull/64): fix container kernel-devel install in CI | Open |
| NVIDIA | [NVIDIA/OpenShell#5625](https://github.com/NVIDIA/OpenShell/pull/5625): queue SQLite writers in-process to avoid "database is locked" | Open |

Tooling we maintain:

- **Supply chain and CI**: [patch-cloud](https://github.com/fitzyracing1/patch-cloud) (opt-in npm registry that serves a fixed fork while upstream CI is failing), [lit-dark](https://github.com/fitzyracing1/lit-dark) (reproducible lit/dark CI status standard), [fakegreen](https://github.com/fitzyracing1/fakegreen) (detects skipped, deleted, or weakened tests in agent-written diffs), [merge-guard](https://github.com/fitzyracing1/merge-guard) (tests the merged result of every PR and blocks merges that would break CI), [knobs](https://github.com/fitzyracing1/knobs) (tracks default parameters that change silently between versions).
- **Space and telemetry**: [marslog](https://github.com/fitzyracing1/marslog) (daily cache and per-sol changelog of public NASA Mars rover data, with a Curiosity air-temperature model), [heatgate](https://github.com/fitzyracing1/heatgate) (pauses heavy compute when the machine runs hot). Concept in progress: combining the two so rover-class compute can throttle ahead of forecast thermal limits.
- **Autonomous systems**: [x-robot](https://github.com/Almeidafly/x-robot) (approval-gated browser robot with a localhost allowlist and a STOP kill switch), [phone-robot](https://github.com/fitzyracing1/phone-robot) (Android GPS, activity, and motion logging to a self-hosted server).

## Contact

Joshua Almeida, founder: [Fitzyracing1@gmail.com](mailto:Fitzyracing1@gmail.com) · [almeidafly.github.io](https://almeidafly.github.io)

Almeidafly does not currently hold security clearances or government contracts, and nothing here implies endorsement by NASA, NSA, NVIDIA, or any other organization.
