# Clasificador de Osos con fastai y PyTorch 

Este proyecto es una implementación paso a paso de un clasificador de imágenes de osos (grizzly, negro, teddy) utilizando las bibliotecas `fastai` y `PyTorch`, siguiendo las enseñanzas del libro "Deep Learning for Coders with fastai & PyTorch". El notebook guía a través de la configuración del entorno, la descarga de datos, el preprocesamiento, el entrenamiento del modelo, la interpretación de resultados y finalmente, la creación de una sencilla aplicación interactiva dentro del propio notebook.

##  Índice

1.  [Configuración del Entorno](#configuración-del-entorno)
2.  [Recopilación de Datos](#recopilación-de-datos)
3.  [Limpieza Inicial de Datos](#limpieza-inicial-de-datos)
4.  [Creación de DataLoaders (DataBlock)](#creación-de-dataloaders-datablock)
5.  [Aumento de Datos (Data Augmentation)](#aumento-de-datos-data-augmentation)
6.  [Entrenamiento del Modelo](#entrenamiento-del-modelo)
7.  [Interpretación y Limpieza Adicional de Datos](#interpretación-y-limpieza-adicional-de-datos)
8.  [Exportación y Carga del Modelo para Inferencia](#exportación-y-carga-del-modelo-para-inferencia)
9.  [Creación de una Aplicación Interactiva en el Notebook](#creación-de-una-aplicación-interactiva-en-el-notebook)
10. [Cómo Ejecutar](#cómo-ejecutar)
11. [Tecnologías Utilizadas](#tecnologías-utilizadas)

## Configuración del Entorno

Para comenzar, es necesario instalar y configurar las bibliotecas necesarias.

```python
#hide
!pip install -Uqq fastbook
#import fastbook
#fastbook.setup_book()

# Importamos todas las herramientas y funcionalidades del módulo fastbook
from fastbook import *
# Importamos los widgets del módulo fastai.vision
from fastai.vision.widgets import *
import os
