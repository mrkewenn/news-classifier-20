# Pre-Requisitos
# Windows
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
# Linux/macOS
curl -LsSf https://astral.sh/uv/install.sh | sh

# Instalacao e Preparacao
Sincroniza o ambiente e instala as dependências (torch, sklearn, pandas, etc):
uv sync

Registra o ambiente virtual como um Kernel do Jupyter:
uv run python -m ipykernel install --user --name news-classifier --display-name "Python (News Classifier)"

# Como rodar o projeto
Inicie o Jupyter Lab:
uv run jupyter lab

No menu lateral, abra o arquivo *"ClassificationFetchNews20.ipynb"*
**Importante**: No canto superior direito do Jupyter, certifique-se de que o Kernel selecionado é o "Python (News Classifier)".
Execute as células (Shift + Enter) sequencialmente.
