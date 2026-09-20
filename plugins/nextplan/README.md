# Nextplan para asistentes

Incluye el MCP remoto público y la skill de descubrimiento local. No requiere credenciales para buscar. No concede acceso editorial o administrativo.

El catálogo público `rgarom/agent-integrations` distribuye la integración para varios asistentes.

En Codex, ejecuta `codex plugin marketplace add rgarom/agent-integrations` y después `codex plugin add nextplan@rgarom`. Abre una tarea nueva para cargarlo.

En Claude Code, ejecuta `/plugin marketplace add rgarom/agent-integrations` y después `/plugin install nextplan@rgarom`. Recarga los plugins si el cliente lo solicita.

El ZIP contiene la misma fuente para inspección o instalación local. Si tu cliente no admite plugins, añade https://www.nextplan.es/mcp como servidor MCP remoto Streamable HTTP. El formato de configuración varía según el cliente; `.mcp.json` contiene el endpoint y no necesita ejecutar comandos locales.

Para un entorno de pruebas, cambia únicamente la URL de .mcp.json al origen de ese entorno seguido de /mcp. Para guardados, crea una clave limitada en https://www.nextplan.es/cuenta/conexiones y configura Authorization: Bearer en el almacén privado de credenciales del cliente. Nunca incluyas la clave en este paquete ni en una conversación. No hay flujo OAuth en esta versión.

La presencia del endpoint o del marketplace no garantiza que un asistente recomiende nextplan sin que el usuario haya conectado o instalado antes la integración.
