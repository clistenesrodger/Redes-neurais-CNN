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

## Dataset utilizado

O notebook utiliza o conjunto Fashion-MNIST — imagens em escala de cinza de tamanho 28×28, com 10 classes (60.000 imagens de treino e 10.000 de teste). Ele é carregado diretamente do Keras com o comando:

```python
from tensorflow import keras
(X_train, y_train), (X_test, y_test) = keras.datasets.fashion_mnist.load_data()
```

No notebook os dados são normalizados (`/255.`) e reshapeados para `(28, 28, 1)` antes do treino.