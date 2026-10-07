# Hey, I'm ex16x41

Outside of EPCYBER, I spend my time learning and practicing offensive security concepts across **Web, API, and Cloud security**.

A lot of my offensive work starts from reading public research, bug bounty write-ups, documentation, and real-world findings, then turning that material into notes, personal labs, methodologies, and things I can actually apply during authorized testing. I'm not posting OSINT here, only purely offensive research. 

### 🔭 Bypass methods identified

- **AWS IAM policy bypasses** — Researched and documented a technique for bypassing IAM conditions based on `aws:UserAgent` by modifying the SDK user-agent used by Python clients.

- **AWS CodeBuild privilege escalation** — Contributed research around an `iam:PassRole` + `codebuild:CreateProject` + `codebuild:StartBuild` escalation path involving CodeBuild service-role credentials.

- **Bug bounty methodology** — Building simple, example-driven playbooks that focus less on memorizing payloads and more on understanding **why something works, why it fails, and what to try next**.

### 📚 Public Bug Bounty Notes

I keep a public collection of methodologies, notes, examples, and practical references here:

**[public-bb](https://github.com/ex16x41/public-bb)**

The goal is to keep the material practical and easy to follow using a **KISS — Keep It Simple, Stupid** approach.

Current areas include:

- API pentesting methodology
- XSS testing methodology
- recon and attack-surface mapping
- bug bounty workflows
- real-world write-up notes
- failure → observation → pivot → result examples
- vulnerability chaining concepts

The material is collected from public research, documentation, other researchers' write-ups, and my own notes and testing experience. Credit belongs to the original researchers where applicable.

Everything here is for authorized security research, labs, ctfs, and bug bounty programs.
