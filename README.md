# Integraciones de agentes de Rafa Garrido

Catálogo público preparado para distribuir varios proyectos en asistentes compatibles.

## Proyectos disponibles

- [nextplan](https://www.nextplan.es/asistentes): descubre planes locales mediante MCP.

## Codex

```bash
codex plugin marketplace add rgarom/agent-integrations
codex plugin add nextplan@rgarom
```

Abre una tarea nueva después de instalar el plugin.

## Claude Code

```text
/plugin marketplace add rgarom/agent-integrations
/plugin install nextplan@rgarom
```

Recarga los plugins si Claude Code lo solicita.

## Otros asistentes

Los clientes compatibles con MCP remoto pueden conectarse directamente a `https://www.nextplan.es/mcp`.

Cada proyecto vive en `plugins/<proyecto>` y comparte sus recursos comunes. Los manifiestos de cada plataforma permanecen separados.
