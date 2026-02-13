## Local setup

### Dependencies:
```bash
brew install pyenv
brew install pyenv-virtualenv

pyenv install 3.13
pyenv virtualenv 3.13 lnd_env
source ~/.pyenv/versions/3.13.12/envs/lnd_env/bin/activate
pip install -r requirements.txt
```

### AI model dependency (OpenAI has no free tier)
```yaml
  curl -fsSL https://ollama.com/install.sh | sh
  ollama pull lfm2.5-thinking # example model to pull - this one works well on cpu device ~0.7gb
  ollama list # verification
  curl http://localhost:11434/api/tags # api verifications - list models
```

### Basic Verification:
```bash
python env_utils.py
```

## Local editor
```bash
jupyter lab
```

## Model UI interaction
```bash
cd ./module1
# based on notebooks/module-1/langgraph.json
langgraph dev --tunnel
```

## Links
- https://ollama.com/
- https://www.tavily.com/ search web engine for AI agents (even crawling)
- https://academy.langchain.com/courses/take/foundation-introduction-to-langchain-python/lessons/71234859-module-2-introduction