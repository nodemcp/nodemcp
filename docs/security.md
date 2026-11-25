# Security model and safe operating practices

NodeMCP provides **authorized remote control**, not a read-only chat viewer.

- **Identity and authorization:** access to the MCP gateway is protected by OAuth; devices must be paired with a NodeMCP account.
- **Connection direction:** the device agent initiates an outbound connection; you do not have to publish a new inbound management port or reverse tunnel for NodeMCP.
- **Powerful tools:** depending on device, operating system and granted permissions, tools may read or modify files, execute commands, restart services or interact with the desktop.
- **Local OS controls:** macOS screen recording and accessibility/input still require the device owner's system-level permissions where applicable.
- **Human review:** test on a disposable VM, keep backups and authorize risky actions explicitly.

Recommended first prompt:

> Inspect my paired test machine and report the operating system, memory, storage and failed services. Explain what you found. Do not install software, modify files, restart services or reboot the machine without my approval.

For full, current details, read the [NodeMCP security and permissions documentation](https://nodemcp.dev/docs/security-model/). To report a vulnerability privately, see [SECURITY.md](../SECURITY.md). Do not put credentials or private user data into public issues.
