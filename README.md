# Integraciones para agentes de Rafa Garrido

Catálogo público preparado para distribuir varios proyectos en asistentes compatibles.

## Proyectos disponibles

- [nextplan](https://www.nextplan.es/asistentes): descubre planes locales mediante MCP.
- [Dupo](https://dupo.es/asistentes): busca y compara muebles y decoración mediante MCP.

## Codex

```bash
codex plugin marketplace add rgarom/agent-integrations
codex plugin add nextplan@rgarom
codex plugin add dupo@rgarom
```

Instala solo los proyectos que quieras usar. Abre una tarea nueva después de instalarlos.

## Claude Code

```bash
claude plugin marketplace add rgarom/agent-integrations
claude plugin install nextplan@rgarom
claude plugin install dupo@rgarom
```

Instala solo los proyectos que quieras usar. Recarga los plugins si Claude Code lo solicita.

## Otros asistentes

Los clientes compatibles con MCP remoto pueden conectarse directamente a:

- Nextplan: `https://www.nextplan.es/mcp`
- Dupo: `https://mcp.dupo.es`

Cada proyecto vive en `plugins/<proyecto>` y comparte sus recursos comunes. Los manifiestos de cada plataforma permanecen separados.
