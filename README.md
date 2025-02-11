# cancer-cnn

Este repositorio contiene una solución al reto de Kaggle [Histopathologic Cancer Detection](https://www.kaggle.com/competitions/histopathologic-cancer-detection/code) en el que se utilizan redes neuronales convolucionales (CNN) para la detección de cáncer metastásico en imágenes histopatológicas.  

## Descripción  
- Se entrenan varios modelos mediante **transfer learning**, utilizan el modelo preentrenado [**ResNet-50**](https://arxiv.org/abs/1512.03385) para extraer características de las imágenes. Se entrenan 7 modelos los cuales varían en ajustes de hiperparámetros.
- Se aplica un **ensamble por votación** para mejorar la precisión final del modelo completo. 

## 📂 Datos  
Los datos no están incluidos en este repositorio. Deben descargarse desde Kaggle:  
[Data Histopathologic Cancer Detection](https://www.kaggle.com/competitions/histopathologic-cancer-detection/data)  

Si se ejecuta en Kaggle, el dataset ya está disponible en `/kaggle/input/histopathologic-cancer-detection/`.  

## 📜 Estructura  
- `train_models.ipynb` → Entrena CNN con distintas configuraciones.  
- `ensemble_voting.ipynb` → Carga los modelos entrenados y realiza un ensamble por votación.  
