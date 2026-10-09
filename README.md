# Hey, I'm ex16x41

Outside of EPCYBER, I spend my time learning and practicing offensive security concepts across **Web, API, and Cloud security (recently considering to dive into mobile too)**.

A lot of my offensive work starts from reading public research, bug bounty write-ups, documentation, and real-world findings, then turning that material into notes, personal labs, methodologies, and things I can actually apply during authorized testing. I'm not posting OSINT here, only purely offensive research. 

### 🔭 Bypass methods identified

- **`2025` · IAM policy bypass on AWS** — Discovered a technique to [bypass user-agent–based IAM restrictions from Python](https://cloud.hacktricks.wiki/en/pentesting-cloud/aws-security/aws-post-exploitation/aws-sts-post-exploitation.html#bypass-user-agent-restrictions-from-python). Some IAM policies condition access on the `aws:UserAgent` string; the method spoofs the SDK's user-agent so requests aren't filtered by these condition keys.

- **`2025` · CodeBuild PrivEsc (Example 3)** — Contributed a PR for the [`iam:PassRole` + `codebuild:CreateProject` + `codebuild:StartBuild` escalation path](https://cloud.hacktricks.wiki/en/pentesting-cloud/aws-security/aws-privilege-escalation/aws-codebuild-privesc/index.html#iampassrole-codebuildcreateproject-codebuildstartbuild--codebuildstartbuildbatch). The technique creates a project with a crafted `hook.json` buildspec that reads the CodeBuild service-role credentials from the container credentials URI (`http://169.254.170.2$AWS_CONTAINER_CREDENTIALS_RELATIVE_URI`) and forwards them to an attacker-controlled webhook — direct privesc to any passable CodeBuild role.

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

**Note:** This GitHub account, including my comments, workflows, methodologies, repositories, and any other content published here, pulls, merges etc, is maintained in a personal capacity and is not affiliated with, endorsed by, or representative of any employer, company, client, or other organization or GitHub users.

If this account or its content is mentioned, referenced, or shared by others, that is solely their own choice and does not imply any affiliation, endorsement, or official relationship.


---

### 🔗 Other Contributions & Mentions

A few other projects and public resources I've contributed to or been mentioned in:

- **[LeakIX](https://leakix.net/credits)** — Credited as [@ex16x41](https://twitter.com/ex16x41) for ideas, testing, and technical discussions on new plugins.
- **[OSINT Google Dork Scanner — Firefox Add-on](https://addons.mozilla.org/en-US/firefox/addon/osint-google-dork-scanner/)** — Mentioned in the add-on's shoutouts for the **Notion Scan** Google dork (`@ex16x41`).
- **[Google Hacking Database (GHDB)](https://www.exploit-db.com/google-hacking-database)** — Submitted Google dorks to GHDB in the past.

