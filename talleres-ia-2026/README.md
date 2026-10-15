# Talleres de Introducción a la IA (2026)

Soluciones de los talleres de las semanas 4 a 8. Cada semana está en su propia carpeta y los ejercicios se completaron en los notebooks originales.

## Contenido

| Semana | Carpeta | Tema |
|---|---|---|
| 4 | `semana4/` | MDP en gridworld: Value Iteration, Policy Iteration y el laboratorio del almacén (`WarehouseMDP`) |
| 5 | `semana5/` | Q-learning en CheeseWorld, FrozenLake y Taxi |
| 6 | `semana6/` | Pipeline de clasificación y challenge con el dataset Wine |
| 7 | `semana7/` | Redes fully-connected en Keras 3: Fashion-MNIST, CIFAR-10 en escala de grises y caras Olivetti |
| 8 | `semana8/` | Transfer learning con EfficientNet y detección con YOLO |

## Cómo ejecutarlo

Hace falta Python 3.10 o superior y Jupyter.

```bash
pip install jupyter numpy matplotlib pandas scikit-learn joblib gymnasium tensorflow keras
```

La semana 8, además, usa Ultralytics, OpenCV y Gradio:

```bash
pip install ultralytics opencv-python gradio pillow
```

Abre el notebook y ejecútalo de arriba hacia abajo. En la semana 5 las semillas están fijas para poder repetir los resultados. En la semana 6, `wine_challenge/01_data_challenge.ipynb` genera `data/raw/wine.csv` desde `sklearn.datasets.load_wine` si el archivo no viene en el material.

## Estado

- Semanas 4, 5 y 6: notebooks ejecutados, con salidas guardadas.
- Semana 7: los `TODO` de CIFAR-10 y Olivetti están completos. Falta correrlos con los datasets reales; las respuestas que dependen del entrenamiento están marcadas como pendientes.
- Semana 8: la introducción a YOLO está ejecutada. El taller de transfer learning (`bicycle` / `motorcycle` / `bus`) tiene el código listo y falta entrenarlo con imágenes propias y los pesos de ImageNet.

## Notas

- No subas `semana8/yolo/apikeys.env`. Ahí va la clave de Roboflow y no debe quedar en el repositorio.
- En `semana8/yolo/deployment/app_webcam.py`, la opción `"best.py"` de la lista de modelos debería ser `"best.pt"`.
