# Redes-neurais-CNN

## Ambiente virtual Python

### Linux

Crie e ative o ambiente virtual com os comandos abaixo:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Windows

No PowerShell, use:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

No Prompt de Comando (cmd), use:

```bat
python -m venv .venv
.venv\Scripts\activate.bat
```

### Instalação das dependências

Depois de ativar o ambiente, instale as bibliotecas com:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Se for usar o notebook no VS Code, o `ipykernel` já está incluído no `requirements.txt`, então a instalação acima também deixa o ambiente pronto para seleção do kernel.