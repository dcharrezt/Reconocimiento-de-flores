# Sistema de reconocimiento de especies de flores #

![alt text](https://github.com/uddua/Reconocimiento-de-flores/blob/master/myimage.gif)

## Integrantes ##
* Diego David Charrez Ticona
* Edson Arratea Ope

### Resumen del proyecto ###

* Base de datos **FLOWERS17** and **FLOWERS102**.

[FLOWERS17](http://www.robots.ox.ac.uk/~vgg/data/flowers/17/index.html)

[FLOWERS102](http://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html)
* Modelos usados    - **VGG16, VGG19**.
* Weights used    - **ImageNet**
* Clasificador usado - **Logistic Regression**

### Dependencias ###
* Theano o TensorFlow `sudo pip install theano` or `sudo pip install tensorflow`
* Keras `sudo pip install keras`
* NumPy `sudo pip install numpy`
* matplotlib `sudo pip install matplotlib` tambien se necesita este `sudo apt-get install python-dev`
* seaborn `sudo pip install seaborn`
* h5py `sudo pip install h5py`
* scikit-learn `sudo pip install scikit-learn`

### Requerimientos del sistema
* Este proyecto fue probado en ubuntu 14.04.


### Uso ###
* Organizar base de datos                                - `python organize_flowers17.py`
* Extraccion de caracteristicas usando CNN               - `python extract_features.py`
* Entrenamiento del modelo usando regresion logistica    - `python train.py`

### Numeros ###
Las tablas de abajo muestran la precision obtenida por cada modelo deep neural network para extraer caracteristicas del dateset **FLOWERS17** usando diferentes parametros.

* Resultados-1
  
  * test_size  : **0.10**
  * clasificador : **Logistic Regression**
  
| Modelo       | Rank-1 precision | Rank-5 precision |
|--------------|------------------|------------------|
| VGG16        | 85.29%           | 98.53%           |
| VGG19        | 88.24%           | 99.26%           |

* Resultados-2
  
  * test_size  : **0.30**
  * clasificador : **Logistic Regression**

| Modelo       | Rank-1 precision | Rank-5 precision |
|--------------|-----------------|-----------------|
| VGG16        | 88.24%          | 99.02%          |
| VGG19        | 88.73%          | 98.77%          |
