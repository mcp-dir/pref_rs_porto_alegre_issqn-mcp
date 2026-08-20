---
name: pref_rs_porto_alegre_issqn-mcp
description: Skill da REST API do Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN na MCP.AI: 1 endpoint em /api/pref_rs_porto_alegre_issqn. Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN, consulta em fonte oficial. Hospedado pela plataforma, sem credenciais da plataforma, pague por consulta com crédito pré-pago. Autentique com workspace API key (sk_live) gerada em app.mcp.ai/settings/api-keys. Use quando o usuário pedir algo coberto pelos endpoints.
---

# Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN — REST API skill

Você tem acesso à **Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN** REST API na MCP.AI.

> Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN, consulta em fonte oficial. Hospedado pela plataforma, sem credenciais da plataforma, pague por consulta com crédito pré-pago.

## Base URL

```
https://api.mcp.ai/api/pref_rs_porto_alegre_issqn
```

Todo endpoint é um **POST** na Base URL + o path abaixo. Os parâmetros vão no corpo JSON.

## Autenticação

Inclua em toda request:

```
Authorization: Bearer sk_live_...
Content-Type: application/json
```

> Gere sua chave em **https://app.mcp.ai/settings/api-keys** (workspace API key `sk_live_…`, não expira, revogável). Uma única chave serve pra todos os seus MCPs.

## Formato de resposta

```json
{ "ok": true, "tool": "<tool_id>", "result": <payload> }
```

## Exemplo cURL

```bash
curl -X POST https://api.mcp.ai/api/pref_rs_porto_alegre_issqn/consultar \
  -H "Authorization: Bearer sk_live_..." \
  -H "Content-Type: application/json" \
  -d '{}'
```

## Reportar problemas

Se um endpoint retornar erro, vazio ou dado inesperado, reporte (não desista calado): **POST /api/pref_rs_porto_alegre_issqn/report** com `{ "message": "...", "context"?: "...", "conversation"?: [...] }`. Isso notifica o time da MCP.AI.

## Endpoints (1)

#### `pref_rs_porto_alegre_issqn_consultar`

Prefeitura RS Porto Alegre: Comprovante de Inscrição do ISSQN, consulta em fonte oficial. _(POST /api/pref_rs_porto_alegre_issqn/consultar)_

| Parâmetro | Tipo | Obrigatório | Descrição |
|---|---|---|---|
| `cnpj` | string | Não | Parâmetro de consulta "cnpj". |
| `cpf` | string | Não | Parâmetro de consulta "cpf". |
| `ie` | string | Não | Parâmetro de consulta "ie". |
| `nire` | string | Não | Parâmetro de consulta "nire". |

---

Este MCP também funciona via **conexão MCP** (Claude / Cursor) em `https://api.mcp.ai/p_pref_rs_porto_alegre_issqn` — veja o [README](../../README.md). A skill acima é pra consumir a **REST API** direto (agente próprio / código).
