# count-vehicles-with-yolo

Status: Em desenvolvimento

## Sobre o Projeto

Este projeto tem como objetivo fornecer uma contagem automatizada de veículos a partir de um vídeo contendo tráfego em movimento. Para isso, utilizamos a biblioteca **YOLO (You Only Look Once)**, uma das mais eficientes para detecção de objetos em tempo real, permitindo o reconhecimento de diferentes tipos de veículos.

## Tecnologias Utilizadas

- Python 3.x
- OpenCV
- YOLO (You Only Look Once)
- Jupyter Notebook
- NumPy

## Como Instalar e Executar

### **Clone o repositório**

```sh
git clone https://github.com/seu-usuario/count-vehicles-with-yolo.git
cd count-vehicles-with-yolo
```

### **Crie e ative um ambiente virtual (opcional, mas recomendado)**

#### Para Windows (cmd/powershell):
```sh
python -m venv venv
venv\Scripts\activate
```

#### Para Linux/macOS:
```sh
python3 -m venv venv
source venv/bin/activate
```

### **Instale as dependências**

```sh
pip install -r requirements.txt
```

Caso o arquivo `requirements.txt` ainda não esteja disponível, crie-o com as seguintes dependências:
```txt
opencv-python
numpy
matplotlib
tensorflow
p_utils
torch
torchvision
```

### **Baixe os pesos do modelo YOLO**

O YOLO requer arquivos de pesos pré-treinados. Baixe-os executando:
```sh
wget https://pjreddie.com/media/files/yolov3.weights -P weights/
```
Ou baixe manualmente a partir do link: [YOLO Weights](https://pjreddie.com/media/files/yolov3.weights) e mova para a pasta `weights/`.

### **Execute o notebook**

Certifique-se de ter o Jupyter Notebook instalado:
```sh
pip install jupyter
```
Agora, execute o notebook:
```sh
jupyter notebook
```
Abra o arquivo `code.ipynb` e execute as células para processar o vídeo e contar os veículos automaticamente.
