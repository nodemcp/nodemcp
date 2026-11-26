<div align="center">

<img src="https://nodemcp.dev/wp-content/uploads/2026/11/cropped-cropped-NodeMCP_Icon-192x192.png" width="96" height="96" alt="NodeMCP icon" />

# NodeMCP

**Let your AI assistant work on computers and servers you control.**

Remote, OAuth-protected MCP access to authorized **Linux**, **Windows** and supported **Intel macOS** devices. Your device agent initiates an outbound connection to the NodeMCP gateway — no additional inbound management ports or reverse tunnels to configure.

[Website](https://nodemcp.dev/) · [Quickstart](https://nodemcp.dev/quickstart/) · [Documentation](https://nodemcp.dev/docs/) · [Real Linux demo](https://nodemcp.dev/demo/) · [Start free trial](https://app.nodemcp.dev/devices/signup)

</div>

---

## From a chat request to real work

NodeMCP connects an MCP-compatible AI client to a device you have explicitly paired and authorized. The tools available depend on the OS, installed agent, client capabilities and granted permissions.

```text
Your AI client (ChatGPT / Claude / other compatible client)
                       │ OAuth + remote MCP
                       ▼
              NodeMCP gateway
                       ▲ outbound connection
                       │
           Agent on your own device
                       │
                       ▼
           Linux / Windows / Intel Mac
```

**Remote MCP endpoint:** `https://mcp.nodemcp.dev/mcp`  
**Official Registry ID:** [`dev.nodemcp/nodemcp`](https://registry.modelcontextprotocol.io/v0.1/servers/dev.nodemcp%2Fnodemcp/versions/latest)

### What can you do?

| Platform | Example tasks |
|---|---|
| **Linux** | Inspect service health, diagnose logs, manage files and carry out approved terminal tasks. |
| **Windows** | Organize files, compare exported data and prepare documents with available local tools. |
| **Intel macOS** | Run diagnostics and, with the required local permissions, use supported screen or input features. |
| **Android** | Native agent is under QA testing; a public APK is **not yet available**. |

## See a real test

Our [read-only Ubuntu diagnostic example](https://nodemcp.dev/demo/) documents three actual NodeMCP operations and the resulting memory, disk and service checks. It is a sanitized record of a real test — not an anonymous live admin console and not a synthetic chat transcript.

You can also explore [Linux server troubleshooting](https://nodemcp.dev/use-cases/diagnose-linux-server-failures-with-ai/) and additional [use cases](https://nodemcp.dev/use-cases/).

## Get started

1. [Start your free trial](https://app.nodemcp.dev/devices/signup): **72 hours, up to 3 paired devices**.
2. Open the [NodeMCP Control Center](https://app.nodemcp.dev/) and create a one-time pairing code.
3. Follow the [official installer instructions](https://nodemcp.dev/quickstart/) for your supported OS. **Review installer scripts before running them.**
4. Connect your MCP-capable AI client using the [connection guide](https://nodemcp.dev/docs/connecting-ai-clients/) and authenticate via OAuth.
5. Start with a read-only diagnostic request and approve changes only after inspecting the plan.

> **Security matters.** Some NodeMCP tools are privileged. An authorized AI request can affect a real machine. Restrict access to devices you own or administer, maintain backups, and review potentially destructive changes. See the [security model](https://nodemcp.dev/docs/security-model/).

## Documentation & support

- [Docs index](docs/README.md) · [Supported platforms](docs/platforms.md) · [MCP connection](docs/connection.md)
- [Security model](docs/security.md) · [Practical workflows](docs/workflows.md)
- [Support](SUPPORT.md) · [Report a security concern](SECURITY.md)
- [Official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers/dev.nodemcp%2Fnodemcp/versions/latest)

## Registries & directories

Find NodeMCP in the official MCP Registry and independent MCP directories.

[![Listed on MCP Harbor](https://mcpharbor.app/badge/registry-dev-nodemcp-nodemcp.svg)](https://mcpharbor.app/tools/registry-dev-nodemcp-nodemcp/)

- [Official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers/dev.nodemcp%2Fnodemcp/versions/latest) — published server metadata (`dev.nodemcp/nodemcp`).
- [Glama](https://glama.ai/mcp/connectors/dev.nodemcp/nodemcp) — remote MCP connector listing.
- [mcptry](https://mcptry.com/servers/dev.nodemcp/nodemcp) — server listing.
- [MCP Servers](https://mcpservers.org/servers/nodemcp-dev-remote-mcp-server) — hosted MCP server listing.
- [MCP Harbor](https://mcpharbor.app/tools/registry-dev-nodemcp-nodemcp/) — server directory listing.
- [MCP Lantern](https://mcplantern.com/server/sub_02a04364e2c0) — remote MCP server listing.

Directory inclusion does not imply endorsement, security certification or unrestricted access. NodeMCP requires authentication and device authorization.

### About this repository

This repository is the **official public documentation and integration-example home** for the hosted NodeMCP service. **It is not a source-code distribution of the NodeMCP gateway or proprietary device agents.** No open-source software license is implied for the service. Public documentation and examples may be updated independently of agent releases.

NodeMCP is independent and is not affiliated with or endorsed by AI client providers merely because their clients may interoperate with MCP.
