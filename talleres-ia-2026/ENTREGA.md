# Entrega — talleres IA 2026

Cada semana se resolvió dentro de su propio directorio y sin mezclar soluciones entre semanas.
Los notebooks se completaron **en el mismo archivo** (los originales siguen en el historial de git).

| Semana | Qué se hizo | Estado |
|---|---|---|
| **4** | `03_lab_warehouse_mdp_estudiantes.ipynb`: clase `WarehouseMDP` (transiciones según piso normal/resbaloso), Value Iteration, Policy Iteration. Los notebooks 01 y 02 se ejecutaron sin cambios y funcionan. | Completo y ejecutado. Mapa tomado de tu imagen (`start`, `walls`, `slippery_states`, `terminal_states`, `danger_states`). Partes 4 y 5 resueltas: preguntas 1–5, predicciones antes de cada experimento, experimentos A/B/C y bonus (umbral de recompensa ≈ -0.80), con VI y PI coincidiendo. |
| **5** | `03_qlearning_taxi`: `choose_action`, `update_q`, `train_q_learning`, curva, antes/después, experimento (α 0.1→0.5) y las 7 preguntas respondidas con números reales. `02_qlearning_frozenlake`: todas las actividades respondidas. `01_cheeseworld`: ejecutado. | Completo y ejecutado (semillas fijas, reproducible). |
| **6** | `wine_challenge/`: el challenge de la guía (`01_data_challenge`, `02_training_challenge`, `03_evaluation_deployment_challenge`) con `wine.csv`, artefactos y reportes. | Completo y ejecutado. `wine.csv` se genera desde `sklearn.datasets.load_wine` porque no venía en el zip. |
| **7** | `Challenge_Keras3_CIFAR10_Grayscale` y `Challenge_Keras3_OlivettiFaces`: todos los `TODO` completados y las preguntas conceptuales respondidas. | Código verificado de punta a punta con datos sintéticos. **Sin ejecutar con datos reales** (descarga bloqueada); las respuestas que dependen de resultados están marcadas como «Pendiente de ejecución». |
| **8** | `yolo/Lecture_08_Yolo_Intro`: ejecutado completo (incluye el ejercicio con tu propia imagen). `transfer_learning/taller_...`: `TODO` completados, problema definido (bicycle / motorcycle / bus), respuestas conceptuales y cierre escritos. | YOLO Intro completo. El taller de transfer learning está verificado con datos sintéticos pero **sin ejecutar con datos reales** (necesita buscador de imágenes y pesos ImageNet). Los notebooks de entrenamiento YOLO con Roboflow no se ejecutaron (no tienen ejercicios por completar). |

## Detalles a tener en cuenta

- `semana8/yolo/images/mi_imagen.jpg` es una imagen de prueba (un gato) para el ejercicio de YOLO. Reemplázala por tu propia foto y cambia `MI_IMAGEN` si quieres.
- Las celdas «Pendiente de ejecución» se completan al correr el notebook donde haya acceso a los datasets.
- `semana8/yolo/apikeys.env` contiene una clave de Roboflow **versionada en git**. Conviene regenerarla y añadir el archivo a `.gitignore`.
- `semana8/yolo/deployment/app_webcam.py`: la lista `MODEL_CHOICES` contiene `"best.py"`, probablemente un error por `"best.pt"`.
