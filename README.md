# electiva-inteligencia-artificial

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15Tj8wl2HOKooz7hta_nNW6mLTJh8f1yt?usp=sharing )
> **Sugerencia:** abre el notebook en una nueva pestaña (Ctrl+clic o ⌘+clic) para conservar este repositorio abierto.

# Red neuronal para estimar síntomas depresivos mediante hábitos de pantalla y sueño

Modelo de aprendizaje profundo desarrollado con TensorFlow/Keras para estimar la puntuación de síntomas depresivos (BDI-II) a partir de variables relacionadas con el tiempo de pantalla y los hábitos de sueño en adolescentes.

## Dataset

El proyecto utiliza el conjunto de datos "Screen Time vs Mental Health (ML-Ready)", derivado del estudio longitudinal de Hökby et al. (2025), con información de 4.810 adolescentes suecos.

Variables utilizadas:
- Tiempo de pantalla
- Calidad del sueño
- Duración del sueño
- Variables categóricas codificadas

Variable objetivo:
- Puntuación BDI-II (0–63)

## Arquitectura

Input
↓
Dense(64, ReLU)
↓
Dropout(0.3)
↓
Dense(32, ReLU)
↓
Dropout(0.2)
↓
Dense(16, ReLU)
↓
Dense(1, Linear)

Optimizador:
- Adam

Función de pérdida:
- MSE

Métrica:
- MAE
<img width="1189" height="390" alt="Unknown" src="https://github.com/user-attachments/assets/2f0ba47d-5309-4130-9783-29b533cadf36" />
