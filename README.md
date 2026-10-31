# Proposing-Machine
A machine that proposes new ideas and meanings.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Propose something, machine." \
  | uvx proposing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install proposing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
proposing-machine -a multilogue.txt
```
Or:
```bash
proposing-machine multilogue.txt > response.txt
```
Or:
```bash
proposing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import proposing_machine
```
