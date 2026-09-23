### 🔭 Currently exploring new bypass methods

- **`2025` · IAM policy bypass on AWS** — Discovered a technique to [bypass user-agent–based IAM restrictions from Python](https://cloud.hacktricks.wiki/en/pentesting-cloud/aws-security/aws-post-exploitation/aws-sts-post-exploitation.html#bypass-user-agent-restrictions-from-python). Some IAM policies condition access on the `aws:UserAgent` string; the method spoofs the SDK's user-agent so requests aren't filtered by these condition keys.

- **`2025` · CodeBuild PrivEsc (Example 3)** — Contributed a PR for the [`iam:PassRole` + `codebuild:CreateProject` + `codebuild:StartBuild` escalation path](https://cloud.hacktricks.wiki/en/pentesting-cloud/aws-security/aws-privilege-escalation/aws-codebuild-privesc/index.html#iampassrole-codebuildcreateproject-codebuildstartbuild--codebuildstartbuildbatch). The technique creates a project with a crafted `hook.json` buildspec that reads the CodeBuild service-role credentials from the container credentials URI (`http://169.254.170.2$AWS_CONTAINER_CREDENTIALS_RELATIVE_URI`) and forwards them to an attacker-controlled webhook — direct privesc to any passable CodeBuild role.

### 🎯 Focus areas

`Web` · `API` · `Cloud`
