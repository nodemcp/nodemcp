# Supported devices and availability

NodeMCP is a hosted remote MCP gateway with agents running on devices you authorize. Individual platform capabilities depend on the agent build, permissions and installed software.

| OS | Current public guidance | Where to check |
|---|---|---|
| Linux | Released agent; terminal, files, diagnostics and service-related operations are supported where authorized | [Linux installation](https://nodemcp.dev/docs/linux-installation/) |
| Windows x64 | Released agent; real-machine automation depends on installed tools and Windows privileges | [Windows installation](https://nodemcp.dev/docs/windows-installation/) |
| Intel macOS | Released on verified Intel Mac configurations; screen/input capabilities require explicit local macOS permission | [macOS installation](https://nodemcp.dev/docs/macos-installation/) |
| Apple Silicon Mac | Not independently verified as equivalent to the tested Intel Mac configurations | [macOS installation](https://nodemcp.dev/docs/macos-installation/) |
| Android | Native agent exists in QA; **no publicly released universal APK yet** | [Android status](https://nodemcp.dev/docs/android-status/) |

Don't assume an AI client supports every remote MCP transport, authentication flow or tool. See the [client connection guide](https://nodemcp.dev/docs/connecting-ai-clients/).
