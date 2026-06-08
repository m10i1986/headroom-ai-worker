# Headroom AI Proxy
Headroom AI Proxy is a kit designed to help you perform the initial setup of Headroom 
(https://github.com/chopratejas/headroom) Proxy.

## Start
```bash
# Install tools
sudo dnf install curl tmux cpp g++ clang

# Install uv
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install Claude Code
curl -fsSL https://claude.ai/install.sh | bash

# Setup
mkdir -p ${HOME}/workspace/headroom-ai-proxy
cd ${HOME}/workspace/headroom-ai-proxy
uv python install 3.13
uv sync

# LiteLLM Vulnerability Response
uv pip install --upgrade --no-deps "litellm>=1.83.7"

# Start
./start.sh
```

## License
MIT License - see LICENSE file for details.
