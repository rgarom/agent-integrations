# Dupo para asistentes

Incluye el MCP remoto público y la skill de búsqueda y comparación de muebles. No requiere credenciales, no compra productos y no concede acceso de escritura al catálogo.

El catálogo público `rgarom/agent-integrations` distribuye la misma integración para Codex y Claude Code.

## Codex

```bash
codex plugin marketplace add rgarom/agent-integrations
codex plugin add dupo@rgarom
```

Abre una tarea nueva después de instalar el plugin.

## Claude Code

```bash
claude plugin marketplace add rgarom/agent-integrations
claude plugin install dupo@rgarom
```

Recarga los plugins si Claude Code lo solicita. La skill queda disponible con el espacio de nombres del plugin y Claude puede invocarla cuando la petición encaja.

## MCP directo

Si el cliente no admite plugins, añade `https://mcp.dupo.es` como servidor MCP remoto Streamable HTTP. El formato de configuración varía según el cliente; `.mcp.json` contiene el endpoint y no ejecuta comandos locales.

Los precios, el stock y las condiciones de compra deben confirmarse siempre en la tienda original. La presencia del endpoint o del marketplace no garantiza que un asistente use Dupo si el usuario no ha conectado o instalado antes la integración.
