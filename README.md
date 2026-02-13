## Local setup

Dependencies:
```bash
brew install pyenv
brew install pyenv-virtualenv

pyenv install 3.13
pyenv virtualenv 3.13 lnd_env
source ~/.pyenv/versions/3.13.12/envs/lnd_env/bin/activate
pip install -r requirements.txt
```

Verification:
```bash
python env_utils.py
```

## Local run jupyter lab
```bash
jupyter lab
```

## Local run lang-studio
```bash
cd ./module1 # 2,3
langgraph dev
```
