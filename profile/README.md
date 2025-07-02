<p align="center">
  <img src="https://github.com/kvm-i7/.github/blob/main/profile/logo.png?raw=true" alt="KVM-i7 Logo" width="150">
</p>

<h1 align="center">KVM-i7 Hosting</h1>

<p align="center">
  <strong>Raw Metal. Zero Bloat. Your Box, Your Rules.</strong>
</p>

<p align="center">
  <a href="https://discord.gg/t3vps"><img src="https://img.shields.io/badge/Join_our_Discord-2.1K%2B_Members-5865F2?style=for-the-badge&logo=discord&logoColor=white"></a>
  <a href="https://panel.kvm-i7.host/"><img src="https://img.shields.io/badge/Official_Panel-API_Powered-A6D8E8?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0iI2ZmZiI+PHBhdGggZD0iTTQgNmgxNnYxMEg0eiIvPjwvc3ZnPg=="></a>
    <a href="https://kvm-i7.host/status.html"><img src="https://img.shields.io/badge/Service_Status-Online-23a55a?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0iI2ZmZiI+PHBhdGggZD0iTTEyIDE3LjI3TDQuNSAxMi41bDEuNDE0LTEuNDE0TDExIDE0LjQ0bDYuMDgtNi4wOEwxOC41IDEyLjV6Ii8+PC9zdmc+"></a>
</p>

Welcome to the official GitHub organization for KVM-i7! We provide lifetime, one-time payment LXC VPS hosting for builders, developers, and hobbyists who value freedom and raw performance. This is hosting without the hand-holding.

## What We're About

*   ⚙️ **Lifetime Ownership:** Pay once. Own your VPS slot forever. No monthly bills, ever.
*   🚀 **Developer-First:** Manage everything via Discord bot commands or our simple, powerful REST API.
*   🗽 **Absolute Freedom:** We don't police your content. Host your websites, game servers, bots, or development projects. As long as you don't abuse the shared CPU, you're free to build.
*   🤖 **Automation-Focused:** Our entire platform is built on automation, from crypto payments with OxaPay to server management via the API.

---

## The KVM-i7 REST API

Our core philosophy is to empower users. The same API that powers our Discord bot and official web panel is available to you. Automate your workflow, build custom tools, or integrate your KVM-i7 VPS into your existing applications.

### Quick Start Guide

*   **Base URL:** `https://platform.kvm-i7.host/api`
*   **Authentication:** Your VPS SSH Token (found via the `!manage` command in Discord) is your API key. Pass it as a Bearer Token in the Authorization header.

> **Warning:** Your API token is a password. Keep it secret and do not share it. Use it only in applications you trust.

### Example Usage with `curl`

**1. Get VPS Status**
```bash
# Replace <your-token> with your actual token
curl https://platform.kvm-i7.host/api/status \
  -H "Authorization: Bearer <your-token>"

# Expected Response:
# {"status":"success","data":"status: running"}
```
2. Execute a Command
```
# This example runs 'ls -la' on your VPS
curl -X POST https://platform.kvm-i7.host/api/exec \
  -H "Authorization: Bearer <your-token>" \
  -H "Content-Type: application/json" \
  -d '{"command": "ls -la"}'

# Expected Response:
# {"status":"success","output":"total 24\ndrwxr-xr-x 1 root root 1024 Jul 28 12:00 .\n..."}
```

---

## Getting Started

Ready to get your own lifetime VPS?

1.  **Join our [Discord Server](https://discord.gg/t3vps)** - This is our main hub for community and management.
2.  **Choose a Plan** - Check out the available plans on our [website](https://kvm-i7.host/#plans).
3.  **Request Your VPS** - In the appropriate channel on Discord, use the command `!request {plan} {ssd/hdd}`.
4.  **Pay & Deploy** - Our bot will provide an OxaPay link. Once paid, your server is deployed automatically.
5.  **Manage Your Box** - Use `!manage {vps-id}` to get your credentials, or start building with the API!

## Community & Contributions

The KVM-i7 platform is for the community, by the community.

*   **Build Something Cool:** Have an idea for a tool, a script, or a new panel? Use the API and build it!
*   **Share Your Project:** If you build a useful open-source tool, let us know. We feature community projects in our **[Trusted 3rd Party Panels List](https://kvm-i7.host/trusted)**.
*   **Contribute:** Found a bug or have a suggestion? Open an issue in the relevant repository. We welcome pull requests for our open-source projects.

Have questions? The best place to ask is in our **[Discord](https://discord.gg/t3vps)**.
