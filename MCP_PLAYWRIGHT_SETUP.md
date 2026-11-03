# Configuración del MCP de Playwright

## ¿Qué es Playwright MCP?

Playwright MCP (Model Context Protocol) es una herramienta que permite a Claude interactuar con navegadores web de manera programática usando Playwright, facilitando la automatización de pruebas, web scraping y otras tareas relacionadas con la navegación web.

## Instalación

La configuración del MCP de Playwright se encuentra en el archivo `.mcp.json` en la raíz del proyecto:

```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@playwright/mcp@latest"]
    }
  }
}
```

### Verificación

Para verificar que el MCP está correctamente instalado:

```bash
npx @playwright/mcp@latest --version
```

Versión actual instalada: **0.0.83**

## Uso

Una vez configurado, OpenCode y Claude pueden:
- Abrir navegadores web
- Navegar a URLs específicas
- Interactuar con elementos de la página
- Ejecutar scripts en el contexto del navegador
- Tomar capturas de pantalla
- Rellenar formularios y enviar datos

## Próximos pasos

1. Reinicia la sesión de OpenCode para que cargue la configuración
2. El MCP estará disponible automáticamente para Claude
3. Puedes usar comandos como `mcp__playwright__*` en tus tareas

## Documentación

- [Playwright Documentation](https://playwright.dev/)
- [Model Context Protocol](https://modelcontextprotocol.io/)
