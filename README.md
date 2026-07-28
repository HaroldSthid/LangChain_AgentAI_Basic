# LangChain_AgentAI_Basic · RAGAgentic

Notebook educativo en español para recorrer un flujo RAG + LangGraph en Colab o Jupyter local, usando OpenRouter como proveedor principal. El sitio público y el notebook viven en `HaroldSthid/LangChain_AgentAI_Basic`; esta carpeta local se usa como espacio de preparación.

## Quick path

1. Open `Script_LangGraph_para_Colab_y_Diagrama.ipynb`.
2. Run the install cell.
3. Set the required OpenRouter key and any optional keys.
4. Build or reload the vector store.
5. Run the graph and the minimal tests.
6. Enable Gradio only if you want the UI.

## What it covers

- Instalación de dependencias para Colab o Jupyter local.
- Carga de una base RAG con Chroma + embeddings de Hugging Face.
- Grafo LangGraph con `StateGraph`, `START` y `END`.
- Ruta opcional de búsqueda web con Tavily.
- Visualización del grafo y demo opcional con Gradio.

## Colab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HaroldSthid/LangChain_AgentAI_Basic/blob/main/Script_LangGraph_para_Colab_y_Diagrama.ipynb)

Ese enlace apunta al notebook principal publicado en `HaroldSthid/LangChain_AgentAI_Basic` dentro de la rama `main`.

## GitHub Pages note

Si publicas este repositorio con GitHub Pages, usa `docs/index.html` como landing page. La portada enlaza al notebook en GitHub y Colab para evitar rutas rotas cuando Pages se sirve desde `docs/`.
La demo estable de Gradio debe vivir en un hosted app como Hugging Face Spaces, y las trazas de LangSmith deben compartirse como links públicos sanitizados o capturas, no como un embed autenticado.
Gradio en Pages usa `TU_USUARIO/TU_SPACE` como placeholder hasta tener el Space real.

## Run locally

- Python 3.10+
- Jupyter Notebook or JupyterLab
- Required API key: `OPENROUTER_API_KEY` (or `OPENROUTER_AGENTICRAG_API_KEY` if you keep the project-specific name)
- Optional API keys: `TAVILY_API_KEY` for web search, `LANGCHAIN_API_KEY` for LangSmith traces/observability
## Execution notes

- If the kernel restarts, rerun the vector-store cell first; it reloads persisted Chroma when available and falls back to local documents if needed.
- Set `DEBUG_RAG_FLOW=1` only when you want diagnostic prints.
- Keep Gradio optional: the notebook only launches it when the flag is enabled in the Gradio cell.
