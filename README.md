# RAGAgentic

Notebook educativo en español para recorrer un flujo RAG + LangGraph en Colab o Jupyter local.

## Quick path

1. Open `Script_LangGraph_para_Colab_y_Diagrama.ipynb`.
2. Run the setup cells from top to bottom.
3. Set your API keys when the notebook asks for them.

## What it covers

- Instalación de dependencias para Colab.
- Carga de una base RAG con Chroma + embeddings de Hugging Face.
- Grafo LangGraph con `StateGraph`, `START` y `END`.
- Ruta opcional de búsqueda web con Tavily.
- Visualización del grafo y demo opcional con Gradio.

## Colab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HaroldSthid/LangChain_AgentAI_Basic/blob/main/Script_LangGraph_para_Colab_y_Diagrama.ipynb)

Ese enlace asume que el notebook se publicará en `HaroldSthid/LangChain_AgentAI_Basic` dentro de la rama `main`.

## GitHub Pages note

Si publicas este repositorio con GitHub Pages, usa `docs/index.md` como landing page. La portada enlaza al notebook en GitHub para evitar rutas rotas cuando Pages se sirve desde `docs/`.

## Run locally

- Python 3.10+
- Jupyter Notebook or JupyterLab
- Optional API keys: `GROQ_API_KEY`, `TAVILY_API_KEY`, `LANGCHAIN_API_KEY`
