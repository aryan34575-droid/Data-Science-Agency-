# Data Science Agency

A Streamlit-based AI data science workspace built on the open-source **AI Data Science Team** framework by Business Science.

**Upstream project:** https://github.com/business-science/ai-data-science-team  
**Upstream license:** MIT — see [LICENSE](LICENSE). Original copyright and license notices are retained.

## Included in this repository

- Core `ai_data_science_team` Python package and agent implementations
- Supervisor and multi-agent Pandas / SQL analyst workflows
- AI Pipeline Studio Streamlit app
- Exploratory Copilot, Pandas Data Analyst and SQL Database Agent Streamlit apps
- Root dependency manifest and setup configuration
- Selected upstream planning and application documentation

Large upstream datasets, notebooks, image assets, bytecode caches and test fixtures were not copied in this initial import to keep the repository lighter. This is an application-source import, not a byte-for-byte Git history mirror.

## Recommended app to deploy

**AI Pipeline Studio**

- Main file: `apps/ai-pipeline-studio-app/app.py`
- Python package: root directory
- Dependencies: root `requirements.txt`

## Run locally

Python 3.10+ recommended.

```bash
python -m venv .venv
# Windows PowerShell
.venv\\Scripts\\Activate.ps1
# macOS/Linux
source .venv/bin/activate

pip install -r requirements.txt
pip install -e .
streamlit run apps/ai-pipeline-studio-app/app.py
```

Configure your model provider (OpenAI API key or supported local Ollama setup) using the application's supported settings. Never commit API keys or credentials to GitHub.

## Deploy on Streamlit Community Cloud

1. Open https://share.streamlit.io/ and connect GitHub.
2. Choose **Create app** and select this repository.
3. Branch: `main`.
4. Main file path: `apps/ai-pipeline-studio-app/app.py`.
5. Deploy and review build logs. If dependency resolution fails, address the specific package/version issue before retrying.

## Other included apps

- `apps/exploratory-copilot-app/app.py`
- `apps/pandas-data-analyst-app/app.py`
- `apps/sql-database-agent-app/app.py`

Each app has its own README; the primary deployment recommendation is AI Pipeline Studio.

## Attribution

This project incorporates source code from Business Science's AI Data Science Team under the MIT License. The upstream license is included in this repository. Please review upstream documentation and notices before redistributing or operating a modified version.

## Security and operational notes

- Do not upload confidential, regulated or personally identifiable datasets to a public demo without appropriate access controls.
- Store API keys in the hosting platform's secrets manager, not source files.
- Validate generated code, SQL, cleaning transformations and model outputs before relying on them for business decisions.
- This repository has not yet undergone a complete production security, dependency or deployment audit.
