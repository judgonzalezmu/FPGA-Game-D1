# PWM ULTRASONIDO

## Integrantes del equipo de trabajo:

### 1. Adriana Mercedes Rivera Gonzalez - amriverag@unal.edu.co
### 2. Heriberto Forero Correa - hforeroc@unal.edu.co
### 3. Gilbert Andrés Angulo Saucedo - gaangulosa@unal.edu.co

## Descripción general del sistema: (tomado del documento de clase)

El módulo de ultrasonido HC-SR04 es un sensor de distancias por ultrasonidos capaz de detectar objetos y calcular la distancia a la que se encuentra en un rango de 2 a 450 cm. consta de dos membranas, de las cuales una emite una señal mecánica de alta frecuencia (trigger) que al encontrarse con algún obstáculo rebota, siendo captada por la membrana receptora (echo), dicha onda inicialmente es un puso de 10uS el cual al llegar al trigger es modulado a una frecuencia de 8 ciclos de ultrasonido a 40kHz. La distancia se puede calcular de dos formas, la primera es tomando el intervalo de tiempo entre  la emisión y recepción en uS y dividiéndolo por 58 si se requiere la distancia expresada en centímetros de lo contrario de necesitarse expresada en pulgadas la división debe ser por 148. La segunda forma de calcular la distancia es tomando en cuenta el tiempo en el cual la señal recibida se encuentra en un nivel alto y dividiéndolo por la velocidad del sonido, tomada como una constante (340m/s).<br />
![hc-sr04](https://user-images.githubusercontent.com/31454781/30242381-05e49d58-955b-11e7-8ddf-e27dde32208e.png)

## Descripción de la caja Funcional  (in/out)

La caja funcional del módulo ultrasonido tiene como entradas, Pulse la cual introduce un pulso de 10uS. Echo en donde se recibe la señal luego de que esta haya rebotado con algún objeto cercano. Clock parte crucial ya que permite establecer el intervalo de tiempo entre la emisión y recepción o la cantidad de tiempo en que la señal recibida se encuentre en el nivel alto, lo que permitiría calcular las distancias. Init que permitiría iniciar el proceso de emisión y recepción de la señal de ultrasonido. Como salidas se tiene Trigger desde la cual se emite la señal de ultrasonido y Distance la cual me proporciona el valor calculado de la distancia del obstáculo cercano.<br />
![caja funcional](https://user-images.githubusercontent.com/31454781/30354225-e3ce2d2c-97f0-11e7-9dac-c3947ffb93b8.png)

## Descripción funcional:
Emisor
![diagrama funcional emisor](https://user-images.githubusercontent.com/31454781/30006058-94d65aba-90b5-11e7-9be5-b66a2653858f.png)
Receptor
![diagrama funcional receptor](https://user-images.githubusercontent.com/31454781/30354235-f4319370-97f0-11e7-8e76-6ad0ec90db2c.png)

## Descripción Estructural:
![descripcion estructural](https://user-images.githubusercontent.com/31454781/30354243-07936dda-97f1-11e7-91cd-a085eb4cba08.png)

## Diagrama de Estados:
![diagrama de estados](https://github.com/Fabeltranm/FPGA-Game-D1/blob/master/HW/RTL/08ULTRASONIDO/Version_01/03%20document/imgs/estados.PNG)


## Arquitectura del periférico:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## Diagrama de bloques del periférico:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## referencias:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

