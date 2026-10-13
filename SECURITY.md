# Security policy

Management OS, Inc. welcomes reports from security researchers. This file summarizes our published [vulnerability disclosure policy](https://app.mgmt-os.ai/security-policy). If the two ever differ, the published policy governs.

## Report a vulnerability

Report privately, in either of two ways:

- **On GitHub:** open the affected repository's **Security** tab and choose **Report a vulnerability**. These reports are handled under the same published policy.
- **By email:** [security@mgmt-os.ai](mailto:security@mgmt-os.ai). If the report is sensitive, ask for a secure channel and we will arrange one.

Include a description of the issue, the steps to reproduce it, and any proof of concept that helps us confirm it. Please don't open a public issue for a security problem.

Machine-readable contact: [mgmt-os.ai/.well-known/security.txt](https://mgmt-os.ai/.well-known/security.txt)

## What to expect from us

- We acknowledge every report, typically within two business days.
- We investigate promptly, keep you updated on our assessment, and tell you when the issue is resolved.
- We credit you for the discovery if you'd like, once the issue is fixed.

We don't run a paid bug bounty. We offer public acknowledgment.

## What we ask of you

- Give us a reasonable window to investigate and fix the issue before any public disclosure.
- Make a good-faith effort to avoid privacy violations, data destruction and any interruption to the service.
- Only use accounts you own or have explicit permission to test. Do not access, change or copy other customers' data.
- Don't run automated scanning that degrades the service, and don't use social engineering, physical attacks or denial of service.

## Safe harbor

We will not pursue or support legal action against researchers who act in good faith and in accordance with the published policy. The full safe-harbor terms are in the [policy](https://app.mgmt-os.ai/security-policy).

## Scope

**In scope:** the Management OS application and its APIs at mgmt-os.ai and its subdomains. That includes the MCP server at `https://app.mgmt-os.ai/api/mcp`, which the plugin and connectors in this organization use.

For the AI-assistant integration, we especially want to hear about anything that:

- lets one workspace read another workspace's data
- gets past sign-in, or uses a token for something it wasn't granted
- makes a read-only tool send, change or delete anything
- lets text inside shared evidence steer a tool into revealing data it shouldn't

**Out of scope:** our sub-processors' own infrastructure (report those to the provider directly), findings that require a compromised device or account, and best-practice suggestions without a demonstrable security impact. Our sub-processors are listed at [mgmt-os.ai/subprocessors](https://mgmt-os.ai/subprocessors).

The management-os-plugin repository holds no code and no credentials; its tools run on Management OS servers. If you find a file in any of our public repositories that points somewhere it shouldn't, report it the same way.
