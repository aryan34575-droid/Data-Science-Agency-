# Data Science Agency

A personalized workspace built on the open-source AI Data Science Team by Business Science.

Upstream project: https://github.com/business-science/ai-data-science-team

The upstream project is distributed under the MIT License. Its original copyright and license notice are retained in `LICENSE`.

## AI Pipeline Studio
The Streamlit app entry point is `apps/ai-pipeline-studio-app/app.py`.

## Run locally
See upstream setup instructions and install dependencies with `pip install -r requirements.txt`, then run:

```bash
streamlit run apps/ai-pipeline-studio-app/app.py
```

Configure model credentials (OpenAI or a supported local Ollama setup) as described in upstream documentation. Do not commit API keys.
