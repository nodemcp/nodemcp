# Connect an AI client using remote MCP

NodeMCP exposes an **OAuth-protected Streamable HTTP MCP endpoint**:

```text
https://mcp.nodemcp.dev/mcp
```

The corresponding official MCP Registry identifier is [`dev.nodemcp/nodemcp`](https://registry.modelcontextprotocol.io/v0.1/servers/dev.nodemcp%2Fnodemcp/versions/latest).

## Connection checklist

1. Create a [NodeMCP account](https://app.nodemcp.dev/devices/signup) and pair a supported device in the [Control Center](https://app.nodemcp.dev/).
2. Follow the official [AI client connection instructions](https://nodemcp.dev/docs/connecting-ai-clients/) for your client. Use the HTTPS URL above, not a localhost or machine-specific management port.
3. Complete the OAuth sign-in requested by the client. An anonymous HTTP request returning **401 Unauthorized** is expected for a protected endpoint, not by itself an outage.
4. Inspect the granted tool permissions. Ask for a harmless read-only check first.
5. Review privileged or destructive actions before allowing them.

> Never commit OAuth tokens, pairing codes, secret environment variables, private keys, device identifiers, logs containing credentials or captured authentication callbacks to this repository or GitHub Issues.

Individual clients differ. Some require a separate connector setup or have limitations on remote MCP and OAuth. The [official compatibility instructions](https://nodemcp.dev/docs/connecting-ai-clients/) take precedence over generic third-party examples.
