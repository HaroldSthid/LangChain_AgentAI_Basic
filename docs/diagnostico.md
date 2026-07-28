# Diagnóstico y recomendaciones de ejecución

Guía corta para ejecutar el notebook sin perder tiempo cuando Colab reinicia o una clave falta.

## Orden recomendado

1. Instala dependencias.
2. Configura OpenRouter.
3. Ejecuta la celda de la base vectorial.
4. Revisa el grafo.
5. Corre las pruebas mínimas.
6. Activa Gradio solo al final.

## Claves

- **Obligatoria**: `OPENROUTER_API_KEY` o `OPENROUTER_AGENTICRAG_API_KEY`.
- **Opcionales**: `TAVILY_API_KEY`, `LANGCHAIN_API_KEY`.

## Si el kernel se reinicia

- Vuelve a ejecutar primero la celda de la base vectorial.
- Si `vector_store` no existe, la celda debe recargar Chroma desde disco o crear un respaldo local.

## Gradio

- La UI es opcional.
- Si no se lanza, revisa el flag `ENABLE_GRADIO` dentro de su celda.

## Depuración

- `DEBUG_RAG_FLOW=1` habilita impresiones diagnósticas.
- Déjalo en `0` para una ejecución limpia en clase.
