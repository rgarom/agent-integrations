# Plugin público de nextplan

Incluye el MCP remoto público y la skill de descubrimiento local. No requiere credenciales para buscar. No concede acceso editorial o administrativo.

Codex instala este plugin desde el marketplace público: ejecuta `codex plugin marketplace add rgarom/nextplan-marketplace` y después `codex plugin add nextplan@nextplan`. Abre una tarea nueva para cargarlo. El ZIP contiene la misma fuente para inspección o instalación local. Si tu cliente no admite plugins, añade https://www.nextplan.es/mcp como servidor MCP remoto Streamable HTTP. El formato de configuración varía según el cliente; .mcp.json contiene el endpoint y no necesita ejecutar comandos locales.

Para un entorno de pruebas, cambia únicamente la URL de .mcp.json al origen de ese entorno seguido de /mcp. Para guardados, crea una clave limitada en https://www.nextplan.es/cuenta/conexiones y configura Authorization: Bearer en el almacén privado de credenciales del cliente. Nunca incluyas la clave en este paquete ni en una conversación. No hay flujo OAuth en esta versión.

El paquete no se instala ni se publica automáticamente en directorios externos. La presencia del endpoint no garantiza descubrimiento automático por asistentes.
