# Instalação detalhada

Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_pref_rs_porto_alegre_issqn`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_pref_rs_porto_alegre_issqn` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_pref_rs_porto_alegre_issqn` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_pref_rs_porto_alegre_issqn` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.pref_rs_porto_alegre_issqn` (ou `servers.pref_rs_porto_alegre_issqn` no VS Code) do config do cliente e reinicie.
