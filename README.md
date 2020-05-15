# Distanciamiento Social con Vision Computacional
Proyecto realizado con python, deep learning and computer vision to monitor social distancing.
Credito de idea: LandingAI

[![Watch the video](/images/cover.png)](https://www.youtube.com/watch?v=kxFwbn7Tap0&feature=emb_title)

# How to install?
Es recomendable crear un nuevo entorno virtual para este proyecto e instalar las dependencias. Se pueden seguir los siguientes pasos para descargar comenzar con el proyecto

## Clone the repository
```
git clone https://github.com/guillermodxh/SocialDistancingBirdEye
```
## Install required packages
El archivo requerimientos.txt proporcionado se puede usar para instalar todos los paquetes requeridos. Usa el siguiente comando

```
pip install –r requirements.txt
```


## Ejecutar el proyecto
```
cd SocialDistancingAI
python main.py --videpath "video.mp4"
```

Al ejecutar main.py se abrirá una ventana del primer fotograma del video. En este punto, el código espera que el usuario marque 6 puntos haciendo clic en las posiciones apropiadas en el marco.

#### Primeros 4 puntos:
Los primeros 4 entre los 6 puntos requeridos se utilizan para marcar la Región de interés (ROI) donde desea monitorear. Además, las líneas marcadas por estos puntos deben ser líneas paralelas en el mundo real como se ve desde arriba. Por ejemplo, estas líneas podrían ser los bordes de la carretera. Estos 4 puntos deben proporcionarse en un orden predefinido que sigue.

* __Point1 (ai)__:  abajo a la izquierda
* __Point2 (ad)__: abajo a la derecha
* __Point3 (Ai)__: arriba a la izquierda
* __Point4 (Ad)__: arriba a la derecha



#### Últimos 2 puntos:
Los últimos dos puntos se usan para marcar dos puntos separados 6 pies en la región de interés. Por ejemplo, esto podría ser la altura de una persona (más fácil de marcar en el marco)

El siguiente gif ayudará a comprender mejor los puntos
![mark4points](images/mark4points.gif)
![mark4points](images/pedestrian.gif)

## ¿Como funciona?
El diagrama de bloques completo del algoritmo se puede ver a continuación.
![Block Diagram](images/block_diagram.png)


## Advertencia
Ejecutar desde PC debido a que colab tiene algunas restricciones.
__Créditos de idea: LandingAI__
